# Lab 3.2: KI, Ethik und Recht

**Leitfragen:**

<details>
<summary>Wenn eine Maschine aus alten Entscheidungen lernt – was passiert mit alten Fehlern und Vorurteilen?</summary>

Sie werden mitgelernt und oft verstärkt. Wurden früher bestimmte Gruppen benachteiligt, wiederholt das Modell dieses Muster, ohne dass es auffällt.

</details>

<details>
<summary>Sollte erkennbar sein, dass ein Bild oder Text von einer Maschine stammt?</summary>

Ja, wenn Menschen sonst getäuscht werden könnten. Der EU AI Act schreibt das für bestimmte Fälle vor, etwa für täuschend echte Bilder, Videos und Stimmen.

</details>

<details>
<summary>Wer ist verantwortlich, wenn eine Maschine einen falschen Rat gibt?</summary>

Der Mensch, der den Rat übernimmt und weitergibt, und das Unternehmen, das das Werkzeug einsetzt. Ein Werkzeug trägt keine Verantwortung.

</details>

- KI übernimmt Muster aus ihren Trainingsdaten – gute wie schlechte (Lab 1.2).
- Die EU regelt KI seit 2024 mit dem EU AI Act: je höher das Risiko für Menschen, desto strenger die Regeln.

## Begriffe

| Begriff | Bedeutung |
| ------- | --------- |
| Bias (Verzerrung) | systematische Schieflage in Daten oder Ergebnissen, durch die bestimmte Gruppen bevorzugt oder benachteiligt werden |
| Deepfake | mit KI erzeugtes oder verändertes Bild, Video oder Audio, das echt wirkt, z. B. eine Person sagt etwas, das sie nie gesagt hat |
| EU AI Act | Verordnung (EU) 2024/1689, das KI-Gesetz der EU; gilt in allen Mitgliedstaaten direkt |
| KI-Kompetenz | Wissen und Fähigkeiten, um KI sachkundig, sicher und verantwortungsvoll einzusetzen |

## Sechs ethische Fragen im Überblick

| Frage | Worum es geht |
| ----- | ------------- |
| Bias | Ergebnisse können Gruppen benachteiligen, weil die Trainingsdaten schief sind |
| Transparenz | Ist erkennbar, dass ein Inhalt oder ein Gesprächspartner eine KI ist? |
| Deepfakes und Manipulation | täuschend echte Fälschungen können Menschen schaden und Vertrauen zerstören |
| Urheberrecht | Wem gehören Eingaben und Ergebnisse, und dürfen fremde Werke verwendet werden? |
| Verantwortung | Wer haftet für ein falsches oder schädliches Ergebnis? |
| Arbeitswelt und Energie | Aufgaben verändern sich; Training und Nutzung großer Modelle verbrauchen viel Strom |

### Bias an einem Beispiel

Ein Unternehmen hat in den letzten zehn Jahren überwiegend Männer in technische Rollen eingestellt. Eine KI, die aus diesen Entscheidungen lernt, „merkt" sich: Bewerbungen von Männern passen besser. Sie sortiert Frauen schlechter ein – nicht aus Absicht, sondern weil die Daten es so zeigen.

### Transparenz an einem Beispiel

Ein Werbefoto zeigt eine zufriedene „Kundin". Die Person existiert nicht, das Bild ist KI-erzeugt. Ohne Hinweis entsteht der Eindruck einer echten Kundenstimme.

So realistisch wirkt ein KI-erzeugtes Gesicht: Die Frau auf dem folgenden Bild hat es nie gegeben. Ein Modell (StyleGAN) hat das Bild aus Millionen echter Fotos gelernt und neu erzeugt.

