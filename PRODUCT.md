# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

delegated: plain static HTML/CSS/JS in einer einzigen `index.html` ohne Build-Schritt.
Begründung: Ziel ist GitHub Pages, die Seite lebt wenige Monate, und jeder Beteiligte
soll sie ohne Installation auf dem Handy öffnen können. Die Stack-Frage wurde nicht
separat gestellt – bei Widerspruch ist der Umbau billig, weil es eine Datei ist.

## Users

8–10 Männer zwischen ~35 und ~50, Freundeskreis von Lars Effenberg. Sie öffnen die
Seite **auf dem Handy, in einer WhatsApp-Gruppe**, meistens nebenbei: abends auf der
Couch, in der Pause, im Zug. Niemand liest lange. Der Job ist: in unter zwei Minuten
verstehen, worüber abgestimmt wird, eine Meinung abgeben und zurück in die Gruppe.

Sekundär: Lars selbst als Organisator. Er braucht die Zahlen belastbar genug, um
später Finca und Flüge zu buchen, und er zählt die Rückmeldungen von Hand aus.

## Product Purpose

Eine Entscheidungsgrundlage für den Männertrip nach Mallorca im September 2027.
Die Seite ersetzt die endlose WhatsApp-Diskussion durch drei klare Abstimmungen:
**Termin, Finca-Lage, Transportart.** Erfolg heißt: Nach ein paar Tagen liegen
8–10 Rückmeldungen vor, und die Buchung kann beginnen.

Kein Buchungssystem, keine Bezahlung, keine Verwaltung. Nur informieren und Meinung
einsammeln.

## Positioning

Was eine Doodle-Umfrage nicht kann: Die Seite zeigt **neben jeder Option, was sie
kostet**. Jede Abstimmungsfrage hängt direkt an einer durchgerechneten Kalkulation,
inklusive der Taxikosten, die sonst niemand auf dem Schirm hat. Man stimmt nicht über
Namen ab, sondern über Konsequenzen.

## Constraints

- **Kein Backend.** GitHub Pages liefert nur statische Dateien aus. Die Auswahl wird
  im Browser zu einem Text zusammengebaut, den der Nutzer per Knopfdruck in die
  Zwischenablage legt oder direkt an WhatsApp übergibt.
- **Öffentliches Repository.** Damit ist die Seite für jeden im Netz erreichbar.
  Deshalb: **keine Nachnamen, keine Telefonnummern, keine Adressen, keine Fotos von
  Personen.** Nur Termine, Orte, Preise. Repo-Name bewusst unauffällig: `mallorca-27`.
- **Mobil zuerst.** Desktop ist Zweitfall.
- **Preise sind Stand September 2026** und ausdrücklich Planwerte. Flüge für
  September 2027 sind noch nicht buchbar. Das muss auf der Seite sichtbar bleiben,
  damit später niemand sagt, ihm sei ein Festpreis versprochen worden.

## Brand commitments

Farben und Schriften aus dem bestehenden Brand Kit des Nutzers
(`04 Ressourcen/Grafikdesign/LE Brand Kit.md` im Obsidian-Vault):
Near Black `#190926`, Deep Violet `#34134f`, Royal Purple `#4f1d78`,
Golden Yellow `#ffd633`, Amber Gold `#ffcc00`, Soft Gold `#ffe066`.
Schriften: Montserrat für Überschriften, Inter für Fließtext.

## Voice

**Malle-Humor, ausdrücklich vom Nutzer gewählt.** Laut, derb, Ballermann-Sprech.
Grenze: Die Zahlen müssen trotzdem auf Anhieb lesbar sein – der Spaß sitzt in den
Überschriften und Zwischentexten, nicht in den Tabellen. Keine Sprüche auf Kosten
Dritter, nichts Sexistisches, nichts, was in einem öffentlichen Repo unangenehm wird.

## Facts to preserve

- Zeitraum: Donnerstag bis Sonntag, entweder **02.–05.09.2027** oder **09.–12.09.2027**
- Teilnehmer: 8–10, Kalkulation basiert auf 10
- Budget: **450 € pro Person inklusive Flug**
- Unterkunft: **Finca mit Pool ist gesetzt** (Entscheidung vom 11.09.2026)
- Transport: **ausschließlich Taxi oder Kleinbus**, kein Mietwagen
- **Ein** Partyabend am Ballermann ist geplant, nicht zwei
- **Selbstverpflegung** auf der Finca
- Abflug ab BER, Ziel PMI

## Open decisions

- Termin (Abstimmung)
- Finca-Lage: stadtnah, mittlere Lage oder Inselinneres (Abstimmung)
- Transportart: Großraumtaxi spontan oder Kleinbus mit Fahrer vorbestellt (Abstimmung)
- Endgültige Teilnehmerzahl – 8 oder 10 verschiebt den Pro-Kopf-Preis deutlich
