# Lab 2.1: KI-Werkzeuge und ihre Unterschiede

**Leitfragen:**

<details>
<summary>Welche KI-Werkzeuge sind im eigenen Umfeld schon bekannt oder im Einsatz?</summary>

Meist KI-Chats wie ChatGPT oder Microsoft Copilot, Übersetzer wie DeepL und KI-Funktionen in bekannten Programmen. Viele nutzen KI, ohne sie als eigenes Werkzeug wahrzunehmen.

</details>

<details>
<summary>Macht es einen Unterschied, ob ein Text in einem privaten oder einem dienstlichen Konto eingegeben wird?</summary>

Ja. Beim Unternehmenskonto gelten vertragliche Zusagen des Anbieters gegenüber dem Arbeitgeber; beim privaten Konto gelten die allgemeinen Nutzungsbedingungen. Was das für Daten heißt, folgt in Lab 3.1.

</details>

<details>
<summary>Woran wird bei Software sonst entschieden, ob sie zur Aufgabe passt?</summary>

An Aufgabe, Datenzugriff, Sicherheit, Anbieter und Bedienbarkeit – bei KI-Werkzeugen gelten dieselben Kriterien.

</details>

- Es gibt nicht „das beste KI-Werkzeug", sondern das passende für eine Aufgabe.
- Fünf Kriterien machen Werkzeuge vergleichbar.

## Die Landkarte der KI-Werkzeuge

| Werkzeugart | Beispiele | Typische Aufgabe |
| ----------- | --------- | ---------------- |
| Chat-Assistent | ChatGPT, Microsoft Copilot, Claude, Gemini, Le Chat | fragen, schreiben, zusammenfassen, erklären |
| in Arbeitsprogramme eingebaute KI | Microsoft 365 Copilot, KI in Mail- und Schreibprogrammen | direkt im Dokument, in der Mail, in der Besprechung arbeiten |
| Recherche mit Quellenangaben | Perplexity, Chat-Assistenten mit Websuche | aktuelle Fragen mit Belegen beantworten |
| Übersetzung | DeepL | Texte in andere Sprachen übertragen |
| Bild und Video | Bildgeneratoren, Videowerkzeuge | Bilder, Grafiken, kurze Videos aus einer Beschreibung |
| Transkription | Funktionen in Meeting- und Diktierprogrammen | gesprochene Sprache in Text umwandeln |

Viele Werkzeuge decken mehrere Arten ab; die Grenzen verschwimmen. Werkzeugnamen sind Beispiele, keine Empfehlung. Stand: 09.11.2026, vor Kursbeginn prüfen.

Anbieter der bekannten Chat-Assistenten: ChatGPT (OpenAI, USA), Microsoft Copilot (Microsoft, USA), Claude (Anthropic, USA), Gemini (Google, USA), Le Chat (Mistral AI, Frankreich). Oberflächen ändern sich oft; die Bilder zeigen den Stand, der in der Quellenzeile steht.

**Chat-Assistent, Beispiel ChatGPT:** ein Eingabefeld, darüber Vorschläge für typische Aufgaben. Claude, Gemini und Le Chat sind nach demselben Prinzip aufgebaut.

