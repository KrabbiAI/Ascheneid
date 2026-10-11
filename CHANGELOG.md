# Changelog

Alle Änderungen an **Ascheneid – Die Gruft des Gefallenen Wächters**, die neueste Version oben.
Die Downloads jeder Version liegen unter [Releases](https://github.com/KrabbiAI/Ascheneid/releases).
Die Texte der GitHub-Releases entstehen aus diesem Dokument (`tools/release_notes.sh <version>`).

## [0.8.3] – 2026-10-11 – Am besten mit Controller

### Neu
- **Controller-Empfehlung beim Start:** Eine eigene Tafel in der Startsequenz empfiehlt, mit Controller zu
  spielen. Ist schon einer angeschlossen oder läuft das Spiel auf dem Steam Deck, bestätigt sie ihn
  („Steam Deck erkannt – du bist bereit.“), sonst nennt sie, welche erkannt werden. Tastatur und Maus
  bleiben ausdrücklich erlaubt; jede Taste überspringt die Startsequenz wie bisher.

### Änderungen
- README, Changelog und Release-Texte beschreiben die Spielsysteme für sich, ohne andere Spiele zu nennen.

### Technik
- Der Steuerungstest prüft, dass die Tafel in der Startsequenz voll eingeblendet wird, bevor der Titel kommt.

## [0.8.2] – 2026-10-11 – Neue Versionen

### Neu
- **Updates aus dem Spiel heraus:**
  - Beim Start schaut das Spiel im Hintergrund nach, ob es eine neue Version gibt. Der Start wartet
    nie darauf.
  - Gibt es eine, fragt das Titelmenü: „Ascheneid v… ist erschienen. Jetzt herunterladen?“, mit Größe
    und **Herunterladen** oder **Später**. Ohne Zustimmung wird nichts geladen.
  - Ein **Downloadbalken** zeigt Prozent und Megabyte. Man kann währenddessen im Menü bleiben oder
    losspielen.
  - Danach steht im Menü **Neu starten und aktualisieren** (Linux und Steam Deck: **Beenden und
    aktualisieren**, damit Steam das Spiel nicht aus dem Blick verliert). Sonst wird beim Beenden
    installiert.
  - Jedes System bekommt sein eigenes Zip. Vor der Installation werden Größe und SHA-256-Prüfsumme
    mit GitHub abgeglichen und der Inhalt geprüft: ein Windows-Programm für Windows, ein Linux-Programm
    für x86_64, eine Mac-App für macOS. Ein vertauschter oder beschädigter Download wird verworfen.
  - Spielstände und Einstellungen bleiben unberührt; Dateinamen und Verknüpfungen bleiben gleich.
  - Nach „Später“ bleibt im Menü der Knopf **Update herunterladen**; gefragt wird erst beim nächsten
    Start wieder.
  - Abschalten unter *Optionen → Spiel → Nach Updates suchen* (dann keine Verbindung ins Netz).
  - Auf dem Mac muss die App in einem beschreibbaren Ordner liegen, etwa in *Programme*; sonst gibt
    es nur einen Hinweis.
- **Wichtig:** Der Updater steckt ab dieser Version im Spiel. Ältere Versionen einmal von Hand durch
  v0.8.2 ersetzen, danach geht es aus dem Spiel heraus.

### Behoben
- Inventar: Nach dem Belegen eines Platzes in der Schnellleiste hatte für einen Moment nichts den Fokus.
  Ein Controller-Druck genau dann ging verloren; jetzt bleibt der Fokus ohne Lücke auf dem Platz.

### Technik
- Neuer **Updater-Test** (37 Prüfungen): Versionen, Wahl des Zips je System, vertauschte Zips,
  Prüfsumme, Nachfrage und Balken im Titel, und das echte Austauschskript in einem Probeordner. Er
  läuft in der GitHub Action unter Linux und in einem eigenen Job auf einem Mac.
- **Windows Ende zu Ende** (`tests/updater_e2e_windows.ps1`): baut das Spiel, lässt es das neueste
  Release vom öffentlichen Repo laden, drückt im Titel den echten Knopf „Herunterladen“, installiert,
  startet neu und vergleicht die Dateien Byte für Byte mit dem Release.
- Die Action bricht ab, wenn Tag und Spielversion nicht zusammenpassen. Sonst würde der Updater
  immer wieder dieselbe Version laden.

## [0.8.1] – 2026-10-11 – Erwachen und Thron

### Neu
- **Zehn Spielstände,** je einer pro Figur. Einstellungen und Tastenbelegung
  gelten für alle.
  - **Fortsetzen** lädt den zuletzt gespielten Stand; darunter steht, wo man weitermacht
    (Platz, Stufe, Ort, Spielzeit).
  - **Spiel laden** zeigt links die Liste, rechts eine Tafel mit Ort (letztes Glutfeuer), Spielzeit,
    Durchgang (Neues Spiel+), Toden und Datum.
  - **Neues Spiel** nimmt den ersten freien Platz. Sind alle belegt, wählt man einen aus; überschrieben
    wird nur nach Nachfrage.
  - **Löschen** mit Dreieck/Y bzw. Entf, mit Nachfrage. Der Fokus steht dabei sicherheitshalber auf
    „Zurück“.
  - Ein durchgespielter Stand bietet beim Auswählen „Fortsetzen“ oder „Neues Spiel+“.
  - Der bisherige Spielstand wird beim ersten Start automatisch zu Platz 1.
- **Die Gruft des Erwachens:** Die Einführung ist jetzt ein eigener kleiner Ort.
  - Man erwacht im offenen Sarg, lernt in der Halle der Prüfung die Grundlagen, dann hebt sich ein
    Gitter zur **Siegelkammer**.
  - Tritt man auf das Siegel der Eidritter, brüllt etwas tief unten, die Gruft bebt immer stärker,
    die Glutrisse lodern auf, und **der Boden bricht ein**.
  - Man erwacht in Level 1 auf dem Schutt unter einem Lichtschacht: „Der Boden gab nach. Kein Weg
    führt zurück.“ Steht man auf, erklärt ein Hinweis das erste Glutfeuer (nur im Startgebiet, nie mitten
    in einer Zwischensequenz).
  - Ohne Einführung, mit „Einführung überspringen“ im Pausemenü und in Neues Spiel+ beginnt man direkt
    in Level 1, ohne Sturz. „Fortsetzen“ mitten in der Einführung beginnt sie in der Gruft des
    Erwachens von vorn.
- **Der Thronsaal als eigener Ort:**
  - **Klar abgetrennt:** Statt der Balkonbrüstung eine geschlossene Wand mit einem
    vergitterten Bogenfenster. Die Freitreppe führt durch ein Treppenhaus zu einem Torbogen, den die
    Nebelwand ausfüllt. Von außen gibt es keinen Blick mehr in die Arena.
  - **Eine eigene Welt:**
    - höhere Wände, keine Fackeln, nur Feuerschalen und ein großer Lichtfall auf den Thron
    - aschebedeckter Boden mit glühenden Rissen, in der Mitte das Siegel der Eidritter
    - tiefrote Banner der Eidritter; im übrigen Level hängen jetzt braune, Rot gibt es nur hier
    - sechs aschfahle Eidritter an den Wänden, ein Feld zerbrochener Klingen ums Podest, fallende Asche
  - **Stimmung:** Beim Eintreten werden die Farben blasser und härter, statt Musik weht Wind durch das
    offene Dach.
  - **Auftritt:** Der Wächter sitzt auf seinem Thron oben auf einem Podest, erwacht, brüllt und
    **springt herab** in den Kampf. Beim zweiten Versuch nur noch der Sprung.
  - **Phase 2:** Die Glutrisse im Boden und das Siegel lodern auf.
  - Der Aschewirbel öffnet sich am Ende auf dem Podest vor dem Thron.

### Änderungen
- Die kurze Säule mitten im Thronsaal ist fort: Vom Nebel bis zum Thron führt ein freier Gang.
- Der Gang durch den Nebel ist etwas länger, die Kamera steht danach schon in der Halle statt im
  Nebel.
- Level 1 hat kein Fallgitter und keine Übungspuppe mehr. In der Einführung entfällt der
  Glutfeuer-Schritt (der Hinweis kommt jetzt in Level 1), und der Schritt „Rolle“ heißt „Ausweichen“.
- Der Knopf „Neues Spiel+“ im Titelmenü ist in die Auswahl eines durchgespielten Stands gewandert.

### Behoben
- Stand die Figur beim Betreten des Nebels noch auf der untersten Stufe, schwebte und ruckelte sie
  durch den Torbogen. Jetzt steigt sie sauber herab, und die Kamera bleibt dabei hinter ihr.

### Technik
- **Parallele Tests:** `tools/run_tests.sh` startet alle Suiten gleichzeitig (der Ausweich- und
  Paradetest in neun Teilen). Der volle Durchlauf dauert lokal rund 3 statt 25 Minuten. Jede Suite
  schreibt in einen eigenen Ordner, auch für Einstellungen; die echten Dateien bleiben unberührt.
- In der GitHub Action laufen die Suiten als Matrix gleichzeitig; gebaut wird erst, wenn alle grün sind.
- Neue Tests:
  - **Spielstände** (36 Prüfungen): anlegen, laden, löschen und überschreiben mit Nachfrage, Migration,
    Neues Spiel+, Bedienung mit Controller und Tastatur, Aufbau im echten Titelbildschirm.
  - **Thronsaal** (16 Prüfungen): 8100 Sichtlinien von Balkon, Vorhof und Treppe, Kamera beim Gang
    durch den Nebel, Auftritt vom Thron, Stimmung, Phase 2.
  - Die Einführung testet jetzt auch Einsturz, Ankunft auf dem Schutt und das Überspringen; der
    Begehbarkeitstest läuft durch die Gruft des Erwachens und hinauf aufs Podest.

## [0.8.0] – 2026-10-11 – Klinge und Ring

### Neu
- **Wurfmesser:** ein Fernkampf-Werkzeug mit **endlichem Vorrat**.
  - Die ersten fünf liegen auf einem Leichnam im Gang von der Gruft zur Halle.
  - Danach gibt es Nachschub nur durch Gegner, die mit fester Wahrscheinlichkeit Messer fallen lassen:
    Knochenschleicher 40 %, Skelettritter 25 %, Skelettsoldaten und Knochenseher 15 %.
  - Hrodgar lässt sicher vier fallen.
  - Der Gurt fasst höchstens 10; Drops sammelt man im Vorbeilaufen ein.
  - **Wirkung:**
    - wenig Schaden, unterbricht den Knochenseher beim Zaubern
    - weckt nur den Gegner, den es trifft – schlafende Skelette lassen sich einzeln locken
    - deckt Scheinmauern auf, zerbricht Kisten und weckt die Gierige Truhe ohne Überraschungsbiss
  - **Zielen:** Das Messer fliegt aufs fixierte Ziel, sonst auf den nächsten Gegner (oder die nächste
    Kiste) im Blick. Der Schild bleibt in der linken Hand, Blocken und Parieren gehen weiter.
- **Schnellleiste:** vier Plätze für Schwert & Schild, Zweihänder und Wurfmesser.
  - **C** bzw. **Steuerkreuz rechts** rotiert vorwärts, **X** bzw. **Steuerkreuz links** zurück; dazu
    Mausrad und die Tasten **1–4**.
  - Leere Plätze und Messer ohne Vorrat werden übersprungen.
  - Beim Wechseln blendet die Leiste kurz im HUD ein; unten links steht, was man in der Hand hält.
- **Inventar mit Reitern und Detailtafel** (**I** bzw. **Ansicht/Create**, oder über das Pausemenü):
  - Das Spiel pausiert, der Hintergrund dunkelt weich ab.
  - **Reiter** Ausrüstung, Gegenstände und Schätze, umschalten mit L1/R1 bzw. Q/E.
  - **Ausrüstung:** Schnellleiste frei anordnen, Ringe anlegen. Mit der Maus geht das auch per Ziehen
    und Ablegen.
  - **Detailtafel:** großes Bild, Werte als Vorher → Nachher und ein Lore-Text zu jedem Gegenstand.
  - Die Gegenstandsbilder sind aus den 3D-Modellen gerendert. Unten steht eine Tastenleiste mit den
    Symbolen des benutzten Geräts.
- **Ring des Verschlungenen:** −15 % Schaden durch Treffer. Die Gierige Truhe gibt ihn einmalig statt
  ihres Glutsplitters; der Ring wird gleich angelegt.
- Neue Inschrift am Eingang der Halle: „Ein Messer weckt nur einen.“

### Änderungen
- Es gibt jetzt fünf statt sechs Glutsplitter. Flakon oder Klinge ganz auszubauen ist eine Entscheidung.
- Der Zweihänder liegt nach dem Fund in der Schnellleiste. Ältere Spielstände werden übernommen.
- Der Knochenseher holt für ein einzelnes Geschoss etwas länger aus (0,8 statt 0,55 s): besser zu lesen,
  und aus seiner Kampfdistanz lässt er sich mit einem Messer unterbrechen. Seine Salve bleibt schnell.

### Technik
- Neue Tests:
  - **Inventar** (80 Prüfungen): Bedienung mit Controller, Tastatur und Maus; Aufbau im Bild auch im
    Steam-Deck-Format; jeder Platz per Steuerkreuz erreichbar; Regeln der Leiste; Speichern.
  - **Wurfmesser:** Fund, Wurf, Zielen, alle Wirkungen, Drops, Obergrenze, kein Auffüllen beim Rasten.
- Der Ausweich- und Paradetest misst jetzt jeden Angriff zusätzlich mit Ring.

## [0.7.2] – 2026-10-11 – Der Eid des Ungebrannten

### Neu
- **Aldrics Quest:** Ser Aldric sitzt jetzt mitten im Level, oben an der Galerietreppe, mit
  Glut und Licht neben sich. Er gibt dir den **Kerkerschlüssel** und schickt dich zu Hrodgar, der
  sein Eidsiegel gestohlen hat.
  - Eine ruhige **Kamerafahrt** zeigt dir das Ziel: die Treppe hinunter zum Kerkertor, an dem du
    vorhin schon vorbeigekommen bist.
  - Das **Kerkertor** öffnet sich nur mit dem Schlüssel. Hrodgar wartet jetzt dahinter in einer
    eigenen Kammer; die alte Kammer hinter der Scheinmauer ist ein geheimes Beutelager mit Truhe.
  - Fällt Hrodgar, erscheint **„ALDRICS GEIST IST FREI“**. An Aldrics Platz bleiben nur Rüstung
    und Schild zurück.
  - Vor dem Nebel liegt ein goldenes **Rufzeichen**, das man nicht übersehen kann: Lichtschacht,
    Glut und ein leises Flüstern. Wer es ignoriert, hört einmal: „Vergiss mich nicht, Ungebrannter.“
  - **Aldric kämpft mit:** Er erhebt sich als goldener Phantomritter, folgt dir durch den Nebel und
    kämpft mit Schwert und Schild. Er weicht aus, blockt und zieht die Aufmerksamkeit des Wächters
    auf sich. Sein Lebensbalken steht im HUD. Der Wächter hat dafür rund 25 % mehr Leben.
  - Das Glutfeuer im Vorhof leuchtet heller und ist die letzte Rast vor dem Boss.
- **Controller-Unterstützung:** Xbox-, PlayStation- und Steam-Deck-Controller (dazu Switch) werden
  automatisch erkannt. Hinweise, Tutorial, Optionen und Pausemenü zeigen die passenden
  **Tastensymbole** (Kenney Input Prompts, CC0).
- **Belegung nach Soulslike-Standard:** Kreis/B kurz tippen = Dash, gedrückt halten = Sprint; Dreieck/Y
  interagiert, Quadrat/X trinkt, R1/R2 greifen an, L1 blockt, L2 pariert, R3 fixiert.
- **Pausemenü mit Steuerung:** Esc bzw. Start hält das Spiel an, der Hintergrund dunkelt weich ab
  und verschwimmt. Rechts steht die Steuerung für das Gerät, das du gerade benutzt, mit eigener
  Tastenbelegung oder den Symbolen deines Controllers.
- **Linux und Steam Deck:** Neuer Download `Ascheneid-Linux.zip`. Auf dem Steam Deck startet das
  Spiel im Vollbild mit einer Grafikstufe für den Akku (60 Bilder pro Sekunde, FSR).

### Behoben
- **Nach einem Dash blieb die Figur in der Laufpose hängen.** Angriffe und der erhobene Schild waren
  danach nicht mehr zu sehen, und es wirkte, als könne man nicht mehr kämpfen. Ursache: Der Dash
  spielt eine Laufschleife als einmalige Aktion ab, und eine Schleife endet nie von selbst. Jetzt
  wird jede Aktion nach ihrer Zeit ausdrücklich beendet. Dasselbe betraf den Gang durch den Nebel.
- **Sprungangriffe trafen nie:** Der Sprungschlag der Skelettsoldaten, Hrodgars Sprung und der Satz
  der Gierigen Truhe kamen aus ihrer eigenen Mindestentfernung nicht an. Ausfallschritte setzen jetzt
  sofort ein und reichen genau so weit wie nötig.
- **Die Stoßwelle des Knochensehers** verfehlte, weil er schon vor dem Knall zurücksprang. Jetzt
  springt er danach.
- **Ausgewichene Geschosse** fliegen jetzt durch dich hindurch, statt an dir zu zerplatzen.

### Technik
- **Neuer Test „Ausweichen und Parieren“:** Gegen jeden Angriff jedes Gegners (Soldat, Schleicher,
  Ritter, Seher, Übungswächter, Hrodgar in beiden Phasen, der Wächter in beiden Phasen, die Gierige
  Truhe) wird über echte Eingaben gedasht und pariert. Geprüft wird, dass der Angriff ohne Reaktion
  trifft, der Dash ausweicht, parierbare Angriffe pariert werden und rote nicht. Danach darf keine
  Animation hängen bleiben, und Angriff und Block müssen sichtbar sein. Der Test hätte den Dash-Fehler
  gefunden.
- Weitere neue Tests: Aldrics Quest, Bot-Durchlauf mit Aldric, Controller und Pausemenü.
- Die README verrät das Ende nicht mehr. Der Boss-Clip zeigt einen echten Kampf mit Aldric.

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

