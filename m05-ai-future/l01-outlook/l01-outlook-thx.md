# Lab 5.1: Wohin die Reise geht: verbundene KI

**Leitfragen:**

<details>
<summary>Wie viele verschiedene Programme laufen im eigenen Arbeitstag – und sprechen sie miteinander?</summary>

Meist fünf bis zehn: Mail, Kalender, Chat, Ablage, Fachsysteme. Oft sprechen sie kaum miteinander; Menschen kopieren Inhalte von einem ins andere.

</details>

<details>
<summary>Was wäre anders, wenn ein KI-Modell auf dem eigenen Rechner liefe statt im Internet?</summary>

Die Eingaben verlassen das Haus nicht. Dafür braucht es eigene, leistungsfähige Hardware und jemanden, der das Modell betreibt und aktualisiert.

</details>

<details>
<summary>Wer sollte entscheiden, worauf ein KI-Assistent zugreifen darf?</summary>

Nicht der Assistent selbst. Die Organisation legt Berechtigungen fest, und der Mensch bestätigt einzelne Zugriffe.

</details>

- Heute: ein Chatfenster, in das Texte kopiert werden.
- Morgen: KI, die direkt mit Dateien, Kalendern und Fachsystemen verbunden ist – im Rahmen klarer Berechtigungen.

## Begriffe

| Begriff | Bedeutung |
| ------- | --------- |
| MCP (Model Context Protocol) | offener Standard, über den ein KI-Werkzeug auf Dateien, Kalender, Datenbanken oder Fachsysteme zugreifen kann – wie ein einheitlicher USB-C-Stecker für KI |
| MCP-Server | kleines Programm, das einen Zugang bereitstellt, z. B. zu einem bestimmten Ordner oder Kalender |
| MCP-Client | das KI-Werkzeug, das diese Zugänge nutzt |
| lokales Modell | KI-Modell, das auf eigenen Rechnern oder Servern läuft statt beim Anbieter im Internet |
| offenes Modell | Modell, dessen Dateien heruntergeladen und selbst betrieben werden dürfen |
| Verbindungsschicht | System zwischen Modellen, Wissen, Programmen und Berechtigungen, das festlegt, was wohin darf |

## MCP: ein Stecker statt vieler Kabel

Ohne gemeinsamen Standard braucht jede Kombination aus KI-Werkzeug und Programm eine eigene Anbindung. Fünf Werkzeuge und zehn Programme ergeben bis zu fünfzig Einzellösungen. MCP ersetzt das durch einen gemeinsamen Stecker:

```text
 KI-Modell
    │
 MCP-Client (das KI-Werkzeug)
    │   einheitliche Sprache: MCP
    ├────────────────┬────────────────┬────────────────┐
 MCP-Server       MCP-Server       MCP-Server       MCP-Server
 Dateien          Kalender         Datenbank        Fachsystem
```

Die offizielle MCP-Dokumentation zeigt dasselbe Bild: links die KI-Anwendungen, rechts Datenquellen und Werkzeuge, in der Mitte MCP als gemeinsames Protokoll.