![ChatGPT-Startseite im Browser: Eingabefeld „Message ChatGPT“, darüber vier Beispielaufgaben, oben die Modellauswahl](https://thumb.wikimedia.org/wikipedia/commons/thumb/a/a2/Chatgpt-screenshot.png/1280px-Chatgpt-screenshot.png)
_Quelle: Wikimedia Commons, „Chatgpt-screenshot.png“ (https://commons.wikimedia.org/wiki/File:Chatgpt-screenshot.png), Public Domain, Ansicht Mai 2024, abgerufen am 09.11.2026._

**In Arbeitsprogramme eingebaute KI, Beispiel Microsoft 365 Copilot:** Die KI steckt in Edge, Outlook, Teams, Word, Excel, PowerPoint und OneNote. Im Hintergrund arbeiten ein Sprachmodell (LLM) und bei Bedarf die Websuche Bing; Protokolle bleiben im Microsoft-365-Bereich des Unternehmens.

![Architekturbild Microsoft 365 Copilot: Nutzende arbeiten in Edge, Outlook, Teams, Word, Excel, PowerPoint und OneNote; Microsoft 365 Copilot nutzt ein Sprachmodell über Azure OpenAI und die Bing-Suche und protokolliert im eigenen Microsoft-365-Mandanten, alles innerhalb der Microsoft 365 service boundary](https://learn.microsoft.com/en-us/copilot/media/copilot/copilot-chat-architecture-800.png)
_Quelle: Microsoft Learn, „Microsoft Copilot Chat Privacy and Protections“ (https://learn.microsoft.com/en-us/copilot/privacy-and-protections), © Microsoft, Stand 18.08.2026, abgerufen am 09.11.2026._

**Recherche mit Quellenangaben, Beispiel Perplexity:** Oben stehen die gefundenen Quellen, die Antwort darunter verweist mit kleinen Nummern auf sie.

![Perplexity beantwortet die Frage „What is Vilnius?“: oben drei Quellen-Kacheln, darunter die Antwort mit nummerierten Quellenverweisen, rechts Bilder](https://thumb.wikimedia.org/wikipedia/commons/thumb/6/6d/Screenshot_of_Perplexity_-_What_is_Vilnius_%282024%29.png/1280px-Screenshot_of_Perplexity_-_What_is_Vilnius_%282024%29.png)
_Quelle: Wikimedia Commons, „Screenshot of Perplexity - What is Vilnius (2024).png“ (https://commons.wikimedia.org/wiki/File:Screenshot_of_Perplexity_-_What_is_Vilnius_(2024).png), Public Domain, Ansicht Juli 2024, abgerufen am 09.11.2026._

**Übersetzung, Beispiel DeepL:** links der Ausgangstext, rechts die Übersetzung; die Sprache wird automatisch erkannt.

![DeepL Translator: links ein englischer Fachtext mit erkannter Sprache „English (detected)“, rechts die deutsche Übersetzung](https://thumb.wikimedia.org/wikipedia/commons/thumb/7/79/DeepL_machine_translation_of_English_Wikipedia_%28to_German%29.png/960px-DeepL_machine_translation_of_English_Wikipedia_%28to_German%29.png)
_Quelle: Wikimedia Commons, „DeepL machine translation of English Wikipedia (to German).png“ (https://commons.wikimedia.org/wiki/File:DeepL_machine_translation_of_English_Wikipedia_(to_German).png), CC0, Ansicht Juni 2024, abgerufen am 09.11.2026._

## Fünf Kriterien für den Vergleich

| Kriterium | Prüffrage |
| --------- | --------- |
| Datenbasis | Antwortet das Werkzeug nur aus dem Training, sucht es im Web oder kann es eigene Dateien nutzen? |
| Konto | Privat oder über ein Unternehmenskonto des Arbeitgebers? |
| Umgang mit Eingaben | Werden Eingaben gespeichert oder zum Training genutzt – und lässt sich das abschalten? |
| Anbieter und Speicherort | Wer betreibt das Werkzeug, wo werden die Daten verarbeitet? |
| Typische Stärken | Wofür ist das Werkzeug gebaut – Text, Recherche, Übersetzung, Bilder? |

> **Merksatz:** Im Beruf zuerst das Werkzeug nutzen, das der Arbeitgeber freigegeben hat – dann erst nach Stärken auswählen.

## Vertiefung

**Steckbriefe der Werkzeugarten**

| Werkzeugart | Stärke | Grenze | Typischer Einsatz im Beruf |
| ----------- | ------ | ------ | -------------------------- |
| Chat-Assistent | vielseitig, versteht Rückfragen | ohne Websuche kein aktuelles Wissen | Entwürfe, Zusammenfassungen, Ideen |
| eingebaute KI | kennt das offene Dokument oder die Mail | an ein Programm und meist eine Lizenz gebunden | Mail beantworten, Protokoll zusammenfassen |
| Recherche mit Quellen | zeigt Belege, aktuell | Quellen können falsch wiedergegeben sein | Marktüberblick, Faktencheck vorbereiten |
| Übersetzung | sehr gute Sprachqualität | Fachbegriffe und Ton prüfen | Kundenmail auf Englisch |
| Bild und Video | schnelle Visualisierung | Urheber- und Kennzeichnungsfragen (Lab 3.2) | Skizze für eine Präsentation |
| Transkription | spart Mitschrift | Fehler bei Namen und Fachbegriffen | Besprechungsnotizen |

**Kriterien mit Prüffragen für die Praxis**

- Datenbasis: Zeigt das Werkzeug an, woher eine Antwort stammt?
- Konto: Ist die Anmeldung mit dem dienstlichen Konto sichtbar?
- Umgang mit Eingaben: Wo in den Einstellungen steht, ob Eingaben zum Training genutzt werden?
- Anbieter und Speicherort: Gibt es Angaben zu Rechenzentren in der EU?
- Stärken: Liefert ein Test mit einer typischen eigenen Aufgabe ein brauchbares Ergebnis?

## Fazit

- Sechs Werkzeugarten, viele Überschneidungen – die Aufgabe bestimmt die Wahl.
- Datenbasis, Konto, Umgang mit Eingaben, Anbieter und Stärken machen Werkzeuge vergleichbar.
- Im Beruf gilt zuerst die Freigabe des Arbeitgebers.

In der Übung wird dieselbe Aufgabe in zwei Werkzeugen gelöst und nach drei Kriterien verglichen.
