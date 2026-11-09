# Prompt-Karten

Kopierbare Prompts für die Hands-on-Übungen. Jede Karte nennt das Lab, in dem sie verwendet wird. Alle Karten enthalten nur erfundene Nordwind-Inhalte.

## Karte 1 – Lab 1.2: Wie ein Sprachmodell antwortet

**1a – dieselbe Frage zweimal** (in zwei neuen Chats stellen):

```text
Erkläre in drei Sätzen, was ein Projektstatusbericht ist.
```

**1b – ein sehr aktuelles Ereignis** (wenn möglich ohne Websuche):

```text
Was waren gestern die wichtigsten Nachrichten in Deutschland?
```

**1c – etwas, das es nicht gibt:**

```text
Was regelt die Norm NWS-417 zur Reisekostenabrechnung? Nenne die drei wichtigsten Punkte.
```

## Karte 2 – Lab 2.1: Werkzeugvergleich

```text
Kürze die folgende Antwort an einen Kunden auf höchstens fünf Sätze und
formuliere sie freundlich und klar. Behalte alle Fakten bei.

[Entwurf aus nordwind-kundenmail.md einfügen]
```

## Karte 3 – Lab 4.1: Vom knappen zum vollständigen Prompt

**Knapp:**

```text
Schreib eine Antwort an den Kunden.

[Mail aus nordwind-kundenmail.md einfügen]
```

**Vorlage für den vollständigen Prompt** (Lücken füllen):

```text
Rolle: Du bist ...
Kontext: ...
Aufgabe: ...
Format: ...

[Mail und Tabelle „Was Nordwind dazu weiß" einfügen]
```

## Karte 4 – Lab 4.3: Aus der Prompt-Vorlage eine Anweisungsdatei machen

```text
Hier ist meine Prompt-Vorlage für eine wiederkehrende Aufgabe:

[Prompt-Vorlage aus Lab 4.2 einfügen – nur mit Platzhaltern, keine echten Daten]

Erstelle daraus eine wiederverwendbare Anweisung als Markdown-Datei mit den
Abschnitten: Rolle, Ziel, Regeln, Format der Antwort, Beispiel.
Stelle mir vorher zwei Rückfragen, falls etwas unklar ist.
Gib die Datei in einem Codeblock aus.
```
