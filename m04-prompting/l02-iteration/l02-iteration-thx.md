# Lab 4.2: Im Dialog verbessern

**Leitfragen:**

<details>
<summary>Wie läuft ein Gespräch, wenn eine Antwort nicht ganz passt?</summary>

Man sagt, was fehlt oder stört, statt von vorn zu beginnen. Ein KI-Chat funktioniert genauso: Der bisherige Verlauf bleibt Kontext.

</details>

<details>
<summary>Was ist schneller: neu anfangen oder gezielt nachbessern?</summary>

Meist gezielt nachbessern. Neu anfangen lohnt sich, wenn die Richtung grundsätzlich falsch ist oder der Verlauf widersprüchlich geworden ist.

</details>

<details>
<summary>Woran wird erkannt, dass ein Ergebnis gut genug ist?</summary>

Wenn es das Prüfraster aus Lab 3.3 besteht und ohne weiteren Umbau weitergegeben werden kann.

</details>

- Ein Prompt ist selten beim ersten Mal fertig; der Dialog ist Teil der Methode.
- Jede Nachbesserung nennt genau eine Störung und die gewünschte Änderung.

## Fünf Wege nachzubessern

| Weg | Beispiel |
| --- | -------- |
| korrigieren | „Der Termin ist Donnerstag, nicht Dienstag. Bitte korrigieren." |
| eingrenzen | „Kürze auf vier Sätze." / „Ton etwas lockerer, aber ohne Duzen." |
| Beispiel mitgeben | „Die Betreffzeile soll so aussehen: Re: Workshop – neuer Termin" |
| Rückfragen zulassen | „Stelle mir zuerst drei Fragen, bevor du schreibst." |
| in Schritten arbeiten | „Erst nur die Gliederung, dann den Text." |

„Rückfragen zulassen" ist in manchen Werkzeugen schon eingebaut. Der Recherche-Agent „Researcher" in Microsoft 365 Copilot stellt nach der ersten Frage Rückfragen (Schritt 3 „Clarify"); erst mit den Antworten darauf beginnt er zu arbeiten.

![Ablauf von Researcher in Microsoft 365 Copilot in sechs Schritten: Researcher öffnen, Frage stellen, Rückfragen beantworten (Clarify), arbeiten lassen, Bericht erhalten, weiterarbeiten](https://learn.microsoft.com/en-us/copilot/media/researcher-agent/researcher-agent-workflow.png)

_Quelle: Microsoft Learn, „What is Researcher Agent in Microsoft Copilot?" (https://learn.microsoft.com/en-us/copilot/manage/researcher-agent), abgerufen am 09.11.2026._

## Der Ablauf

```text
Prompt  →  Ergebnis  →  prüfen (Prüfraster, Lab 3.3)  →  eine gezielte Nachbesserung  →  …
                                   │
                                   └─ gut genug? → weitergeben (Mensch gibt frei)
```

- Der Mensch prüft jeden Zwischenstand, nicht nur das Endergebnis.
- Eine Nachbesserung pro Runde macht sichtbar, welche Änderung gewirkt hat.

> **Merksatz:** Nicht „mach es besser", sondern „ändere genau das".

## Warum der Mensch jede Runde prüft

Eine Feldstudie der Boston Consulting Group mit 758 Beratenden hat gemessen, wie GPT-4 die Arbeit verändert (veröffentlicht am 21.09.2023):

| Ergebnis | Wert |
| -------- | ---- |
| Teilnehmende mit KI, die sich bei kreativer Produktentwicklung verbessert haben | rund 90 % |
| Leistung bei dieser Aufgabe im Vergleich zur Gruppe ohne KI | rund 40 % höher |
| Leistung bei einer Geschäftsanalyse, die außerhalb der Stärken der KI lag | 23 % schlechter als ohne KI |

KI hilft bei vielen Aufgaben deutlich, bei anderen verschlechtert sie das Ergebnis – und von außen ist das nicht immer zu erkennen. Darum prüft der Mensch jeden Zwischenstand mit dem Prüfraster aus Lab 3.3 (Quelle: [BCG, „How People Can Create—and Destroy—Value with Generative AI"](https://www.bcg.com/publications/2023/how-people-create-and-destroy-value-with-gen-ai), abgerufen am 09.11.2026).

## Wann abbrechen und selbst schreiben

| Signal | Bedeutung |
| ------ | --------- |
| nach drei Runden immer noch falsche Fakten | die Information fehlt im Kontext – nachliefern oder selbst schreiben |
| jede Korrektur erzeugt einen neuen Fehler | der Verlauf ist widersprüchlich – neuen Chat mit vollständigem Prompt starten |
| der Text ist kürzer selbst geschrieben | die Aufgabe ist für KI zu klein |

## Vom guten Prompt zur Vorlage

Ein Prompt, der funktioniert hat, ist wiederverwendbar. Dafür werden die einmaligen Inhalte durch Platzhalter ersetzt:

```text
Rolle: Du bist [Rolle] bei [Firma].
Kontext: [Was die Kundin oder der Kunde fragt] – [Was dazu feststeht].
Aufgabe: Schreibe die Antwortmail.
Format: Betreffzeile mit „Re:", höchstens sechs Sätze, freundlich und verbindlich.
```

Platzhalter in eckigen Klammern enthalten keine echten Daten. So bleibt die Vorlage auch nach der Datenampel aus Lab 3.1 unbedenklich.

## Typische Fehler

| Symptom | Ursache | Lösung |
| ------- | ------- | ------ |
| Antwort wird mit jeder Runde schlechter | mehrere Änderungen auf einmal | eine Änderung pro Runde |
| „Mach es besser" ändert kaum etwas | Störung nicht benannt | konkret sagen, was stört |
| Vorlage enthält noch Kundennamen | Platzhalter vergessen | einmalige Inhalte durch `[…]` ersetzen |

## Fazit

- Nachbessern ist schneller als neu anfangen, wenn die Richtung stimmt.
- Eine Störung, eine Änderung, ein Prüfschritt pro Runde.
- Ein bewährter Prompt wird mit Platzhaltern zur Vorlage.

In der Übung wird die Variante B aus Lab 4.1 nachgebessert und als Vorlage für einen eigenen Anwendungsfall umgeschrieben.