![MCP in der Mitte als standardisiertes Protokoll: links KI-Anwendungen wie Chat-Oberflächen und Editoren, rechts Datenquellen und Werkzeuge wie Datenbanken, Dateiablagen, Slack und Google Maps, verbunden durch Pfeile in beide Richtungen](https://mintcdn.com/mcp/bEUxYpZqie0DsluH/images/mcp-simple-diagram.png)

_Quelle: Model Context Protocol, „What is the Model Context Protocol (MCP)?" (https://modelcontextprotocol.io/docs/getting-started/intro), CC BY 4.0, abgerufen am 09.11.2026._

- Ein Programm wird einmal per MCP angeschlossen und ist dann für jedes MCP-fähige Werkzeug nutzbar.
- Vorgestellt hat MCP das Unternehmen Anthropic am 25.11.2024 als offenen Standard. Seit Dezember 2025 gehört MCP zur Agentic AI Foundation, einem Fonds unter dem Dach der Linux Foundation; Anthropic hat das Projekt dorthin abgegeben (Quellen: [Anthropic](https://www.anthropic.com/news/model-context-protocol), [MCP-Blog](https://blog.modelcontextprotocol.io/posts/2025-12-09-mcp-joins-agentic-ai-foundation/), abgerufen am 09.11.2026).

| Wann | Was |
| ---- | --- |
| Nov. 2024 | Anthropic stellt MCP als offenen Standard vor |
| Sept. 2025 | offizielles Verzeichnis öffentlicher MCP-Server startet als Vorschau (MCP Registry) |
| Dez. 2025 | MCP geht an die Agentic AI Foundation; laut MCP-Blog rund 10.000 aktive Server, über 97 Mio. Downloads der Programmbausteine (SDKs) pro Monat und Unterstützung u. a. in ChatGPT, Claude, Cursor, Gemini, Microsoft Copilot und Visual Studio Code |

Quellen: [MCP-Blog, „Introducing the MCP Registry"](https://blog.modelcontextprotocol.io/posts/2025-09-08-mcp-registry-preview/) (08.09.2025) und [„MCP joins the Agentic AI Foundation"](https://blog.modelcontextprotocol.io/posts/2025-12-09-mcp-joins-agentic-ai-foundation/) (09.12.2025), abgerufen am 09.11.2026.
- Wichtig: Ein MCP-Server kann lesen und je nach Einrichtung auch handeln (z. B. einen Termin anlegen). Darum fragen viele Werkzeuge vor einem Zugriff nach Erlaubnis.

### Beispiel: KI liest einen Ordner über MCP

Ein KI-Assistent ist über einen Datei-MCP-Server mit genau einem Ordner verbunden, der die Nordwind-Dateien enthält. Auftrag:

```text
Lies die Reisekostenrichtlinie im Nordwind-Ordner und erstelle drei Quizfragen
mit je drei Antworten für Einsteiger. Markiere die richtige Antwort.
```

| Schritt | Was passiert |
| ------- | ------------ |
| 1 | Das Werkzeug erkennt, dass es dafür eine Datei braucht, und fragt: „Zugriff auf `nordwind-reisekosten-richtlinie.md` erlauben?" |
| 2 | Der Mensch erlaubt den Zugriff einmalig. |
| 3 | Der MCP-Server liefert den Dateiinhalt; nur dieser Ordner ist freigegeben. |
| 4 | Das Modell erzeugt drei Fragen aus der Richtlinie (Beispiel: `output/project/quiz/mcp-fallback-fragen.md`). |
| 5 | Der Mensch prüft die Fragen gegen die Richtlinie (Prüfraster, Lab 3.3), bevor sie verwendet werden. |

Statt die Richtlinie in den Chat zu kopieren, holt sich die KI den Kontext selbst – aber nur dort, wo es erlaubt ist.

## Lokale Modelle: Daten bleiben im Haus

| | KI beim Anbieter (Cloud) | lokales Modell |
| --- | --- | --- |
| Wo läuft das Modell? | im Rechenzentrum des Anbieters | auf eigenem Rechner, Server oder in der eigenen Cloud |
| Wohin gehen Eingaben? | zum Anbieter (je nach Vertrag geschützt) | bleiben in der eigenen Umgebung |
| Leistung | meist die stärksten Modelle | kleinere Modelle, für viele Aufgaben ausreichend |
| Aufwand | gering, Anmeldung genügt | eigene Hardware, Einrichtung, Pflege |

- Bezug zur Datenampel (Lab 3.1): Ein lokal betriebenes Modell kann eine Option für vertrauliche Inhalte sein – wenn Betrieb und Berechtigungen geregelt sind.
- Bekannte offene Modellfamilien sind z. B. Llama, Mistral, Gemma, Qwen oder gpt-oss; Werkzeuge wie Ollama oder LM Studio machen sie auf einem Rechner nutzbar (Quelle: [Ollama-Modellbibliothek](https://ollama.com/library), abgerufen am 09.11.2026; Stand vor Kursbeginn prüfen).
- Die Auswahl ist groß: Die Plattform Hugging Face listet über 3,2 Millionen Modelle zum Herunterladen, vom kleinen Spezialmodell bis zum großen Sprachmodell (Quelle: [huggingface.co/models](https://huggingface.co/models), abgerufen am 09.11.2026).

So sieht ein lokales Modell im Alltag aus: Die App Ollama zeigt ein schlichtes Chatfenster; unten rechts steht das gewählte offene Modell (hier `gemma3:27b`), das komplett auf dem eigenen Rechner läuft.

![Ollama-App auf dem Mac: schlichtes Chatfenster mit Eingabefeld und Modellauswahl gemma3:27b](https://files.ollama.com/ollama-app-screenshot.png)

_Quelle: Ollama Blog, „Ollama's new app" vom 30.07.2025 (https://ollama.com/blog/new-app), abgerufen am 09.11.2026._

## Die Verbindungsschicht

Viele Modelle, viele Programme, viel Kontext: Dazwischen braucht es eine Schicht, die alles sicher zusammenführt.

```text
verbundene KI  =  Modell  +  Kontext  +  Systeme  +  Berechtigungen
```

Vier Fragen, die jede solche Lösung beantworten muss:

| # | Frage | Mögliche Antworten |
| - | ----- | ------------------ |
| 1 | Welches Modell läuft wo? | Cloud-Anbieter, eigene Cloud, lokal |
| 2 | Welches Wissen und welche Systeme sind angebunden? | Ablagen, Postfächer, Wikis, Fachsysteme |
| 3 | Wer darf was sehen und auslösen? | Berechtigungen je Person und Rolle, Freigabe von Aktionen |
| 4 | Wer betreibt und prüft das Ganze? | IT, Datenschutz, Fachbereich, Anbieter |

### Zwei Wege als Referenz

| Weg | Beispiel | Antwort auf Frage 1 |
| --- | -------- | ------------------- |
| Cloud-Lösung eines großen Anbieters | Microsoft 365 Copilot mit Konnektoren zu weiteren Datenquellen | Modell beim Anbieter, Daten im Vertragsrahmen des Anbieters |
| selbst gehostete Plattform | Nextise CIP | eigene Infrastruktur, offene Modelle |

Wie verbundene KI im Alltag aussieht, zeigt ein Beispiel aus der Microsoft-Dokumentation: Microsoft 365 Copilot beantwortet eine Frage zu Reisekosten und nennt drei Quellen – zwei aus einem angebundenen Fachsystem (ServiceNow, über einen Copilot-Konnektor) und eine Mail aus Outlook.

![Antwort von Microsoft 365 Copilot mit drei Quellenangaben: „Company Travel Policy" aus ServiceNow, eine Outlook-Mail zu einer Reisekosten-Ausnahme und eine Erstattungsrichtlinie aus ServiceNow](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/assets/images/connectors-copilot-logo.png)

_Quelle: Microsoft Learn, „Microsoft 365 Copilot connectors overview" (https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/overview-copilot-connector), abgerufen am 09.11.2026._

Nextise CIP ist eine selbst gehostete Wissensplattform von Nextise, die bestehende Ablagen und Fachsysteme anbindet, Firmenwissen über KI-Assistenten befragbar macht und offene Modelle nutzt (Quelle: [nextise.de/firmen-ki](https://nextise.de/firmen-ki), abgerufen am 09.11.2026, Stand vor Kursbeginn prüfen). Beide Wege beantworten dieselben vier Fragen unterschiedlich; welcher passt, hängt von Daten, Anforderungen und vorhandener IT ab.

> **Merksatz:** Je mehr KI verbunden ist, desto wichtiger werden Berechtigungen, Prüfung und Verantwortung aus Modul 3.

## Vertiefung

- **Lesen vs. Handeln:** Ein MCP-Server, der nur liest (Dateien), ist weniger riskant als einer, der handelt (Mails senden, Termine anlegen). Handelnde Zugänge brauchen eine Bestätigung durch den Menschen.
- **Manipulierte Inhalte:** Liest eine KI Dateien oder Webseiten, können darin versteckte Anweisungen stehen (Lab 3.3). Verbundene KI braucht deshalb klare Grenzen, was sie ohne Rückfrage tun darf.
- **Agenten:** Ein Agent (Lab 4.3) mit MCP-Zugängen kann mehrere Schritte selbst ausführen. Der Nutzen steigt, ebenso die Bedeutung von Freigaben und Protokollen.

## Fazit

- MCP verbindet KI-Werkzeuge über einen gemeinsamen Standard mit Dateien und Programmen.
- Lokale Modelle halten Daten im Haus, kosten aber Betrieb und Pflege.
- Eine Verbindungsschicht beantwortet vier Fragen: Modell, Wissen und Systeme, Berechtigungen, Betrieb.

In der Übung wird der MCP-Ablauf nachvollzogen und die eigene wertvollste Verbindung bewertet.
