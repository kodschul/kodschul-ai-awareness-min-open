# Drei-Assistenten-Kette – vorbereitete Zwischenstände

Ergebnisse der Kette aus Lab 4.3 für das Nordwind-Problem „Neue Mitarbeitende stellen immer dieselben Fragen zur Reisekostenabrechnung". Die Ausgaben sind gekürzt; die Prompts der drei Assistenten stehen in `m04-prompting/anhang-assistenten-prompts.md`.

## Eingabe an Assistent 1

```text
Neue Mitarbeitende bei Nordwind stellen jede Woche dieselben Fragen zur
Reisekostenabrechnung. Das Team Finanzen beantwortet sie einzeln per Mail.
```

## Ausgabe Assistent 1 – „Problem-Solver"

| Feld | Ergebnis |
| ---- | -------- |
| Problem | wiederkehrende Standardfragen binden das Team Finanzen; Antworten fallen unterschiedlich aus |
| Zielgruppe | ca. 5 neue Mitarbeitende pro Woche, dazu Bestandspersonal vor Dienstreisen |
| Datenquelle | interne Reisekostenrichtlinie (6 Abschnitte, ein Jahr unverändert) |
| Risiko | gering: keine personenbezogenen Daten nötig; Richtlinie muss aktuell bleiben |
| Erfolgskriterium | 80 % der Standardfragen ohne Mail an das Team Finanzen beantwortet, gemessen nach 8 Wochen |
| Empfehlung | Assistent, der ausschließlich aus der Richtlinie antwortet und die Quelle nennt |

**Entscheidung des Menschen:** Empfehlung übernommen; Gehaltsfragen und Einzelfälle ausdrücklich ausgeschlossen.

## Ausgabe Assistent 2 – „Solution Architect"

| Baustein | Inhalt |
| -------- | ------ |
| Rolle | freundliche Ansprechperson für Reisekostenfragen |
| Wissen | nur `nordwind-reisekosten-richtlinie.md` |
| Ablauf | Frage einem Abschnitt zuordnen → Regel in einem Satz → nächster Schritt → Quelle |
| Grenzen | keine Steuer- oder Rechtsberatung, keine Einzelfälle, bei Lücken an Team Finanzen verweisen |
| Test | drei Fragen: Belege Bahnfahrt, Hotel über 130 €, Frage außerhalb der Richtlinie (Gehalt) |

**Entscheidung des Menschen:** Testfrage „außerhalb der Richtlinie" ist Pflicht, weil sie zeigt, ob der Assistent erfindet.

## Ausgabe Assistent 3 – „Skill-Generator"

Ergebnis: `skills/nordwind-reisekosten/SKILL.md`.

## Vergleich mit und ohne Skill

Frage: „Welche Belege brauche ich für eine Bahnfahrt?"

| Ohne Skill | Mit Skill |
| ---------- | --------- |
| allgemeine Antwort zu Fahrkarten, Steuer und „je nach Arbeitgeber"; keine Frist, keine Quelle | Fahrkarte oder Buchungsbestätigung als PDF, Foto genügt, Abrechnung binnen 30 Tagen; Quelle: Abschnitt 4 und 5 |
