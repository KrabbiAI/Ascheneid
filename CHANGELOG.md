# Changelog

Alle Änderungen an **Ascheneid – Die Gruft des Gefallenen Wächters**, die neueste Version oben.
Die aktuelle Version gibt es unter [Releases](https://github.com/KrabbiAI/Ascheneid/releases).

## [1.1.0] – 2026-10-17 – Das Vergessene Refugium

Der Sieg über den Wächter ist nicht mehr das Ende: Der Aschewirbel trägt dich an einen Ort zwischen den Orten.

### Neu
- **Das Vergessene Refugium:** ein verwunschener Friedhof unter Sternen und einem riesigen Blutmond. Ein
  gepflasterter Weg führt zwischen Gräbern, Gruften und toten Bäumen hindurch, Laternen glimmen im Bodennebel,
  und am Ende wartet eine Kathedrale. Hier gibt es keine Gegner, nur Stille, eine ferne Glocke und eine eigene,
  ruhige Musik.
- **Dobby, der Imp:** Du erwachst, und über dir beugt sich ein kleiner Kerl mit großen Augen – Hüter der
  Schlüssel, Bewahrer der Geheimnisse und gelegentlich zuständig für die Unkrautentfernung. Er führt dich zur
  Kathedrale, wartet, wenn du trödelst, und hat zu allem etwas zu sagen. Schlagen kannst du ihn. Er beschwert
  sich nur.
- **Das große Tor:** In der Kathedrale steht ein versiegeltes Tor mit drei leeren Fassungen. Drei Steine
  fehlen, verstreut in Welten, die längst hätten verschwinden sollen. Eine Questanzeige zeigt dir das
  aktuelle Ziel.
- **Das Portal zu den Eishöhlen:** Über einer Portalsäule schwebt ein eisblaues Portal. Berühre es, und
  du erfährst, was hinter dem Eis wartet. Die Eishöhlen selbst folgen im nächsten Kapitel.
- **Ein neues Glutfeuer** in der Kathedrale. Im Refugium kann dir nichts geschehen: Wer herunterfällt, steht
  einfach wieder auf sicherem Boden.
- **Art-Pack für die Steam-Bibliothek:** Wer Ascheneid als Nicht-Steam-Spiel auf dem Steam Deck oder am PC
  spielt, findet Capsule, Wide Capsule, Hero, Logo und Icon im Ordner `docs/media/steam`.

### Änderungen
- **Dialoge lassen sich in Ruhe lesen:** Ein Tastendruck zeigt die Zeile sofort ganz, erst der nächste
  schaltet weiter.
- **Optionen besser bedienbar:** Die gewählte Zeile leuchtet golden, Schieberegler haben einen großen, hellen
  Griff. Du siehst sofort, welcher Regler gerade aktiv ist.
- **Neues Spiel+ entfällt:** Durchgespielte Spielstände laden direkt weiter und tragen ihre Markierung ◆.
  Alte Spielstände laden ohne Fehler.

### Behoben
- Nach dem Sieg über den Wächter konnte das Spiel bei sehr niedriger Bildrate im Sog des Aschewirbels hängen
  bleiben.
- In Zwischensequenzen lief die Figur manchmal auf der Stelle, statt zu stehen.

## [1.0.0] – 2026-10-15 – Das erste Kapitel

Ascheneid 1.0: die Gruft des Gefallenen Wächters als abgeschlossenes erstes Kapitel.

### Neu
- **Das Urteil der Krone:** Der Wächter hat schon in Phase 1 einen roten Angriff. Er reißt das Kronzepter
  über den Kopf und schmettert es herab; parieren geht nicht, seitlich ausweichen schon, und danach bleibt
  ein Fenster zum Zurückschlagen. Er kommt zufällig zwischendurch und sicher, sobald man ihn zweimal in Folge
  pariert hat – wer nur pariert, muss jetzt auch ausweichen.
- **Ser Aldric erneuert seinen Eid:** Brüllt der Wächter in seine zweite Phase, antwortet Aldric, reckt das
  Schwert und schöpft einmal neue Kraft. So erlebt er den Sieg fast immer mit, samt Gruß und Abschied.

### Änderungen
- **Endkampf ausgewogener:** 1050 statt 1250 Leben, Grundschaden statt 20 % Aufschlag, und in Phase 2 ruft
  der Wächter zweimal zwei Skelette statt zweimal drei. Fordernd, aber auch für Spieler fair, die nicht
  jede Parade treffen.
- **Rote Angriffe des Wächters sind unübersehbar:** Holt er zu einem nicht parierbaren Angriff aus, glüht
  er vom ersten Moment an am ganzen Körper rot, samt Krone und Kronzepter. Das Urteil der Krone holt dabei
  länger aus (1,44 Sekunden, in Phase 2 1,22).
- **Keine Truhe mit dem Zweihänder mehr vor dem Boss:** Weitere Nahkampfwaffen kommen in einem späteren
  Kapitel. Wer den Zweihänder schon hat, behält ihn.

### Behoben
- **Einsturz der Gruft:** Statt feiner Staubkörner fielen große graue Scheiben vor die Kamera und
  verdeckten den Sturz. Jetzt rieselt feiner Staub, und der Blick auf die fallende Figur bleibt frei.
- **Der Einsturz lässt sich wieder überspringen:** Wie bei allen Zwischensequenzen genügt es, eine beliebige
  Taste gedrückt zu halten.

## [0.9.0] – 2026-10-15 – Der Gekrönte Wahn

### Neu
- **Der Endboss in neuer Gestalt – der Gekrönte Wahn:** Der Gefallene Wächter trägt eine schiefe,
  gesprungene Krone mit gebrochenem Dornenkranz, sein Brustkorb ist aufgebrochen und gibt ein
  glühendes Herz frei, und er führt das Kronzepter, einen Streitkolben mit einer Glutkugel in einer
  gebrochenen Krone. Krone, Herz und Zepterkugel pulsieren und glühen in Phase 2 heller. Fällt er,
  stürzen Krone und Zepter zu Boden, und seine Glut erlischt.
- **Ein epischer Auftritt:** Nach dem Nebel liegt der Saal im Dunkeln, die Feuerschalen entzünden
  sich nacheinander, in der Krone kehrt die Glut zurück, er hebt das Haupt, die Augen flammen auf,
  er rammt das Zepter in den Boden, und die Glutrisse lodern bis zum Spieler auf. Dann Schrei und
  Titelkarte: „Der Gefallene Wächter – Der Gekrönte Wahn“. Beim nächsten Versuch nur der Sprung.
- **Glutschild:** Während er in Phase 2 übergeht und während er Skelette beschwört, ist er kurz
  unverwundbar. Treffer prallen mit Funken an einem Glutschild ab.
- **Im Intro** zeigt sich der Wächter vor seinem Thron nur noch als schwarzer Schattenriss vor
  Gegenlicht – wer er wirklich ist, sieht man erst im Kampf.
- **Rote Angriffe heben sich deutlich ab:** Holt ein Gegner zu einem nicht parierbaren Angriff aus,
  glüht seine Waffe rot auf, statt des Sterns blitzt ein großer roter Kreuzblitz mit Ring (etwas
  früher und länger), und ein eigener, tiefer Warnklang ertönt. Parierbare Angriffe bleiben beim
  hellen Stern.
- **Einführung, neuer Schritt „Rote Angriffe“:** Der Übungswächter holt rot aus. Erklärt wird, dass
  sich rote Angriffe nicht parieren lassen und Blocken viel Kraft kostet; geschafft ist der Schritt
  mit einem Dash durch den Hieb. Zur Bewährung mischt er danach beides.
- **Gegenstände mit Bild:** Die Meldung „Gegenstand erhalten“ zeigt links das Symbol des Gegenstands
  (Glutsplitter, Zweihänder, Ring, Wurfmesser, Schlüssel, Seelen).
- Entwicklermenü hinzugefügt.

### Änderungen
- **Endboss härter:** 1250 statt 950 Leben, alle Angriffe richten ein Fünftel mehr Schaden an, und in
  Phase 2 ruft er zweimal je drei Skelette herbei (bei 40 % und bei 18 %).
- **Aldrics Kamerafahrt** ist ruhiger und professioneller: auf Augenhöhe mit Blick geradeaus statt
  auf den Boden, langsamer und gleichmäßig, mit weichem Anfang; zurück zur Figur geht es per
  Schwarzblende.
- **Am Ende der Einführung** steht die Figur genau mittig auf der Siegelplatte, wenn sie einbricht.

### Behoben
- Aldrics Rufzeichen lag halb auf der Oberkante der Freitreppe; es liegt jetzt mittig auf ebenem Boden.
- Fünf Inschriften am Boden ragten in Wände (am Fuß der Galerietreppe, im Vorhof, in der Halle, vor der
  Schatzkammer und in der Siegelkammer der Einführung). Ein Test prüft jetzt jede Leuchtfläche auf
  ebenen, freien Boden.

## [0.8.9] – 2026-10-14 – Glut und Eid

### Neu
- **Intro, neu erzählt:** Die vier am großen Feuer sind jetzt verschiedene Gestalten mit eigenen
  Farben und Silhouetten: der Rote in geschwärztem Eisen mit Helmbusch und Zweihänder, der Bronzene
  mit Hörnerhelm, Rundschild und Axt, der Magier des Eides in Silberblau mit Spitzhut, Kristallstab
  und der Rosette des Eides auf der Brust, und der Ungebrannte. Als die Glut erlischt, brechen die drei
  nacheinander zusammen und zerfallen langsam zu Asche und Glut. Nur der Ungebrannte bleibt und sinkt
  allein am letzten Glimmen nieder: „Nur einer blieb am Feuer zurück.“
- **Ausdauer zählt:**
  - Jede Aktion braucht ihre volle Ausdauer (Dash 22, leichter Schlag 16, schwerer 30, Parade 10,
    Wurfmesser 8). Kritische Stöße kosten weiterhin nichts.
  - Wer knapp zu früh drückt, verliert die Eingabe nicht: Sie greift, sobald genug nachgeflossen ist.
  - Wer die Leiste leer macht, ist kurz außer Atem: Die Erholung setzt später ein und läuft anfangs
    langsamer. Wer sich die Kraft einteilt, merkt davon nichts; endloses Dashen und Schlagen geht
    nicht mehr.
  - Zu sehen und zu hören: Die Leiste zeigt dunkel, was bis zum nächsten Dash fehlt, und zuckt
    grau-rot, wenn eine Aktion an der Ausdauer scheitert. Außer Atem steigen Atemwölkchen vom Helm,
    man hört leises Keuchen, und der Bildrand dunkelt kurz ein.
- **Alle Fässer** im Level zerbersten bei einem Hieb oder Dash, auch große Fässer, Fässchen und Stapel.
- **Glut einschmelzen** ist am Glutfeuer ein eigener Menüpunkt. Solange Splitter etwas bewirken
  können, flackert er wie Glut und sprüht Funken. Dahinter liegt ein eigener Bildschirm: Glutflakon
  und **jede eigene Waffe** (auch die, die gerade nicht in der Hand liegt) mit Stufe, Schaden vorher
  und nachher und dem Vorrat an Splittern. B/Esc führt zurück ans Feuer.
- **Unentzündete Glutfeuer** glimmen: Restglut in der Asche, ein matter Schein und aufsteigende Funken.
  Ein kaltes Feuer übersieht man im Dunkeln nicht mehr.
- **Das Ende der Einführung** ist neu inszeniert:
  - Harter Schnitt auf die Figur über dem glühenden Siegel; sie verliert den Halt.
  - Ein Glutstoß, kurze Zeitlupe: Der Boden zerspringt in taumelnde Brocken.
  - Die Kamera taucht der stürzenden Figur in den glühenden Abgrund hinterher, aus der Tiefe brüllt
    der Wächter.

### Änderungen
- **Parade ohne Starre:**
  - Während der Parade lässt sich die Figur langsam versetzen.
  - Nach einer gelungenen Parade bricht jede Aktion den Rest sofort ab (Dash, Angriff, Riposte,
    neue Parade). Das Fenster bleibt danach noch kurz offen, damit auch der Schlag eines zweiten
    Gegners abprallt.
  - Eine Fehlparade ist nach 0,42 s statt 0,6 s vorbei.
- **Schwertklang:** Jeder Hieb klingt anders. Die Tonhöhe springt jedes Mal spürbar, nie zweimal
  fast gleich, und die Kombo hat einen eigenen Rhythmus (hoch, tief). Auch Treffer an Gegnern und
  Blocks variieren, große Gegner klingen dumpfer.
- **Ser Aldric** sitzt jetzt in der Nische auf halber Strecke der Abkürzung, wo früher die Truhe stand.
  Wer die Abkürzung nicht erkundet, verpasst ihn. Der Weg zum Kerkertor führt quer durchs Ossarium,
  und die Kamerafahrt nach der Schlüsselübergabe folgt genau diesem Weg. Die Truhe steht nun am Ende
  der Abkürzung vor der Tür zur Gruft, die zwei Gegner der Abkürzung bewachen ihre Enden.
- **Knochengalerie:** Der Durchgang zum Vorhof ist doppelt so breit. Der Skelettritter wartet allein
  oben an der Treppe; der Knochenseher steht weit dahinter und erwacht erst, wenn man ihm nahe kommt,
  statt in den Ritterkampf zu schießen. Die Truhe mit dem Zweihänder steht in der Ecke hinter ihm.
- **Glutfeuer im Vorhof** steht jetzt rechts neben der Freitreppe mit Blick auf den Nebel, statt
  versteckt links dahinter.
- **Inschriften am Boden** sind größer und heller: kräftigere Schrift, ein weicher Glutschein darunter
  und ein paar aufsteigende Funken.
- **Inschriften überarbeitet:**
  - „Jenseits des Nebels …“ lag mitten in Aldrics Rufzeichen und liegt nun am Eingang des Vorhofs.
  - Am Fuß der Galerietreppe war von Säulen die Rede, die es dort nicht gibt; jetzt warnt die
    Inschrift vor dem Seher oben.
  - Am Eingang der Abkürzung deutet eine Inschrift an, dass dort jemand wartet.

### Behoben
- Oben an der Galerietreppe lag noch der Stein, in dem Aldric früher halb steckte.
- Zweihänder-Truhe und Fässer versperrten im Durchgang zum Vorhof den Weg.
- Nach dem Sturz aus der Einführung lag ein Schuttbrocken mitten auf dem Weg zum ersten Glutfeuer.

## [0.8.5] – 2026-10-11 – Feinschliff

### Neu
- **Erfolge**, gebunden an den Spielstand (ein neuer Stand beginnt ohne, Neues Spiel+ behält sie):
  - *Erwacht* (Einführung bestanden) · *Gierig, aber nicht hungrig genug* (Gierige Truhe) ·
    *Der Grabschänder fällt* (Hrodgar) · *Nichts bleibt verborgen* (alle sieben Geheimnisse: drei
    Scheinmauern und vier versteckte Truhen) · *Ein Eid, gemeinsam erfüllt* (Wächter an Aldrics Seite) ·
    *Letzter Eid der Asche* (Wächter).
  - Neue Erfolge meldet eine Karte, die unten rechts hereingleitet; mehrere kommen nacheinander.
  - Übersicht im Pausemenü unter **Erfolge** (offene mit ihrer Aufgabe, bei den Geheimnissen mit
    Zähler); die Spielstandliste zeigt die Zahl je Platz.
- **Ser Aldric** hat eine eigene Gestalt statt der Spielerfigur: ein Eidritter im zerschlissenen,
  aschgrauen Kapuzenmantel (gleicher Stil), mit Schwert und Wappenschild. Auch sein Phantom im Bosskampf.
- **Update:** Der Dialog bleibt nach „Herunterladen“ offen und zeigt den Balken; ist das Update fertig,
  steht darin direkt **Neu starten und aktualisieren** (Linux: **Beenden und aktualisieren**).
  „Im Hintergrund weiter“ schließt ihn, der Dialog meldet sich, sobald alles bereit ist. Oben rechts
  zeigt ein auffälliges Banner den Stand, und im Pausemenü gibt es einen Eintrag „Update …“.

### Änderungen
- **Aldric** sitzt jetzt in der ruhigen Nische mit der Fackel am Treppenabsatz, direkt neben dem
  Kerkertor, statt oben an der Galerietreppe zwischen Knochenseher und Skelettritter. Ein eigenes Licht
  hebt ihn vom Stein ab.
- **Nach Hrodgars Tod** löst sich Aldric sofort in Glut auf, und sein Rufzeichen liegt gleich vor dem
  Nebel – ohne Rast am Glutfeuer. Ein Hinweis sagt es: „Ein goldenes Zeichen glimmt vor dem Nebel.“
- **Schlafende Gegner** lassen sich fixieren und per Zielwechsel ansteuern. Fixieren weckt sie nicht;
  erst ein Treffer, ein Messer oder Lärm. Die getarnte Gierige Truhe bleibt unentdeckt.
- **Balancing:** Es gibt viel weniger Seelen, jede Stufe ist eine Entscheidung.
  - Stufen kosten 250 × 1,15^(Stufe−1) (vorher 100 × 1,12^…).
  - Skelettsoldat 40, Knochenschleicher 55, Knochenseher 90, Skelettritter 160 Seelen; Hrodgar 1100,
    Gierige Truhe 450, Hrodgars Hort 500.
  - Ohne Farmen reicht es bis zum Endboss für etwa sieben Stufen (vorher rund 18). Wieder erschlagene
    Gegner geben die Hälfte; eine ganze Runde Farmen bringt knapp eine Stufe.
- **Optionen:** Reiter mit **LB/RB** bzw. L1/R1 (Tastatur Q/E) wechseln; der Fokus springt mit.

### Behoben
- Im Optionsreiter **Grafik** (und Steuerung) verschwanden Einträge unten aus dem Bild, die Liste
  scrollte mit dem Controller nicht mit.
- Nach dem Löschen aller Spielstände zeigte das Hauptmenü weiter **Fortsetzen**, das ins Leere führte.
  Das Menü baut sich jetzt beim Zurückkehren neu auf.
- Ein Schutthaufen hing halb über der **Abkürzungstür** am ersten Glutfeuer.
- **Schild und Schwert** (Wandschmuck) schwebten mitten im Weg zur Schatzkammer und vor der Kammer der
  Gierigen Truhe; in der Gruft des Erwachens standen sie vor bzw. in den Wänden. Jetzt hängen sie an
  Wänden oder sind fort.
- Drei Schuttbrocken und ein Tisch ohne Kollision standen auf begehbaren Wegen; man lief durch sie
  hindurch.
- Vier **Truhen**, die sich nicht öffnen ließen, sind durch Münzhaufen, Fässer und Kisten ersetzt. Was
  wie eine Truhe aussieht, lässt sich öffnen.
- Inventar: Nach dem Belegen eines Platzes der Schnellleiste fehlte für einen Moment der Fokus (fiel
  in der CI als wackeliger Test auf).

### Technik
- Neue Tests: **Requisiten** (keine Deko-Truhen, Wandschmuck an Wänden, Türen frei, keine sperrigen
  Teile auf den Wegen), **Balancing** (Seelen aus dem echten Level gegen die Stufenkosten), **Optionen**
  (jeder Eintrag per Steuerkreuz erreichbar und sichtbar, LB/RB), **Erfolge** (über echte Ereignisse,
  je Spielstand, Karte im Bild). Der Quest-Test prüft Aldrics neuen Platz und das sofortige Rufzeichen.
- Tests und Aufnahmen gehen nie ins Netz: Außerhalb des exportierten Spiels wird ein Update-Download nur
  vorgetäuscht.

## [0.8.4] – 2026-10-11 – Ruhige Menüs

### Behoben
- **Menüs mit dem Stick** (vor allem auf dem Steam Deck): Ein leicht ausgelenkter oder zitternder Stick
  sprang manchmal über Einträge hinweg. Jetzt macht ein Druck genau einen Schritt; der nächste kommt erst,
  wenn der Stick zurückgefedert ist. Hält man ihn, wiederholt sich der Schritt erst nach einer kurzen
  Pause und dann in ruhigem Takt. Das Steuerkreuz verhält sich wie bisher.

### Technik
- Der Steuerungstest stellt den zitternden Stick nach und prüft Schritt, Pause und Wiederholung. Gegen
  den alten Stand sprang der Fokus dabei drei Einträge weiter.

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

