# Lab 4.3 – Lösung: Kontext ist alles

KI-Antworten fallen bei jedem Durchlauf etwas anders aus. Die Beispiele zeigen einen typischen Verlauf (Stand: 31.10.2026).

## Aufgabe 1: Karte 4 mit Vorlage

```text
Hier ist meine Prompt-Vorlage für eine wiederkehrende Aufgabe:

Rolle: Du bist [Rolle] bei [Firma].
Kontext: [Kunde] fragt nach [Anliegen]. Fest steht: [Fakt 1], [Fakt 2].
Offen ist: [offener Punkt oder „nichts"].
Aufgabe: Schreibe die Antwortmail auf die folgende Mail.
Format: Betreffzeile mit „Re:", Anrede „Guten Tag zusammen,", höchstens sechs
Sätze, freundlich und verbindlich, ohne Floskeln, am Ende Bitte um Bestätigung
bis [Frist]. Erfinde keine Termine oder Zusagen; schreibe „[offen]", wenn etwas fehlt.

Erstelle daraus eine wiederverwendbare Anweisung als Markdown-Datei mit den
Abschnitten: Rolle, Ziel, Regeln, Format der Antwort, Beispiel.
Stelle mir vorher zwei Rückfragen, falls etwas unklar ist.
Gib die Datei in einem Codeblock aus.
```

Prüfung vor dem Senden: nur Platzhalter, keine Namen, Zahlen oder Kundendaten.

## Aufgabe 2: Rückfragen der KI (typisch)

| Rückfrage | Antwort |
| --------- | ------- |
| „Soll die Datei für eine bestimmte Firma oder allgemein gelten?" | „Allgemein, mit Platzhalter [Firma]." |
| „Soll am Ende eine Prüfliste stehen?" | „Ja: Liste ‚Zu prüfen vor Versand'." |

## Aufgabe 3: Prüfung

Musterergebnis nach einer Nachbesserung: `output/project/beispiel-kontext-baustein.md`.

| Prüffrage | Ergebnis |
| --------- | -------- |
| Abschnitte Rolle, Ziel, Regeln, Format, Beispiel | ja |
| Regeln konkret und prüfbar | ja („höchstens sechs Sätze", „jede Frage einzeln") |
| Regel gegen erfundene Fakten | ja („erfinde keine Termine, Zahlen oder Zusagen") |
| nur Platzhalter | ja |

Prüfraster (Lab 3.3): Fakten und Quellen nicht betroffen; Ton und Zielgruppe passen; Freigabe durch die Person, die die Datei nutzt.

## Aufgabe 4: Nachbesserung (typisch)

Erster Entwurf ohne Beispiel → Nachbesserung:

```text
Ergänze den Abschnitt „Beispiel" mit einer kurzen Beispielmail und der passenden
Antwort. Verwende nur Platzhalter.
```

## Aufgabe 5: Speichern

Dateiname: `kontext-kundenmails.md`; Inhalt wie `output/project/beispiel-kontext-baustein.md`. Gespeichert als reiner Text.

## Aufgabe 6: Spickzettel

| Frage | Antwort |
| ----- | ------- |
| Dateiname | `kontext-kundenmails.md` |
| Wofür | Kundenmails mit Terminfragen beantworten |
| Wo / wie eingefügt | lokal gespeichert; zu Beginn eines Chats einfügen oder als Anweisung im Werkzeug hinterlegen |
| Erster Einsatz | nächste Terminanfrage eines Kunden – ohne personenbezogene Daten |

## Erweiterung

### SKILL.md aus der Anweisungsdatei

```markdown
---
name: kundenmails-beantworten
description: Beantwortet Kundenmails mit Termin- oder Teilnahmefragen freundlich und
  ohne erfundene Fakten. Verwenden, wenn eine Kundenmail beantwortet werden soll.
---

# Kundenmails beantworten

[Inhalt der Anweisungsdatei: Rolle, Regeln, Format, Beispiel]
```

Die `description` nennt den Auslöser („Verwenden, wenn …"); ohne ihn würde der Skill selten geladen.

### Test im neuen Chat

Eingabe: Inhalt der Datei, danach:

```text
Mail: „Können wir das Abstimmungsgespräch am Montag auf Dienstag legen?"
Was wir wissen: Dienstag 10:00 Uhr ist frei. Raum ist offen.
```

Typische Antwort:

```text
Re: Abstimmungsgespräch

Guten Tag zusammen,

gern verlegen wir das Abstimmungsgespräch auf Dienstag, 10:00 Uhr.
Den Raum bestätigen wir separat: [offen: Raum].
Eine kurze Bestätigung bis [Frist] reicht uns.

Viele Grüße
[Rolle]

Zu prüfen vor Versand:
- Dienstag, 10:00 Uhr
- Raum noch offen
```

Das Format wird ohne weitere Erklärung eingehalten; der fehlende Raum wird als „[offen]" markiert statt erfunden.
