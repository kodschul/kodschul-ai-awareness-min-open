# Lab 1.1: Was ist Künstliche Intelligenz?

**Leitfragen:**

<details>
<summary>Wo begegnet im eigenen Tag eine Maschine, die scheinbar „mitdenkt"?</summary>

Oft unbemerkt: im Spamfilter, in der Navigation, bei Übersetzungen, Film- und Produktempfehlungen oder beim Entsperren des Smartphones per Gesicht.

</details>

<details>
<summary>Ist ein Taschenrechner intelligent – und warum nicht?</summary>

Nein. Er führt fest programmierte Rechenregeln aus und lernt nichts dazu. KI dagegen leitet ihr Verhalten aus Beispielen ab und kann mit Unbekanntem umgehen.

</details>

<details>
<summary>Was hat sich geändert, dass seit wenigen Jahren alle über KI sprechen?</summary>

Seit Ende 2022 kann jede Person ohne Vorkenntnisse in normaler Sprache mit KI schreiben. Dahinter stehen riesige Datenmengen, starke Rechner und eine neue Modellarchitektur (2017).

</details>

- KI ist kein neues Thema, aber seit 2022 für alle direkt nutzbar.
- KI steckt schon lange in vielen Alltagsgeräten – meist unsichtbar.

## Begriffe

| Begriff | Bedeutung |
| ------- | --------- |
| Künstliche Intelligenz (KI, englisch AI) | Sammelbegriff für Systeme, die Aufgaben lösen, für die bisher menschliche Intelligenz nötig war: erkennen, verstehen, formulieren, entscheiden |
| Maschinelles Lernen | Das System lernt Regeln aus vielen Beispielen, statt dass ein Mensch jede Regel programmiert – wie ein Kind, das Hunde an vielen Bildern erkennt, nicht an einer Definition |
| Neuronales Netz | Rechenmodell aus vielen verknüpften Rechenschritten, lose angelehnt an Nervenzellen; die Grundlage heutiger KI |
| Deep Learning | maschinelles Lernen mit großen, vielschichtigen neuronalen Netzen; darauf bauen heutige Sprachmodelle und generative KI auf |
| Generative KI | KI, die neue Inhalte erzeugt: Texte, Bilder, Audio, Video, Code |
| Schwache KI | KI für eine bestimmte Aufgabe (z. B. Übersetzen) – alle heutigen Systeme |
| Allgemeine KI | hypothetische KI, die jede geistige Aufgabe wie ein Mensch lösen kann; existiert bisher nicht |

So sieht ein neuronales Netz schematisch aus: Eingaben laufen über versteckte Schichten zur Ausgabe. Jede Verbindung trägt eine einstellbare Zahl; beim Lernen werden diese Zahlen so lange angepasst, bis die Ausgaben zu den Beispielen passen.

