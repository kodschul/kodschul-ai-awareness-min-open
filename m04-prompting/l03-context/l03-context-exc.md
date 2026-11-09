# Lab 4.3 – Übung: Kontext ist alles

**Ändert den KI-Spickzettel?** Ja — Abschnitt 8 „Mein Kontext-Baustein"

## Ausgangslage

Die Prompt-Vorlage aus Lab 4.2 funktioniert, muss aber jedes Mal neu eingefügt und erklärt werden. Daraus soll eine wiederverwendbare Anweisungsdatei werden – geschrieben von der KI, geprüft vom Menschen.

Bereitgestellt in `output/project/`:

- `beispiel-prompts.md` — Karte 4 mit dem Auftrag an die KI
- `ki-spickzettel.md` bzw. `ki-spickzettel.docx` — Abschnitt 7 (Prompt-Vorlage) und Abschnitt 8 (Kontext-Baustein)

Benötigt: ein KI-Chat und ein Texteditor (Editor, TextEdit im Modus „Reiner Text" oder vergleichbar).

## Aufgaben

1. Kopiere die Prompt-Vorlage aus Abschnitt 7 des Spickzettels in Karte 4. Prüfe vorher: nur Platzhalter `[…]`, keine echten Daten.
2. Sende Karte 4 in einem neuen Chat und beantworte die zwei Rückfragen der KI.
3. Prüfe die erzeugte Anweisungsdatei mit dem Prüfraster aus Lab 3.3 und zusätzlich mit diesen Fragen:

| Prüffrage | ja / nein |
| --------- | --------- |
| Enthält die Datei die Abschnitte Rolle, Ziel, Regeln, Format, Beispiel? | |
| Sind die Regeln konkret und prüfbar (z. B. „höchstens sechs Sätze")? | |
| Steht eine Regel gegen erfundene Fakten darin? | |
| Enthält die Datei nur Platzhalter, keine echten Daten? | |

4. Bessere jeden „nein"-Punkt mit einer gezielten Nachbesserung im Chat nach (Lab 4.2).
5. Kopiere den Inhalt des Codeblocks in einen Texteditor und speichere ihn als `.md`-Datei mit sprechendem Namen, z. B. `kontext-kundenmails.md`.
6. Fülle Abschnitt 8 des Spickzettels aus.

## Checkpoint

- Eine `.md`-Datei mit den Abschnitten Rolle, Ziel, Regeln, Format, Beispiel liegt lokal gespeichert vor.
- Alle vier Prüffragen sind mit „ja" beantwortet.

## Abschlusskriterien

- Die eigene `.md`-Datei ist gespeichert und enthält keine echten Daten.
- Abschnitt 8 „Mein Kontext-Baustein" ist ausgefüllt.

## Erweiterung

- Teste die Datei: Öffne einen neuen Chat, füge zuerst die Datei ein und danach einen erfundenen Fall mit Werten für die Platzhalter. Das Ergebnis hält das festgelegte Format ein.
- Bitte die KI, aus der Anweisungsdatei einen Skill zu machen: eine `SKILL.md` mit Kopfbereich (`name`, `description`) wie im Beispiel der Theorie. Prüfe, ob die `description` sagt, wann der Skill gilt.

## Fallback

Ohne Zugang zu einem KI-Chat: Schreibe die Anweisungsdatei selbst nach dem Muster in `output/project/beispiel-kontext-baustein.md` und speichere sie. Einschränkung: Der Schritt „KI schreibt die Anweisung" wird nur am Beispiel nachvollzogen.
