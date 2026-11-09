# Lab 3.1 – Lösung: Die Datenampel anwenden

## Aufgaben 1–3: Zuordnung, Begründung, Zweifelsfälle

| # | Eingabe | Farbe | Begründung |
| - | ------- | ----- | ---------- |
| 1 | veröffentlichte Pressemitteilung | grün | öffentlich |
| 2 | internes Projektbudget | gelb | intern, nur im freigegebenen Werkzeug; Zweifelsfall: enthält es Kundenkonditionen, gilt rot |
| 3 | Bewerbung mit Foto, Lebenslauf, Gehalt | rot | personenbezogen; das Foto kann besonders sensible Angaben enthalten (Art. 9 DSGVO) |
| 4 | Protokoll, Namen durch Rollen ersetzt | gelb | nicht mehr personenbezogen, aber weiterhin intern |
| 5 | Krankmeldung eines Kollegen | rot | Gesundheitsdaten, besonders sensibel (Art. 9 DSGVO) |
| 6 | öffentlicher Fachartikel | grün | öffentlich; Ergebnis nicht als eigenen Text ausgeben (Urheberrecht, Lab 3.2) |
| 7 | Präsentation „Strategie 2027" | rot | vertraulich, Geschäftsgeheimnis |
| 8 | Kundenmail mit Name, Telefon, Vertragsnummer | rot | personenbezogen und Kundendaten Dritter; anonymisiert gelb |
| 9 | interne Reisekostenrichtlinie | gelb | intern, ohne Personenbezug |
| 10 | Zugangsdaten zum Kundenportal | rot | Zugangsdaten nie eingeben, auch nicht im freigegebenen Werkzeug |

Typische Zweifelsfälle sind 2, 4 und 6. Regel bei Unsicherheit: die strengere Farbe wählen und bei der Datenschutz- oder IT-Stelle nachfragen.

## Aufgabe 4: Anonymisieren in drei Schritten

**Schritt 1 – Erkennen:** `Herr Jonas Petersen`, `Stadtwerke Nordhafen`, `Tel. 0471 555 0182`, `NH-2026-114`.

**Schritt 2 – Ersetzen:**

```text
[Ansprechperson] ([Kunde], [Telefon]) beschwert sich, dass die Lieferung
zum Vertrag [Vertragsnummer] zwei Wochen zu spät kam.
Bitte eine höfliche Antwort formulieren.
```

**Schritt 3 – Gegenprüfen:** Die Telefonnummer wird für die Antwort nicht gebraucht und wird gestrichen. Die Verspätung um zwei Wochen ist für die Aufgabe nötig und allein nicht identifizierend.

```text
[Ansprechperson] von [Kunde] beschwert sich, dass eine Lieferung zwei Wochen
zu spät kam. Bitte eine höfliche Antwort formulieren.
```

## Aufgabe 5: Farbe des anonymisierten Texts

Gelb: kein Personenbezug mehr, aber ein interner Vorgang. Eingabe nur im freigegebenen Werkzeug mit Unternehmenskonto; die echten Angaben werden erst nach der Antwort von Hand eingesetzt.

## Aufgabe 6: Spickzettel, Abschnitt 4

| Farbe | Was gehört dazu? | Was tue ich? |
| ----- | ---------------- | ------------ |
| grün | Öffentliches: Website, Pressemitteilung, veröffentlichte Artikel | in jedes Werkzeug |
| gelb | Internes ohne Personenbezug: Richtlinien, Pläne, anonymisierte Protokolle | nur freigegebenes Werkzeug mit Unternehmenskonto |
| rot | Personen, Gesundheit, Bewerbungen, Kundendaten, Strategie, Zugangsdaten | nicht eingeben; anonymisieren oder nachfragen |

## Häufige Fehler

| Fehler | Korrektur |
| ------ | --------- |
| nur den Namen gestrichen | Telefonnummer, Vertragsnummer und Firma machen die Person weiterhin erkennbar |
| „intern" mit „unbedenklich" gleichgesetzt | gelb heißt: nur im freigegebenen Werkzeug, nicht im privaten Konto |
| Zugangsdaten für eine Anleitung eingegeben | Anleitung mit Platzhaltern wie `[Benutzername]` erstellen lassen |
