# Lab 3.1: Datenschutz – Was darf in ein KI-Werkzeug?

**Leitfragen:**

<details>
<summary>Welche Informationen aus dem eigenen Arbeitsalltag würden nie per Mail an Fremde gehen?</summary>

Typisch: Personalakten, Gesundheitsangaben, Gehälter, Kundendaten, Verträge, Strategiepapiere, Zugangsdaten. Genau diese Grenze gilt auch für KI-Werkzeuge.

</details>

<details>
<summary>Wer liest mit, wenn ein kostenloser Online-Dienst genutzt wird?</summary>

Der Anbieter verarbeitet jede Eingabe auf seinen Servern. Bei kostenlosen Privatkonten dürfen Eingaben oft zur Verbesserung der Modelle genutzt werden, sofern das nicht abgeschaltet ist.

</details>

<details>
<summary>Reicht es, den Namen in einem Text zu streichen?</summary>

Oft nicht. Telefonnummer, Vertragsnummer, Firma oder ein seltener Vorfall machen eine Person weiterhin erkennbar.

</details>

- Jede Eingabe in ein KI-Werkzeug ist eine Weitergabe an einen Anbieter – wie eine Mail an einen externen Dienstleister.
- Vor der Eingabe zählt nicht, wie nützlich die Antwort wäre, sondern welche Art von Information eingegeben wird.

## Begriffe

| Begriff | Bedeutung |
| ------- | --------- |
| DSGVO | Datenschutz-Grundverordnung der EU; regelt, wie personenbezogene Daten verarbeitet werden dürfen |
| Personenbezogene Daten | alle Angaben, mit denen sich eine Person direkt oder indirekt erkennen lässt: Name, Mail, Telefonnummer, Foto, Kundennummer, Lebenslauf |
| Geschäftsgeheimnis | interne Information mit wirtschaftlichem Wert, die bewusst geschützt wird, z. B. Budgets, Strategie, Angebotskalkulation |
| Kundendaten Dritter | Informationen, die ein Kunde oder Partner anvertraut hat; sie gehören nicht dem eigenen Unternehmen |
| Anonymisieren | Angaben so ändern, dass niemand mehr auf eine bestimmte Person oder Firma schließen kann |

## Wie verbreitet private KI im Job ist

Viele Beschäftigte nutzen KI-Werkzeuge mit privatem Konto auch für dienstliche Aufgaben, oft ohne Freigabe. Das nennt sich Schatten-KI (mehr dazu in Lab 3.3). Drei Erhebungen zeigen, wie verbreitet das ist:

| Erhebung | Ergebnis |
| -------- | -------- |
| Bitkom, 604 Unternehmen in Deutschland ab 20 Beschäftigten, Juli/August 2025 | 4 von 10 Unternehmen gehen zumindest davon aus, dass Beschäftigte private KI-Werkzeuge nutzen: in 8 % weit verbreitet (2024: 4 %), in 17 % Einzelfälle, 17 % vermuten es. Nur 29 % sind sicher, dass es nicht vorkommt (2024: 37 %). Regeln für den KI-Einsatz haben 23 %. |
| IW Köln, rund 5.000 Beschäftigte in Deutschland, März/April 2026 | 29,1 % der Beschäftigten, die KI beruflich nutzen, verwenden Werkzeuge, die der Arbeitgeber nicht bereitstellt. |
| Microsoft Work Trend Index, 31.000 Wissensarbeitende in 31 Ländern, Februar/März 2024 | 75 % nutzen generative KI bei der Arbeit; 78 % davon bringen eigene KI-Werkzeuge mit. |

