# Lab 2.2: Wofür KI sich lohnt – und wofür nicht

**Leitfragen:**

<details>
<summary>Welche Aufgabe im eigenen Alltag kostet viel Zeit, ist aber eher Routine?</summary>

Typisch: lange Mails und Dokumente lesen, Protokolle schreiben, Texte umformulieren, wiederkehrende Fragen beantworten. Genau dort entlastet KI am stärksten.

</details>

<details>
<summary>Welche Entscheidung sollte nie eine Maschine allein treffen?</summary>

Entscheidungen über Menschen (Einstellung, Kündigung, Bewertung) und rechtlich bindende Zusagen. KI darf vorbereiten, entscheiden muss ein Mensch.

</details>

<details>
<summary>Ist ein schneller, aber zu 80 % richtiger Entwurf nützlich?</summary>

Ja, wenn ein Mensch die restlichen 20 % prüft und ergänzt. Nein, wenn der Entwurf ungeprüft weitergeht oder Fehler teuer sind.

</details>

- KI spart Zeit beim ersten Entwurf und beim Verdichten, nicht beim Prüfen.
- Ob sich KI lohnt, hängt an der Aufgabe, nicht am Werkzeug.

## Sieben Nutzenmuster

| Muster | Beispiel bei Nordwind | Zeitgewinn durch |
| ------ | --------------------- | ---------------- |
| Zusammenfassen | 40-seitige Ausschreibung auf drei Kernanforderungen | Lesezeit |
| Entwerfen | erster Entwurf einer Kundenmail oder eines Berichts | Startpunkt statt leeres Blatt |
| Umformulieren | interner Text wird kundentauglich | Überarbeitungsrunden |
| Übersetzen | Kundenmail auf Englisch | Übersetzungszeit |
| Ideen sammeln | Einstieg und Übungen für einen Workshop | Kreativphase |
| Erklären lassen | Fachbegriff oder fremde Formel verständlich machen | Einarbeitung |
| Strukturieren | ungeordnete Notizen werden zur Gliederung | Sortieraufwand |

## Wofür Unternehmen KI tatsächlich einsetzen

Die amtliche Statistik zeigt, dass Unternehmen KI vor allem für Sprache und Text nutzen – genau die Nutzenmuster oben. Anteil der KI-nutzenden Unternehmen in Deutschland, die diese Technik einsetzen (2025):

| KI-Technik | Anteil |
| ---------- | ------ |
| Texte auswerten (Text Mining) | 52 % |
| Bilder, Videos, Ton erzeugen | 52 % |
| gesprochene Sprache erkennen | 42 % |
| Text erzeugen (auch Programmcode) | 35 % |
| Arbeitsabläufe automatisieren, Entscheidungen unterstützen | 27 % |
| maschinelles Lernen zur Datenanalyse | 23 % |
| Bilder erkennen | 17 % |

_Quelle: Statistisches Bundesamt (Destatis), Tabelle „Unternehmen, die künstliche Intelligenz nutzen“, Stand 24.11.2025 (https://www.destatis.de/DE/Themen/Branchen-Unternehmen/Unternehmen/IKT-in-Unternehmen-IKT-Branche/Tabellen/ikti-unternehmen-kuenstliche-intelligenz.html), abgerufen am 09.11.2026._

In der ganzen EU liegt die Textanalyse ebenfalls vorn. Die Grafik zeigt den Anteil an allen Unternehmen, nicht nur an den KI-nutzenden; darum sind die Werte kleiner.

![Eurostat-Balkendiagramm: Art der KI-Technik in EU-Unternehmen 2024 und 2025; vorn Textanalyse mit knapp 12 Prozent aller Unternehmen, dann Erzeugung von Bildern, Video und Audio sowie Erzeugung von Sprache](https://ec.europa.eu/eurostat/o/adaptive-media/image/22691503/Preview-1000x0/ai-tecnhologies-used-eu-enterprises-2024-2025.jpg)
_Quelle: Eurostat, „20% of EU enterprises use AI technologies“, 11.12.2025 (https://ec.europa.eu/eurostat/web/products-eurostat-news/w/ddn-20251211-2), © Europäische Union, abgerufen am 09.11.2026._

## Wo KI sich nicht lohnt oder nicht erlaubt ist

| Fall | Warum nicht | Was stattdessen |
| ---- | ----------- | --------------- |
| Fakten ohne Quelle | Sprachmodelle erfinden plausible Fakten (Lab 1.2) | Fakten aus der Originalquelle nehmen |
| endgültige Entscheidungen über Menschen | Verzerrungen und fehlende Verantwortung; rechtlich besonders geregelt (Lab 3.2) | KI höchstens zur Vorbereitung, Entscheidung beim Menschen |
| rechtlich bindende Aussagen | KI kennt Vertrag und Rechtslage nicht verlässlich | Fachabteilung oder Rechtsberatung |
| Aufgaben mit sehr sensiblen Daten | Eingaben gehen an einen Anbieter (Lab 3.1) | ohne KI oder nur anonymisiert |
| sehr kurze Texte | der Prompt dauert länger als das Schreiben | selbst schreiben |

## Drei Einstufungen

| Einstufung | Bedeutung | Beispiel |
| ---------- | --------- | -------- |
| geeignet | Nutzen hoch, Risiko gering, Ergebnis leicht prüfbar | Workshop-Ideen sammeln |
| mit Prüfung | Nutzen hoch, Ergebnis muss gegen eine Quelle geprüft werden | Ausschreibung zusammenfassen |
| nicht geeignet | Entscheidung über Menschen, bindende Aussage oder unzulässige Daten | Bewerbungen von der KI auswählen lassen |

> **Merksatz:** KI spart beim ersten Entwurf und beim Verdichten, nicht beim Prüfen. Der Prüfaufwand bleibt und verschiebt sich nach hinten.

## Vertiefung

Drei Stufen der Nutzung:

| Stufe | Beschreibung | Beispiel |
| ----- | ------------ | -------- |
| einzelner Prompt | einmalige Aufgabe | „Fasse dieses Protokoll zusammen" |
| besserer Prompt | dieselbe Aufgabe, gezielt gesteuert | Rolle, Format und Umfang mitgeben (Modul 4) |
| eigener Assistent | wiederkehrende Aufgabe mit fester Wissensquelle | Assistent für Reisekostenfragen (Ausblick in Lab 4.3) |

Ein wiederkehrender Anwendungsfall ist der beste Kandidat für die Stufen zwei und drei – darum wird er in der Übung notiert.

## Fazit

- Sieben Nutzenmuster: zusammenfassen, entwerfen, umformulieren, übersetzen, Ideen sammeln, erklären lassen, strukturieren.
- Nicht geeignet: Fakten ohne Quelle, Entscheidungen über Menschen, bindende Aussagen, sehr sensible Daten.
- Jeder Anwendungsfall bekommt eine Einstufung: geeignet, mit Prüfung, nicht geeignet.

In der Übung werden sechs Nordwind-Szenarien eingestuft und ein eigener Anwendungsfall notiert.