![Schema eines neuronalen Netzes: drei Eingabe-Knoten (rot), vier versteckte Knoten (blau) und zwei Ausgabe-Knoten (grün), jeder Knoten mit jedem Knoten der nächsten Schicht durch Pfeile verbunden](https://thumb.wikimedia.org/wikipedia/commons/thumb/e/e1/Colored_neural_network_de.svg/1280px-Colored_neural_network_de.svg.png)
_Quelle: Wikimedia Commons, „Colored neural network de.svg“ (https://commons.wikimedia.org/wiki/File:Colored_neural_network_de.svg), Erik Streb, CC BY-SA 3.0, abgerufen am 09.11.2026._

## KI auf einen Blick

**Das Problem:** Viele Aufgaben lassen sich nicht in feste Regeln fassen. Niemand kann aufschreiben, woran genau eine Katze auf einem Foto zu erkennen ist oder wie eine freundliche Antwort klingt. Menschen lernen das aus Erfahrung – KI ebenfalls, nur aus Daten.

**Das Bild:** Klassische Software ist ein Kochrezept: Schritt für Schritt festgelegt. KI ist eher eine erfahrene Köchin: Sie hat tausende Gerichte gesehen und leitet daraus ab, was zusammenpasst.

Die Ebenen stecken ineinander:

![Drei ineinanderliegende Kreise: außen Artificial Intelligence (Künstliche Intelligenz), darin Machine Learning (maschinelles Lernen), innen Deep Learning](https://thumb.wikimedia.org/wikipedia/commons/thumb/1/1b/AI_hierarchy.svg/1280px-AI_hierarchy.svg.png)
_Quelle: Wikimedia Commons, „AI hierarchy.svg“ (https://commons.wikimedia.org/wiki/File:AI_hierarchy.svg), Lollixzc, CC BY-SA 4.0, abgerufen am 09.11.2026._

- **Künstliche Intelligenz** (äußerer Kreis): z. B. Schachcomputer, Routenplanung
- **Maschinelles Lernen** (mittlerer Kreis): z. B. Spamfilter, Empfehlungen
- **Deep Learning** (innerer Kreis): Lernen mit großen neuronalen Netzen
- **Generative KI** baut auf Deep Learning auf: z. B. KI-Chat, Bildgenerator

### Kurze Geschichte

| Jahr | Ereignis | Bedeutung |
| ---- | -------- | --------- |
| 1950 | Alan Turing veröffentlicht „Computing Machinery and Intelligence" (Turing-Test) | Frage: Kann eine Maschine denken? |
| 1956 | Dartmouth-Konferenz prägt den Begriff „Artificial Intelligence" | Start der KI-Forschung |
| 1970er–80er | regelbasierte Expertensysteme | Fachwissen als Wenn-dann-Regeln; aufwendig, starr |
| 1997 | Schachcomputer Deep Blue schlägt Weltmeister Kasparow | KI gewinnt in einer eng begrenzten Aufgabe |
| 2012 | tiefes neuronales Netz („AlexNet") gewinnt einen Bilderkennungswettbewerb deutlich | Durchbruch des maschinellen Lernens mit vielen Daten und Grafikprozessoren |
| 2017 | Google-Forschende stellen die Transformer-Architektur vor („Attention Is All You Need") | Grundlage aller heutigen Sprachmodelle |
| 30.11.2022 | OpenAI veröffentlicht ChatGPT | KI per Chat für alle nutzbar |

_Quellen: Turing, A. M.: Computing Machinery and Intelligence, Mind 59 (1950); McCarthy et al.: Dartmouth Proposal (1955); Vaswani et al.: Attention Is All You Need (https://arxiv.org/abs/1706.03762); OpenAI: Introducing ChatGPT (https://openai.com/index/chatgpt/), abgerufen am 31.10.2026._

**1950 – Alan Turing.** Der britische Mathematiker stellte die Frage, ob eine Maschine denken kann, und schlug dafür einen Test vor (siehe Vertiefung).

![Schwarz-Weiß-Passfoto des jungen Alan Turing, etwa 16 Jahre alt](https://thumb.wikimedia.org/wikipedia/commons/thumb/a/a1/Alan_Turing_Aged_16.jpg/500px-Alan_Turing_Aged_16.jpg)
_Quelle: Wikimedia Commons, „Alan Turing Aged 16.jpg“ (https://commons.wikimedia.org/wiki/File:Alan_Turing_Aged_16.jpg), Public Domain, abgerufen am 09.11.2026._

**1997 – Deep Blue.** Der Schachrechner von IBM gewann gegen Weltmeister Garri Kasparow. Er konnte nur Schach, sonst nichts – ein frühes Beispiel für schwache KI.

![Schwarzer Rechnerschrank von IBM Deep Blue, ausgestellt im Computer History Museum in Kalifornien](https://thumb.wikimedia.org/wikipedia/commons/thumb/e/ee/IBM_Deep_Blue_at_Computer_History_Museum_%289361685537%29.jpg/960px-IBM_Deep_Blue_at_Computer_History_Museum_%289361685537%29.jpg)
_Quelle: Wikimedia Commons, „IBM Deep Blue at Computer History Museum (9361685537).jpg“ (https://commons.wikimedia.org/wiki/File:IBM_Deep_Blue_at_Computer_History_Museum_(9361685537).jpg), Anton Chiang, CC BY 2.0, abgerufen am 09.11.2026._

**KI holt auf.** Forschende messen KI-Systeme mit standardisierten Tests und vergleichen sie mit der Leistung von Menschen. In der Grafik ist die Leistung des Menschen die Nulllinie; jede Fähigkeit startet bei −100. In der Bilderkennung erzielen KI-Systeme etwa seit 2015 mehr Punkte als Menschen, im Leseverständnis etwa seit 2018. Das gilt für den jeweiligen Test, nicht für jede Aufgabe im Alltag.

![Liniendiagramm von Our World in Data: Testergebnisse von KI-Systemen 1998 bis 2023 in Handschrift-, Sprach- und Bilderkennung, Leseverständnis, Sprachverständnis und Schlussfolgern; alle Linien starten bei minus 100 und überschreiten nach und nach die Nulllinie der menschlichen Leistung](https://ourworldindata.org/grapher/test-scores-ai-capabilities-relative-human-performance.png)
_Quelle: Our World in Data, „Test scores of AI systems on various capabilities relative to human performance“ (https://ourworldindata.org/grapher/test-scores-ai-capabilities-relative-human-performance), Daten: Kiela et al. (2023), CC BY, abgerufen am 09.11.2026._

### Wo KI heute steht

- **Im Alltag:** KI-Chats wie ChatGPT, Microsoft Copilot, Claude, Gemini oder Le Chat gehören für viele Menschen zum Alltag. Allein ChatGPT hat laut OpenAI mehr als 900 Millionen wöchentlich aktive Nutzende (Stand: 31.03.2026).
- **In Unternehmen:** Der Einsatz wächst schnell (Tabelle unten). Große Unternehmen ab 250 Beschäftigten nutzen KI deutlich häufiger (2025: 57 %) als kleine mit 10 bis 49 Beschäftigten (23 %).
- **In Europa:** 2025 nutzten 20 % der Unternehmen in der EU KI (2024: 13,5 %). Die Spanne reicht von Dänemark (42 %) bis Rumänien (5,2 %); Deutschland liegt über dem EU-Schnitt.
- **Im Recht:** Mit dem EU AI Act gibt es seit 2024 ein europäisches KI-Gesetz (Lab 3.2).

Anteil der Unternehmen in Deutschland mit mindestens zehn Beschäftigten, die KI nutzen:

| Jahr | Anteil |
| ---- | ------ |
| 2021 | 11 % |
| 2023 | 12 % |
| 2024 | 20 % |
| 2025 | 26 % |

![Eurostat-Balkendiagramm: Anteil der Unternehmen, die KI nutzen, 2024 und 2025 je EU-Land; EU 2025 bei 20 Prozent, Dänemark vorn mit 42 Prozent, Rumänien hinten mit gut 5 Prozent, Deutschland bei 26 Prozent](https://ec.europa.eu/eurostat/o/adaptive-media/image/22691519/Preview-1000x0/enterprises-using-ai-techonologies-2024-2025.jpg)
_Quelle: Eurostat, „20% of EU enterprises use AI technologies“, 11.12.2025 (https://ec.europa.eu/eurostat/web/products-eurostat-news/w/ddn-20251211-2), © Europäische Union, abgerufen am 09.11.2026._

_Quellen: OpenAI, „OpenAI raises $122 billion to accelerate the next phase of AI“, 31.03.2026 (https://openai.com/index/accelerating-the-next-phase-ai/); Statistisches Bundesamt (Destatis), Pressemitteilung Nr. 444 vom 25.11.2024 (https://www.destatis.de/DE/Presse/Pressemitteilungen/2024/11/PD24_444_52911.html) und Tabelle „Unternehmen, die künstliche Intelligenz nutzen“, Stand 24.11.2025 (https://www.destatis.de/DE/Themen/Branchen-Unternehmen/Unternehmen/IKT-in-Unternehmen-IKT-Branche/Tabellen/ikti-unternehmen-kuenstliche-intelligenz.html); Eurostat (siehe oben); alle abgerufen am 09.11.2026. Stand: 09.11.2026, vor Kursbeginn prüfen._

### KI im Alltag – oft unbemerkt

| Beispiel | Was die KI tut | Ebene |
| -------- | -------------- | ----- |
| Spamfilter | erkennt unerwünschte Mails an Mustern | maschinelles Lernen |
| Navigation | sagt Staus aus Verkehrsdaten voraus und plant Routen | maschinelles Lernen |
| Übersetzung (z. B. DeepL) | überträgt Texte in andere Sprachen | generative KI |
| Empfehlungen (Streaming, Onlinehandel) | schlägt passende Filme oder Produkte vor | maschinelles Lernen |
| Gesichtserkennung am Smartphone | erkennt das Gesicht der Besitzerin | maschinelles Lernen |
| KI-Chat, Bildgenerator | erzeugt neue Texte und Bilder | generative KI |

Ein Beispiel, das fast jede Person kennt: Der Spam-Ordner füllt sich von selbst. Niemand hat für jede dieser Mails eine Regel geschrieben; der Filter hat an Millionen Beispielen gelernt, wie unerwünschte Mails aussehen.

![Spam-Ordner in Gmail mit 15 automatisch aussortierten Werbe- und Betrugsmails, Oberfläche auf Französisch](https://thumb.wikimedia.org/wikipedia/commons/thumb/2/29/Spammed-mail-folder-2024-french.png/960px-Spammed-mail-folder-2024-french.png)
_Quelle: Wikimedia Commons, „Spammed-mail-folder-2024-french.png“ (https://commons.wikimedia.org/wiki/File:Spammed-mail-folder-2024-french.png), Dadu, CC0, Ansicht 2024, abgerufen am 09.11.2026._

### Typische Einsatzfälle im Beruf

- Texte zusammenfassen, entwerfen, umformulieren und übersetzen
- Ideen sammeln, Inhalte strukturieren, Fachbegriffe erklären lassen
- Besprechungen transkribieren und zusammenfassen
- Daten auswerten und Auffälligkeiten finden

Wofür sich KI lohnt und wofür nicht, folgt in Lab 2.2.

## Schwache und allgemeine KI

| | Schwache KI | Allgemeine KI |
| --- | --- | --- |
| Kann | eine Aufgabe oder Aufgabengruppe sehr gut | jede geistige Aufgabe wie ein Mensch |
| Beispiele | Spamfilter, Übersetzer, KI-Chat | keine – bisher nur Forschungsziel |
| Wichtig | auch ein KI-Chat, der „über alles" redet, versteht nicht wie ein Mensch | Schlagzeilen über „denkende Maschinen" beschreiben Ziele, nicht den Stand |

> **Merksatz:** Klassische Software folgt Regeln, die ein Mensch geschrieben hat. KI leitet ihre Regeln aus Beispielen ab – darum kann sie viel, aber auch überraschend danebenliegen.

## Vertiefung

- **Turing-Test:** Eine Maschine gilt als „intelligent", wenn ein Mensch im schriftlichen Gespräch nicht unterscheiden kann, ob ein Mensch oder eine Maschine antwortet. Heutige KI-Chats bestehen solche Tests oft – ein Zeichen für gute Sprachnachahmung, nicht für echtes Verstehen.
- **KI-Winter:** Nach überzogenen Erwartungen gab es zweimal (1970er und späte 1980er) Phasen mit wenig Geld und Interesse. Der heutige Aufschwung beruht auf drei Faktoren: viele Daten, starke Rechner, bessere Modelle.

## Fazit

- KI löst Aufgaben, für die bisher menschliche Intelligenz nötig war, indem sie aus Beispielen lernt.
- KI ⊃ maschinelles Lernen ⊃ Deep Learning, darauf baut generative KI auf; alle heutigen Systeme sind schwache KI.
- Neu seit 2022 ist nicht die KI selbst, sondern dass alle sie per Sprache nutzen können.

In der Übung werden acht Alltagsbeispiele den drei Ebenen zugeordnet.