_Quellen: Bitkom, Presseinformation „Beschäftigte nutzen vermehrt Schatten-KI“, 21.10.2025 ([bitkom.org](https://www.bitkom.org/Presse/Presseinformation/Beschaeftigte-nutzen-vermehrt-Schatten-KI)); IW-Kurzbericht Nr. 63/2026 „Schatten-KI: Beschäftigte sind schneller als ihre Betriebe“, 19.09.2026 ([iwkoeln.de](https://www.iwkoeln.de/studien/barbara-engels-andrea-hammermann-schatten-ki-beschaeftigte-sind-schneller-als-ihre-betriebe.html)); Microsoft und LinkedIn, „2024 Work Trend Index Annual Report“, 08.05.2024 ([microsoft.com](https://www.microsoft.com/en-us/worklab/work-trend-index/ai-at-work-is-here-now-comes-the-hard-part)); alle abgerufen am 09.11.2026._

## Was mit einer Eingabe passiert

```text
Eingabe im Chat ──► Server des Anbieters ──► Modell erzeugt Antwort
                         │
                         ├─ Speicherung im Chat-Verlauf
                         └─ je nach Konto: Nutzung zur Verbesserung der Modelle
```

Was beim Anbieter mit einer Eingabe geschieht, hängt vom Konto ab (siehe Lab 2.1):

| Merkmal | Privates Konto (kostenlos) | Unternehmenskonto mit Datenschutzzusage |
| ------- | -------------------------- | --------------------------------------- |
| Vertrag | Nutzungsbedingungen zwischen Anbieter und Privatperson | Vertrag zwischen Anbieter und Unternehmen, inkl. Auftragsverarbeitung |
| Nutzung der Eingaben für Training | häufig erlaubt, oft abschaltbar | in der Regel vertraglich ausgeschlossen |
| Wer verwaltet Verlauf und Löschung | die Person selbst | die IT des Unternehmens nach festen Regeln |
| Dienstlich geeignet | nein, außer für öffentliche Informationen | ja, wenn das Werkzeug freigegeben ist |

Die genauen Zusagen unterscheiden sich je Anbieter und Tarif. Stand: 09.11.2026, vor Kursbeginn prüfen.

### Beispiel Privatkonto: Training ist eine Einstellung

Bei Privatkonten entscheidet oft ein einzelner Schalter, ob Chats für das Training verwendet werden. Anthropic hat Nutzende von Claude Free, Pro und Max im August 2025 mit diesem Dialog gefragt; der Schalter „You can help improve Claude“ steht dort bereits auf „an“. Wer zustimmt, erlaubt die Nutzung der Chats für das Training, die Speicherdauer verlängert sich dann auf fünf Jahre. Die Einstellung lässt sich später in den Datenschutzeinstellungen ändern. Für Unternehmenstarife (Commercial Terms, z. B. Claude for Work) gilt diese Regel nicht.

![Dialog „Updates to Consumer Terms and Policies“ in Claude: Schalter „You can help improve Claude“ ist eingeschaltet, darunter der Hinweis auf eine Speicherdauer von 5 Jahren, Schaltflächen Accept und Not now](https://www-cdn.anthropic.com/images/4zrzovbb/website/0d48d7f71fe2b5ccc537b48394313a91636bb329-3840x2160.png)

_Quelle: Anthropic, „Updates to Consumer Terms and Privacy Policy“, 28.08.2025 ([anthropic.com](https://www.anthropic.com/news/updates-to-our-consumer-terms)), abgerufen am 09.11.2026._

Andere Werkzeuge haben vergleichbare Einstellungen, oft unter „Datenkontrollen“ oder „Datenschutz“ (siehe Vertiefung „Einstellungen je Werkzeugart“).

### Beispiel Unternehmenskonto: der Weg einer Eingabe

Microsoft zeigt für Copilot Chat mit Unternehmenskonto, wo eine Eingabe verarbeitet wird: Sie bleibt innerhalb der „Microsoft 365 service boundary“, wird für Prüfungen protokolliert (Logging, Audit) und laut Microsoft nicht zum Training der zugrunde liegenden Modelle verwendet. Nur für eine Websuche gehen einzelne Suchbegriffe ohne Personen- oder Firmenkennung an die Suchmaschine Bing.

![Architekturbild „Microsoft 365 AI-powered chat architecture“: Nutzende und Apps (Word, Excel, Outlook, Teams …) senden Eingaben an Microsoft 365 Copilot; Sprachmodell, Protokollierung und Firmendaten liegen innerhalb der Microsoft 365 service boundary, nur Suchanfragen gehen an Bing](https://learn.microsoft.com/en-us/copilot/media/copilot/copilot-chat-architecture-800.png)

_Quelle: Microsoft Learn, „Privacy and protections“ (Microsoft Copilot Chat), Stand 18.08.2026 ([learn.microsoft.com](https://learn.microsoft.com/en-us/copilot/plan/privacy-and-protections)), abgerufen am 09.11.2026. Microsoft 365 Copilot heißt inzwischen Microsoft Copilot._

## Die Datenampel

| Farbe | Art der Information | Beispiele | Regel |
| ----- | ------------------- | --------- | ----- |
| grün | öffentlich | Pressemitteilung, veröffentlichter Fachartikel, Website-Text | in jedes KI-Werkzeug |
| gelb | intern | interne Richtlinie, Projektplan, anonymisiertes Protokoll | nur ins freigegebene Werkzeug mit Unternehmenskonto |
| rot | personenbezogen, vertraulich oder fremd | Bewerbung, Krankmeldung, Kundenmail mit Kontaktdaten, Strategiepapier, Zugangsdaten | nicht eingeben – höchstens anonymisiert |

Zugangsdaten (Passwörter, PINs, Zugangsschlüssel) sind immer rot, auch anonymisiert gibt es dafür keinen sinnvollen Weg.

> **Merksatz:** Die Art der Information entscheidet, nicht die Nützlichkeit der Antwort. Im Zweifel nicht eingeben, sondern die Datenschutz- oder IT-Stelle fragen.

## Datenschutz-Check in drei Schritten

1. Farbe der geplanten Eingabe bestimmen (Tabelle oben).
2. Werkzeug und Konto prüfen: Ist es das freigegebene Werkzeug mit Unternehmenskonto?
3. Bei Rot oder Unsicherheit: anonymisieren oder nicht eingeben und nachfragen.

Eine einmal eingegebene Angabe lässt sich nicht zuverlässig zurückholen.

## Vertiefung

### Besonders sensible Daten (Art. 9 DSGVO)

Für einige Datenarten gelten strengere Regeln: Gesundheit, ethnische Herkunft, politische Meinung, religiöse Überzeugung, Gewerkschaftszugehörigkeit, genetische und biometrische Daten, Sexualleben und sexuelle Orientierung. Eine Krankmeldung oder ein Bewerbungsfoto kann solche Angaben enthalten. Diese Daten gehören nie in ein KI-Werkzeug, auch nicht ins freigegebene.

_Quelle: Verordnung (EU) 2016/679 (DSGVO), Art. 9 ([EUR-Lex](https://eur-lex.europa.eu/eli/reg/2016/679/oj)), abgerufen am 09.11.2026._

### Einstellungen je Werkzeugart

| Einstellung | Wo zu finden (typisch) | Empfehlung |
| ----------- | ---------------------- | ---------- |
| Verlauf speichern | Einstellungen → Datenkontrollen / Datenschutz | bei Privatkonten nur bei Bedarf aktiv |
| Eingaben zur Modellverbesserung nutzen | Einstellungen → Datenkontrollen | bei Privatkonten ausschalten |
| Gedächtnis-Funktion (das Werkzeug merkt sich Angaben aus früheren Gesprächen) | Einstellungen → Personalisierung | gespeicherte Inhalte regelmäßig ansehen und löschen |
| Temporärer Chat / Inkognito-Chat | beim Start eines neuen Chats | für einmalige Fragen ohne Verlauf |

Bezeichnungen und Orte ändern sich häufig und unterscheiden sich je Werkzeug. Stand: 09.11.2026, vor Kursbeginn prüfen.

### Anonymisieren in drei Schritten

1. **Erkennen:** alle Angaben markieren, die auf eine Person oder Firma schließen lassen (Name, Kontakt, Nummern, Firma, seltene Details).
2. **Ersetzen:** jede markierte Angabe durch einen Platzhalter oder eine Rolle ersetzen (`[Ansprechperson]`, `[Kunde]`, `[Vertragsnummer]`).
3. **Gegenprüfen:** den Text so lesen, als wäre er fremd – lässt sich trotzdem noch erraten, wer gemeint ist? Was für die Aufgabe nicht nötig ist, streichen.

Keine Rechtsberatung. Verbindlich sind die Regeln des eigenen Unternehmens und die Auskunft der Datenschutzstelle.

## Fazit

- Jede Eingabe ist eine Weitergabe; das Konto entscheidet mit, was der Anbieter damit tun darf.
- Datenampel: grün überall, gelb nur im freigegebenen Werkzeug, rot nicht – höchstens anonymisiert.
- Anonymisieren heißt erkennen, ersetzen, gegenprüfen; Namen streichen allein reicht selten.

In der Übung werden zehn Nordwind-Eingaben der Datenampel zugeordnet und ein roter Fall anonymisiert.