![Porträtfoto einer jungen Frau, das echt wirkt, aber vollständig von dem KI-Modell StyleGAN erzeugt wurde; die Person existiert nicht](https://thumb.wikimedia.org/wikipedia/commons/thumb/1/1f/Woman_1.jpg/500px-Woman_1.jpg)

_Quelle: Wikimedia Commons, „Woman 1.jpg“ (erzeugt mit StyleGAN, hochgeladen von Owlsmcgee, gemeinfrei) ([commons.wikimedia.org](https://commons.wikimedia.org/wiki/File:Woman_1.jpg)), abgerufen am 09.11.2026._

### Deepfakes an einem echten Fall

Anfang 2024 überwies ein Mitarbeiter des Ingenieurbüros Arup in Hongkong in 15 Überweisungen insgesamt 200 Mio. Hongkong-Dollar (rund 25,6 Mio. US-Dollar) an Betrüger. Zuvor hatte er an einer Videokonferenz mit dem vermeintlichen Finanzchef und weiteren Kollegen teilgenommen; alle Teilnehmenden waren mit KI gefälschte Bilder und Stimmen. Arup bestätigte den Fall im Mai 2024.

_Quellen: Building, „Arup named as victim of £20m deepfake scam“, 17.05.2024 ([building.co.uk](https://www.building.co.uk/news/arup-named-as-victim-of-20m-deepfake-scam/5129479.article)); AI Incident Database, Bericht 3622 (CNN, Februar 2024) ([incidentdatabase.ai](https://incidentdatabase.ai/reports/3622/)); abgerufen am 09.11.2026._

## Der EU AI Act: vier Risikoklassen

Die EU-Kommission zeigt die vier Klassen als Pyramide: oben wenige verbotene Anwendungen, unten die große Masse ohne besondere Pflichten.

![Risikopyramide des EU AI Act mit vier Stufen von oben nach unten: Unacceptable risk (rot), High risk, Limited risk (KI-Systeme mit Transparenzpflichten) und Minimal risk (türkis)](https://ec.europa.eu/information_society/newsroom/image/document/2021-17/pyramid_7F5843E5-9386-8052-931F5C4E98C6E5F2_75757.jpg)

_Quelle: Europäische Kommission, „AI Act“ (Shaping Europe’s digital future), Stand 19.10.2026 ([digital-strategy.ec.europa.eu](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)), abgerufen am 09.11.2026._

| Klasse (englisch in der Grafik) | Beispiel | Folge |
| ------------------------------- | -------- | ----- |
| verboten (unacceptable risk) | Social Scoring (Menschen nach Verhalten bewerten) | darf in der EU nicht eingesetzt werden |
| hohes Risiko (high risk) | KI in der Bewerberauswahl, Kreditvergabe | strenge Pflichten: Risikomanagement, Datenqualität, menschliche Aufsicht, Dokumentation |
| Transparenzpflicht (limited risk) | Chatbots, Deepfakes, KI-erzeugte Inhalte | Menschen müssen erkennen können, dass sie mit KI sprechen oder KI-Inhalte sehen |
| minimales Risiko (minimal risk) | Spamfilter, Rechtschreibprüfung | keine besonderen Pflichten |

### Pflicht zur KI-Kompetenz (Art. 4)

Seit dem 02.02.2025 gilt für Unternehmen, die KI einsetzen, eine Pflicht zur KI-Kompetenz ihrer Mitarbeitenden. Seit dem 27.07.2026 ist Art. 4 durch den „Digital Omnibus zur KI“ neu gefasst: Unternehmen müssen Maßnahmen ergreifen, um die KI-Kompetenz ihres Personals zu fördern – passend zu Vorwissen, Erfahrung und Einsatzzweck. Ein bestimmtes Kompetenzniveau müssen sie nicht garantieren. Eine bestimmte Prüfung oder ein Zertifikat schreibt Art. 4 nicht vor; eine Schulung mit Nachweis dient der Dokumentation.

> **Merksatz:** Je mehr eine KI über Menschen entscheidet, desto strenger die Regeln – und desto wichtiger bleibt der Mensch, der prüft.

_Quelle: Verordnung (EU) 2024/1689 (EU AI Act), Art. 4, Art. 5, Art. 50, Anhang III ([EUR-Lex](https://eur-lex.europa.eu/eli/reg/2024/1689/oj)); Art. 4 in der Fassung der Verordnung (EU) 2026/1744 ([EUR-Lex](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=OJ:L_202601744)); abgerufen am 09.11.2026._

Keine Rechtsberatung. Stand: 09.11.2026, vor Kursbeginn prüfen.

## Vertiefung

### Je ethische Frage: Beispiel und Faustregel

| Frage | Beispiel | Faustregel |
| ----- | -------- | ---------- |
| Bias | KI bewertet Bewerbungen nach alten Einstellungsmustern | Entscheidungen über Menschen nie allein der KI überlassen |
| Transparenz | KI-Chat im Kundenservice ohne Hinweis | offenlegen, wenn KI spricht oder Inhalte erzeugt hat |
| Deepfakes | gefälschte Sprachnachricht der Geschäftsführung fordert eine Überweisung | ungewöhnliche Anweisungen über einen zweiten Kanal bestätigen |
| Urheberrecht | Text, der einem veröffentlichten Artikel fast wörtlich gleicht | Ergebnisse auf auffällige Nähe zu fremden Texten prüfen; Rechtslage zu KI-Ergebnissen ist teils offen |
| Verantwortung | falsche Frist in einer KI-formulierten Kundenmail | wer weitergibt, verantwortet – unabhängig vom Werkzeug |
| Arbeitswelt und Energie | Routinetexte entstehen schneller, Prüfaufgaben werden wichtiger | KI dort einsetzen, wo sie spürbar Zeit spart; nicht für jede Kleinigkeit |

### Zeitplan des EU AI Act

| Datum | Was gilt |
| ----- | -------- |
| 01.08.2024 | Verordnung in Kraft |
| 02.02.2025 | Verbote (Art. 5) und Pflicht zur KI-Kompetenz (Art. 4) |
| 02.08.2025 | Pflichten für Anbieter großer KI-Modelle für allgemeine Zwecke |
| 27.07.2026 | „Digital Omnibus zur KI“ (Verordnung (EU) 2026/1744) in Kraft: Art. 4 neu gefasst, Hochrisiko-Fristen verschoben |
| 02.08.2026 | Transparenzpflichten (Art. 50) und der Großteil der übrigen Regeln |
| 02.12.2026 | Kennzeichnung KI-erzeugter Inhalte (Art. 50 Abs. 2) für Systeme, die schon vor dem 02.08.2026 angeboten wurden; neues Verbot von KI, die ohne Einwilligung Nacktbilder erzeugt („Nudify“-Apps) |
| 02.12.2027 | Hochrisiko-Pflichten für eigenständige Systeme (Anhang III, z. B. Bewerberauswahl) – verschoben, ursprünglich 02.08.2026 |
| 02.08.2028 | Hochrisiko-Pflichten für KI in regulierten Produkten (Anhang I, z. B. Aufzüge, Spielzeug) – verschoben, ursprünglich 02.08.2027 |

Der „Digital Omnibus zur KI“ wurde am 19.11.2025 von der EU-Kommission vorgeschlagen, am 08.07.2026 unterzeichnet, am 24.07.2026 im Amtsblatt veröffentlicht und ist seit dem 27.07.2026 in Kraft.

_Quellen: Verordnung (EU) 2026/1744 (Digital-Omnibus-Verordnung zur KI), ABl. L vom 24.07.2026, Art. 1 Nr. 5 und Nr. 40 ([EUR-Lex](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=OJ:L_202601744)); Europäische Kommission, „AI Act“, Abschnitt „Application timeline“, Stand 19.10.2026 ([digital-strategy.ec.europa.eu](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)); Europäische Kommission, „AI Omnibus enters into force“, 27.07.2026 ([digital-strategy.ec.europa.eu](https://digital-strategy.ec.europa.eu/en/news/ai-omnibus-enters-force)); alle abgerufen am 09.11.2026._

## Fazit

- Bias und fehlende Transparenz sind die häufigsten ethischen Fallen im Arbeitsalltag.
- Der EU AI Act ordnet KI nach Risiko; KI in der Bewerberauswahl gilt als hohes Risiko.
- Die Pflicht zur KI-Kompetenz gilt seit 02.02.2025 für alle Unternehmen, die KI einsetzen; seit 27.07.2026 heißt sie: Maßnahmen zur Förderung der KI-Kompetenz ergreifen.

In der Übung werden zwei Nordwind-Dilemmas nach Haltung, Risikoklasse und Bedingung bewertet.
