# Lab 4.1 – Lösung: Die vier Bausteine eines guten Prompts

KI-Antworten fallen bei jedem Durchlauf etwas anders aus. Die Beispiele zeigen eine typische Antwort (Stand: 31.10.2026).

## Aufgabe 1: Variante A (knapper Prompt)

```text
Betreff: Ihre Anfrage zum Workshop

Sehr geehrte Damen und Herren,

vielen Dank für Ihre Nachricht. Gern verschieben wir den Workshop auf den
kommenden Dienstag. Selbstverständlich können auch weitere Personen teilnehmen.
Bei Fragen stehen wir Ihnen jederzeit zur Verfügung.

Mit freundlichen Grüßen
Ihr Nordwind-Team
```

## Aufgabe 2: Vollständiger Prompt

```text
Rolle: Du bist Projektleitung bei Nordwind Consulting.
Kontext: Das Projektteam der Stadtwerke Nordhafen möchte den Workshop am
Donnerstag um eine Woche verschieben und zwei weitere Personen aus dem
Netzbetrieb dazunehmen. Beides ist möglich: neuer Termin Donnerstag der
Folgewoche, gleiche Uhrzeit; die Gruppe wächst von 8 auf 10 Personen; der
Ablauf bleibt gleich, die Unterlagen werden für 10 Personen gedruckt.
Aufgabe: Schreibe die Antwortmail auf die folgende Kundenmail.
Format: Betreffzeile mit „Re:", höchstens sechs Sätze, freundlich und
verbindlich, ohne Floskeln, Gruß von der Projektleitung.

[Mail]
```

## Aufgabe 3: Variante B

```text
Re: Workshop am Donnerstag – geht das noch?

Hallo Projektteam der Stadtwerke Nordhafen,

danke für den Hinweis. Wir verschieben den Workshop gern um eine Woche auf
Donnerstag der Folgewoche, zur gleichen Uhrzeit. Die zwei zusätzlichen
Personen aus dem Netzbetrieb sind herzlich willkommen; damit sind wir 10
Teilnehmende. Am Ablauf ändert sich nichts, die Unterlagen drucken wir
für alle. Eine kurze Bestätigung reicht uns.

Viele Grüße
Projektleitung Nordwind Consulting
```

## Aufgabe 4: Vergleich

| Kriterium | Besser in | Begründung |
| --------- | --------- | ---------- |
| beantwortet beide Fragen der Mail | B | A lässt die Frage nach Ablauf und Unterlagen offen |
| enthält nur Fakten aus der Tabelle | B | A erfindet „kommenden Dienstag" |
| Länge und Form passen ohne Umbau | B | Betreff, Länge und Gruß sind vorgegeben |
| Ton passt zu einem Kunden | B | A ist floskelhaft („jederzeit zur Verfügung") |

## Aufgabe 5: Vom Modell selbst entschieden (Variante A)

| Stelle | Warum selbst entschieden |
| ------ | ------------------------ |
| „kommenden Dienstag" | kein Termin im Prompt → erfunden |
| „Sehr geehrte Damen und Herren" | keine Rolle und kein Ton vorgegeben |
| „auch weitere Personen" | ohne Zahl, weil der Kontext fehlte |
| Betreffzeile | eigene Formulierung, weil kein Format vorgegeben war |

## Erweiterung

Ohne Kontext-Baustein nennt das Modell häufig einen eigenen Termin oder bittet um Terminvorschläge. Der Unterschied zeigt: Die Fakten verhindern das Erfinden, nicht die Rolle.
