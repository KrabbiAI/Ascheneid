# Changelog

Alle Änderungen an **Ascheneid – Die Gruft des Gefallenen Wächters**, die neueste Version oben.
Die Downloads jeder Version liegen unter [Releases](https://github.com/KrabbiAI/Ascheneid/releases).
Die Texte der GitHub-Releases entstehen aus diesem Dokument (`tools/release_notes.sh <version>`).

## [0.7.1] – 2026-10-11 – Unter der Haube

### Neu
- **Neue Projektseite:** Die README ist jetzt eine Werbeseite mit Titelbild, Download-Knöpfen,
  Spielszenen als Clips und einer Galerie.
- **Changelog:** Alle Versionen stehen jetzt gesammelt in `CHANGELOG.md`.

### Technik
- **Spielfigur aufgeräumt:** `player.gd` ist von 1250 auf 870 Zeilen geschrumpft. Kamera, Effekte,
  Zielsuche und Angriffstabellen sind jetzt eigene Bausteine. Spielerisch ändert sich nichts.
- **Bot-Durchlauf:** Ein automatischer Spieler spielt bei jedem Build die ganze Demo durch, von der
  Gruft bis ins Portal: mit allen Gegnern, Ausweichen, Riposten, Heilen, Glutfeuern und Bosskampf.
  Dafür nutzt er dieselben Eingabewege wie ein Mensch.
- **Clip-Werkzeug:** `tools/trailer_capture` inszeniert Spielszenen und nimmt sie mit Godots Movie
  Maker bei fester Bildrate auf.

## [0.7.0] – 2026-10-10 – Der Grabschänder

### Neu
- **Hrodgar, der Grabschänder:** ein optionaler Mini-Boss hinter einer dritten Scheinmauer an der
  Abkürzung. Er schwor einst, die Toten zu hüten, und begann dann, sie zu plündern.
  - Er sitzt auf seiner Beute und erhebt sich brüllend, wenn man näher kommt.
  - Er kämpft mit zwei Äxten: Doppelhieb, Axtstoß, Tritt und ein roter Sprungschlag.
  - Bei halber Kraft gerät er in Raserei, mit rotem Wirbel und einer Dreierkette.
  - Er hat eigene Kampfmusik und hinterlässt einen Glutsplitter.
- **Neuer Knochenseher:** Das Skelett mit den grünen Kugeln ist jetzt ein Skelettmagier mit Spitzhut
  und Stab. Die Geschosse kommen aus der Stabspitze.
- **Tod mit Gewicht:** Die Zeit dehnt sich, die Farbe weicht aus der Welt, Asche steigt aus dem
  Körper auf, und erst dann erscheint „DU BIST GESTORBEN“.
- **Die Gierige Truhe** knurrt, schnappt und atmet jetzt mit eigenen Geräuschen.
- Die Truhe in der Knochengalerie stand mit dem Rücken zum Raum, das ist behoben.
- Die Bilanz am Ende zählt jetzt vier Geheimnisse.

## [0.6.2] – 2026-10-10 – Hall und Stein

### Änderungen
- **Kamera:** Steht man mit dem Rücken nah an einer Wand, rutscht die Kamera nicht mehr auf Kniehöhe in
  die Figur. Sie setzt höher an und blickt über den Kopf hinweg in den Raum, und die Figur wird halb
  durchsichtig statt unsichtbar.
- **Raumhall:** Der Klang passt sich der Raumgröße an. Enge Gänge klingen kurz und dumpf, große Säle
  lang und weit.
- **Schritte:** Auf Erdboden klingen die Schritte weich (Kenney, CC0), auf Stein hart.
- **Ende der Demo:** Die Chronik nach dem Abspann ist jetzt eine Bilanz mit Glutflakons, Waffe und
  gefundenen Geheimnissen („◆◆◇ 2 / 3“). Sie verrät nicht, wo die fehlenden liegen.
- **Leistung:** Auf Grafikstufe 1 nutzen die Steinoberflächen eine sparsamere Variante, Stufe 0 lässt
  sie ganz weg (rund 30 % weniger GPU-Last). Ruckelt es auf einem älteren Laptop oder Mac:
  Optionen → Grafik → Stufe 0.

## [0.6.1] – 2026-10-10 – Glut verstehen

### Änderungen
- **Glutsplitter im HUD:** Unten links neben dem Flakon zeigt ein glühendes Symbol, wie viele
  ungenutzte Splitter du trägst. Bei einem Fund leuchtet es auf. Es verschwindet, sobald alle
  eingeschmolzen sind.
- **Erklärt, wenn es zählt:** Beim ersten Splitter erklärt eine Hinweiskarte, was man damit tut. Bei
  der ersten Rast mit Splittern führt das Glutfeuer-Menü direkt zu „Glut einschmelzen“, und eine
  Zeile im Menü erklärt die Wahl jedes Mal. Beide Hinweise erscheinen nur einmal, auch nicht erneut
  in Neues Spiel+.

## [0.6.0] – 2026-10-10 – Was die Mauern verbergen

### Neu
- **Scheinmauern:** Zwei Wände der Gruft sind nicht, was sie scheinen. Ein Schlag lässt sie zu Asche
  zerfallen und gibt eine *Verborgene Kapelle* und eine *Vergessene Nische* frei. Ein ganz leichter
  Glutschimmer verrät sie, wenn man genau hinsieht.
- **Die Gierige Truhe:** Eine Mimik lauert im Ossarium. Wer sie öffnen will, wird gebissen. Wer sie
  vorher schlägt, kämpft fair. Ihr Biss lässt sich parieren, der rote Sprungbiss nicht. Sie
  hinterlässt einen Glutsplitter.
- **Glut einschmelzen:** Glutsplitter (jetzt fünf im Spiel) setzt du am Glutfeuer ein: entweder
  **Flakon nähren** (ein Glutflakon mehr) oder **Klinge härten** (ausgerüstete Waffe bis +3, je Stufe
  +15 % Schaden). Ser Aldric weiß mehr darüber.
- **Steinoberflächen:** Wände, Böden, Säulen und Treppen tragen echte Steinstrukturen (Poly Haven, CC0)
  mit Relief, Rauheit, Verfärbungen und Schmutz am Wandfuß. Die KayKit-Farben bleiben erhalten.
- **Licht und Nebel:** Mondlicht fällt in sichtbaren Lichtschächten mit Staub und Schlieren durch das
  Gewölbe. In jedem Gebiet liegt Bodennebel in eigener Farbe. Beides läuft auf jeder Grafikstufe.

## [0.5.4] – 2026-10-10 – Der Aschenschritt

### Änderungen
- **Ausweichen ist jetzt ein echter Dash:** explosiver Antritt, der schnell abbremst, der Körper lehnt
  sich in die Bewegung, und leuchtende Nachbilder bleiben in der Spur stehen. Dazu kommen ein kurzer
  Sichtfeld-Ruck, Staub und ein Zischen. Solange die Unverwundbarkeit hält, schimmert der Charakter
  bläulich, so ist das Ausweich-Zeitfenster sichtbar.
- Distanz und Unverwundbarkeit bleiben fair: ca. 4,3 m in 0,46 s, unverwundbar von 0,02 bis 0,34 s.

## [0.5.3] – 2026-10-10 – Die Erzählung

### Änderungen
- **Intro-Sequenz:** Ein neues Spiel beginnt mit einer erzählten Cinematic im Souls-Stil – die Ritter des
  Eides am großen Feuer, der Wächter vor seinem Thron, das Erlöschen der Glut, die Grabkammer …
  *„Erhebe dich, Ungebrannter.“* (Halten einer Taste überspringt.) Musik: „Fantasy Choir 3“ (CC0).
- **Ladebildschirm:** Die Hinweise bleiben jetzt lange genug stehen, um sie zu lesen.
- **Durchgang Galerie → Vorhof** war durch einen Kistenstapel versperrt – behoben. Ein neuer
  Begehbarkeitstest läuft durch alle Wege der Welt.

## [0.5.2] – 2026-10-10 – Freie Sicht

### Änderungen
- **Treppe zur Knochengalerie begehbar:** Die Treppe hat jetzt unten einen Absatz und wird von unten
  betreten. Vorher kam man nur von der Seite heran, wo die Stufen schon über einen Meter hoch waren.
- **Freie Sicht auf den Gegner:** Steht deine Figur zwischen Kamera und einem nahen Gegner, wird sie
  halb durchsichtig – seine Augen, der Paradeblitz und die Ausholbewegung bleiben sichtbar.
- Aus v0.5.1: Paradeblitz 0,45 s vor dem Treffer, Paradefenster 0,3 s.

## [0.5.1] – 2026-10-10 – Lesbare Paraden

### Änderungen
- **Paraden sind jetzt fair lesbar:** Die Augen der Gegner glühen rund eine Sekunde vor dem Treffer
  langsam auf. 0,45 s vor dem Treffer blitzt ein heller Stern auf, begleitet von einem metallischen
  Klingen – das Zeichen zum Parieren. Rot blitzt es bei Angriffen, die sich nicht parieren lassen:
  dann ausweichen.
- **Paradefenster** von 0,22 s auf 0,3 s verlängert – wer auf den Blitz reagiert, liegt im Fenster.
- Der „JETZT“-Hinweis im Tutorial kommt im selben Moment wie der Blitz.

## [0.5] – 2026-10-10 – Der Riss im Schleier

### Neu
- **Ein Finale, das hängen bleibt:** Nach dem Sieg sammelt sich die Asche des Wächters zu einem
  Wirbel. Wer hineintritt, wird in einer Zwischensequenz hineingezogen – Weißblitz, Stille, dann
  Abspann, „Chronik deiner Reise“ und ein kryptischer Teaser … *Die Glut kehrt zurück.*
- **Boss-Auftritt:** Kamerafahrt, der Wächter erwacht aus der Starre, Titelkarte mit Beinamen.
  Bei halber Kraft: Zeitlupe, auflodernde Feuerschalen, härtere Musik.
- **Ser Aldric:** ein sterbender Ritter am Glutfeuer des Vorhofs, der in Rätseln spricht.
- **Neue Kampftechniken:** Rückenstich, Sturzangriff von der Galerie, zweite Waffe
  „Klinge des Eidbrechers“ (Zweihänder mit unerschütterlichem Wirbelschlag – aber ohne Parade).
- **Neues Spiel+:** Figur behalten, Welt von vorn, stärkere Gegner, mehr Seelen. Der Titelbildschirm
  erinnert sich an deinen Durchgang.
- **Atmosphäre:** echte Orchestermusik (CC0), Gegner zerfallen zu Asche, zerbrechliche Fässer und
  Kisten, Blutspuren, Kinobalken in Zwischensequenzen.
- **Komfort:** frei belegbare Tasten (Optionen → Steuerung), farbige Gamepad-Tasten in der Einführung.
- **Technik:** Builds entstehen künftig automatisch per GitHub Action bei jedem Versions-Tag;
  Tests schreiben nicht mehr in den echten Spielstand.

## [0.4] – 2026-10-10 – Die Einführung

### Neu
- **Geführte Einführung** in der Kammer des Erwachens und der Halle der Prüfung: Bewegung, Kamera,
  Sprinten, Rolle, Fixieren, leichter/schwerer Angriff, Blocken, Parieren mit „JETZT“-Hinweis,
  kritischer Stoß, Glutflakon und ein erster Kampf. Tastenhinweise passen sich an Tastatur oder
  Gamepad an. Überspringbar; im Tutorial stirbt man nicht.
- **Kampfgefühl:** höchstens zwei Gegner greifen gleichzeitig an (der Rest lauert), Rückstoß bei
  Treffern, Gamepad-Vibration, aufblinkende Ausdauerleiste, Fixieren nur mit Sichtlinie und
  automatischer Zielwechsel, wenn ein Gegner fällt.
- **Optik:** flackernde Fackeln, Randlicht an Figuren, Filmkorn (abschaltbar), verstreute Gebeine,
  neue Modelle (Särge, Grabsteine, Übungspuppe), goldgerahmte HUD-Leisten.
- Erstmals auch ein **macOS-Build**.

