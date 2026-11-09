# Lab 4.1: Die vier Bausteine eines guten Prompts

**Leitfragen:**

<details>
<summary>Was braucht eine neue Kollegin, um einen Auftrag ohne Rückfrage richtig zu erledigen?</summary>

Wer schreibt, an wen, worum es geht, was genau entstehen soll und in welcher Form. Fehlt eines davon, rät sie – oder fragt nach.

</details>

<details>
<summary>Was passiert, wenn bei einem Auftrag nichts zur gewünschten Länge oder Form gesagt wird?</summary>

Die Form wird geraten. Ein Sprachmodell wählt dann meist Fließtext mittlerer Länge – nicht falsch, aber selten direkt verwendbar.

</details>

<details>
<summary>Lohnt es sich, eine Minute länger an der Anfrage zu schreiben?</summary>

Ja. Die Minute ersetzt meist zwei bis drei Überarbeitungsrunden.

</details>

- Ein Prompt ist eine Arbeitsanweisung an jemanden, der den Hauskontext nicht kennt.
- Vier Bausteine machen aus einem knappen Auftrag eine Anweisung, die beim ersten Versuch brauchbar ist.

## Die Ausgangsgeschichte

Ein neuer Kollege bekommt den Auftrag: _„Fass uns bitte das heutige Meeting zusammen."_

| Was er liefert | Was das Team erwartet hätte |
| -------------- | --------------------------- |
| drei Seiten Fließtext | Stichpunkte mit kurzen Erklärungen |
| chronologisch | nach Entscheidungen, offenen Punkten, nächsten Schritten |
| als Word-Datei per Mail | im gemeinsamen Teamordner |

Der Auftrag war nicht falsch, sondern unvollständig. Ein Sprachmodell scheitert aus demselben Grund: Es kennt nur, was im Prompt und im mitgegebenen Kontext steht (Lab 1.2).

## Die vier Bausteine

| Baustein | Frage | Beispiel |
| -------- | ----- | -------- |
| Rolle | Aus wessen Sicht wird geschrieben? | „als Projektleitung bei Nordwind Consulting" |
| Kontext | Was muss man wissen, um es zu lösen? | „Kunde möchte den Workshop verschieben; Verschiebung ist möglich" |
| Aufgabe | Was genau soll entstehen? | „Antwortmail an das Projektteam der Stadtwerke" |
| Format | Wie soll das Ergebnis aussehen? | „höchstens sechs Sätze, freundlich, mit Betreffzeile" |

```text
Rolle  +  Kontext  +  Aufgabe  +  Format   →   brauchbares Ergebnis beim ersten Versuch
 wer       was gilt    was entsteht  wie
```

## Vorher / Nachher

| Variante | Prompt |
| -------- | ------ |
| Vorher | „Schreib eine Antwort an den Kunden." |
| Nachher | „Du bist Projektleitung bei Nordwind Consulting. Das Projektteam der Stadtwerke Nordhafen fragt, ob der Workshop am Donnerstag um eine Woche verschoben werden kann und ob zwei weitere Personen teilnehmen dürfen. Beides ist möglich: neuer Termin Donnerstag der Folgewoche, gleiche Uhrzeit; die Gruppe wächst auf 10 Personen, der Ablauf bleibt gleich. Schreibe eine Antwortmail mit Betreffzeile, höchstens sechs Sätze, freundlich und verbindlich, ohne Floskeln." |

Der zweite Prompt ist länger. Genau das ist der Punkt: Die Fakten stehen im Prompt, also muss das Modell nichts erfinden.

> **Merksatz:** Was im Prompt nicht steht, entscheidet das Modell selbst – ohne Rückfrage.

## Typische Lücken

| Fehlt | Sichtbare Folge |
| ----- | --------------- |
| Rolle | unpassender Ton, mal zu locker, mal zu behördlich |
| Kontext | allgemeine Aussagen oder erfundene Details (Termine, Zahlen) |
| Aufgabe | Text über das Thema statt des gewünschten Ergebnisses |
| Format | zu lang, falsche Form, muss erst umgebaut werden |

So sieht die Lücke „Format" in der Praxis aus: Zwei kurze Prompts ohne Angabe zu Länge und Form, zwei lange Antworten. Das Modell hat selbst entschieden, wie viel und in welcher Form es schreibt.

![Le Chat von Mistral: auf den kurzen Prompt „Describe Wikipedia in a thoughtful way" antwortet das Modell mit mehreren langen Absätzen Fließtext](https://thumb.wikimedia.org/wikipedia/commons/thumb/8/81/Le_Chat_chatbot_example_screenshot.webp/500px-Le_Chat_chatbot_example_screenshot.webp)

_Quelle: Screenshot VulcanSphere, Public Domain, Wikimedia Commons (https://commons.wikimedia.org/wiki/File:Le_Chat_chatbot_example_screenshot.webp), abgerufen am 09.11.2026._

![ChatGPT: auf den Prompt „Write a draft of an essay about microplastics" folgt ein vollständiger Aufsatz mit Titel, Einleitung und Zwischenüberschriften](https://thumb.wikimedia.org/wikipedia/commons/thumb/8/84/ChatGPT_essay_draft.png/960px-ChatGPT_essay_draft.png)

_Quelle: Screenshot ChatGPT, Public Domain, Wikimedia Commons (https://commons.wikimedia.org/wiki/File:ChatGPT_essay_draft.png), abgerufen am 09.11.2026._

## Datenampel auch beim Prompten

- Der Kontext-Baustein verführt dazu, alles mitzugeben. Die Datenampel aus Lab 3.1 gilt trotzdem.
- Gelbe Inhalte nur ins freigegebene Werkzeug mit Unternehmenskonto, rote Inhalte nur anonymisiert.
- In der Kursübung enthält die Nordwind-Mail keine personenbezogenen Daten.

## Typische Fehler

| Symptom | Ursache | Lösung |
| ------- | ------- | ------ |
| Antwort enthält einen Termin, der nirgends steht | Fakten fehlen im Kontext | Fakten ausdrücklich in den Prompt schreiben |
| Antwort ist dreimal so lang wie gewünscht | Format fehlt | Länge in Sätzen oder Wörtern angeben |
| Ton passt nicht zum Kunden | Rolle und Ton fehlen | Rolle und Ton („freundlich, verbindlich") nennen |

## Vertiefung

Die erweiterte Fassung der vier Bausteine ist eine 6-Punkte-Checkliste: Klarheit, Kontext, Fokus, Struktur, Sprachstil, Beispiele. Die Punkte 1–3 sagen, **was** entstehen soll, die Punkte 4–6, **wie** es aussehen soll. Ein mitgegebenes Beispiel ersetzt oft drei Sätze Formatbeschreibung.

## Fazit

- Rolle, Kontext, Aufgabe, Format: vier Bausteine tragen jede Anweisung.
- Fakten gehören in den Prompt, sonst füllt das Modell die Lücke selbst.
- Die Datenampel entscheidet, welcher Kontext mitgegeben werden darf.

In der Übung wird ein knapper Prompt für eine Nordwind-Kundenmail mit den vier Bausteinen ausgebaut und verglichen.
