# Design

<!-- impeccable:design-schema 1 -->

## World

**Nacht am Ballermann, aber aufgeräumt.** Tiefes Violett-Schwarz als Grundfläche,
Gold als einziges Leuchtmittel – das liest sich wie eine Clubnacht und bleibt
trotzdem ruhig genug, dass dreistellige Eurobeträge auf Anhieb erfassbar sind.

Die Welt kommt nicht aus der Kategorie „Reiseseite", sondern aus dem bestehenden
Brand Kit des Nutzers. Das war kein Zufallsfund: Near Black plus Deep Violet plus
Golden Yellow ist exakt die Lichtsituation, die der Anlass hat.

**Gegenprobe für jede Entscheidung:** Ein Mann scrollt abends auf der Couch durchs
Handy. Er soll grinsen, verstehen, was ihn etwas kostet, und antippen. In dieser
Reihenfolge.

## Mode

**Operate.** Die Besucher erledigen eine Aufgabe: drei Abstimmungen und eine Zusage.
Scanbarkeit und Zustandsklarheit schlagen Ausdruck. Der Humor sitzt in Überschriften
und Zwischentexten, **niemals in Zahlen, Labels oder Buttons** – dort gilt Klartext.

## Palette

```css
--bg:          #190926;  /* Near Black, Grundfläche */
--surface:     #21103200; /* wird als rgba aus Deep Violet gemischt */
--surface-1:   #2a1140;  /* Karten */
--surface-2:   #34134f;  /* Deep Violet, erhöhte Flächen */
--accent-deep: #4f1d78;  /* Royal Purple, Hover und Ränder */
--gold:        #ffd633;  /* Hauptakzent, gewählte Zustände, CTA */
--gold-mid:    #ffcc00;  /* Button-Kern */
--gold-soft:   #ffe066;  /* Glow, helle Akzente */
--text:        #ffffff;
--text-muted:  #b9a8c8;  /* aus dem Violett getönt, nicht grau */
--text-dim:    #8b7a9b;
```

Sekundärtext ist **aus dem Violett getönt**, nicht das Grau `#a0a0b0` aus dem Brand
Kit – auf dieser Fläche wirkt Neutralgrau schmutzig. Kontrast geprüft: `#b9a8c8`
auf `#190926` liegt über 7:1.

## Type

- **Montserrat** 700/800 für Überschriften, negatives Tracking bis -0.03em
- **Inter** 400/500/600 für Fließtext und Bedienelemente
- **Tabellenziffern** (`font-variant-numeric: tabular-nums`) überall, wo Euro steht.
  Zahlen sind hier Daten, keine Typografie-Deko.

## Components

- **Auswahlkarte** – die tragende Einheit. Große Tap-Fläche, Zustand über Goldrahmen
  plus gefüllter Marke, nie über Farbe allein. Preis pro Kopf steht **in** der Karte;
  man wählt keine Namen, sondern Konsequenzen.
- **Faktenzeile** – gesetzte Rahmenbedingungen, Icon links, kein Auswahlzustand.
- **Kostentabelle** – ausklappbar, tabellarische Ziffern, Summe hervorgehoben.
- **Ergebnisfeld** – baut den WhatsApp-Text live, mit Kopier- und WhatsApp-Knopf.
- **Beispiel-Galerie** – unter jeder Finca-Option eine horizontal scrollbare Reihe
  mit drei echten, aktuell recherchierten Anzeigen (Foto, Name, Kapazität, Preis).
  Reiner Anschauungszweck, kein Bestandteil der Abstimmung selbst – jede Kachel
  verlinkt auf die Originalanzeige. Bilder liegen lokal unter `images/fincas/`,
  weil Hotlink-Schutz vieler Vermieter direktes Einbetten sonst verhindert.

Icons sind **gezeichnete SVG** in einheitlichem Strich, keine Emoji.

## Motion

**Ein einziger authorierter Moment:** Beim Auswählen einer Karte läuft ein goldener
Lichtschein einmal über die Kartenfläche – als ginge der Scheinwerfer an. Sonst nur
kurze Zustandsübergänge. `prefers-reduced-motion` schaltet den Schein ab.

## Browser surfaces

Textmarkierung in Gold auf Dunkel, Caret gold, Scrollbar violett mit goldenem Daumen,
Fokusring gold mit Abstand. Diese Flächen gehören zur Seite, nicht zum Browser.

## Constraints

- Eine einzige `index.html`, kein Build-Schritt, kein Backend
- Mobile zuerst, Desktop ab 720px als zweite Spalte
- Auswahl in `localStorage`, damit ein Reload nichts wegwirft
- Keine personenbezogenen Daten im Markup – das Repo ist öffentlich
