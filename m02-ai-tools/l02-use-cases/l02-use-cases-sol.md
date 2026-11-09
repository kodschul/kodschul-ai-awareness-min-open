# Lab 2.2 – Lösung: Anwendungsfälle einstufen

## Aufgabe 1–3: Einstufung der sechs Szenarien

| # | Szenario | Einstufung | Begründung |
| - | -------- | ---------- | ---------- |
| 1 | Ausschreibung verdichten | mit Prüfung | Nutzenmuster Zusammenfassen; die drei Anforderungen müssen gegen das Original geprüft werden |
| 2 | Reisekostenfragen | geeignet (mit Richtlinie als Quelle) | wiederkehrend, feste Wissensquelle, keine Personendaten – Kandidat für einen eigenen Assistenten |
| 3 | Absage an eine Bewerberin | mit Prüfung, nur ohne Personendaten | Nutzenmuster Umformulieren; Name und Gesprächsnotizen gehören nicht hinein, Entwurf mit Platzhaltern |
| 4 | Bewerbungen vorsortieren | nicht geeignet | endgültige Entscheidung über Menschen; Hochrisiko-Bereich nach EU AI Act (Lab 3.2) |
| 5 | Workshop-Ideen sammeln | geeignet | Nutzenmuster Ideen sammeln; keine internen Daten, Ergebnis leicht zu bewerten |
| 6 | Vertragsklausel bewerten | nicht geeignet | rechtlich bindende Aussage; Prüfung gehört zur Fachabteilung oder Rechtsberatung |

Szenario 3 ist bewusst ein Grenzfall: Mit Personendaten nicht geeignet, als allgemeiner Entwurf mit Platzhaltern sinnvoll.

## Aufgabe 4–5: Eigener Anwendungsfall (Beispiel)

| Aufgabe (nur mit Platzhaltern) | Einstufung | Warum? |
| ------------------------------ | ---------- | ------ |
| Kundenmails mit Terminänderungen beantworten: `[Kunde]` fragt nach Verschiebung von `[Termin]`, Antwort mit neuem `[Datum]` | mit Prüfung | wiederkehrend, Nutzenmuster Entwerfen; Termine vor dem Versand prüfen |

## Erweiterung

Szenario 4, Variante: Die KI erstellt aus der Stellenausschreibung eine Checkliste mit Kriterien; die Bewerbungen sichtet ein Mensch selbst anhand der Checkliste. Die Entscheidung bleibt beim Menschen, und keine Bewerbungsdaten gelangen in die KI.
