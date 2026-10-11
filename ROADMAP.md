# Roadmap

Was als Nächstes in **Ascheneid** kommt. Fertiges wandert in die [CHANGELOG.md](CHANGELOG.md).

## Als Nächstes: v0.7.2 – Der Eid des Ungebrannten (Aldrics Quest)

Ser Aldric wird vom Stichwortgeber zum Verbündeten. Hrodgar ist dann kein Zufallsfund hinter einer
Scheinmauer mehr, sondern das Ziel einer Quest. Wer sie erfüllt, kämpft im Finale nicht allein.

**Ablauf für den Spieler**
1. **Auftrag:** Am Glutfeuer im Vorhof erzählt Aldric von Hrodgar. Der habe einst geschworen, die
   Gräber seiner Waffenbrüder zu hüten, und plündere sie nun. Aldric ist zu schwach, ihn selbst zu
   stellen, und gibt dem Spieler den **Kerkerschlüssel**.
2. **Verschlossener Weg:** Hrodgars Kammer liegt hinter einem **verschlossenen Gittertor** an der
   Abkürzung, nicht mehr hinter einer Scheinmauer. Ohne Schlüssel steht dort „Verschlossen“, mit
   Schlüssel öffnet sich das Tor (Ketten, Staub, Kamerawackeln).
3. **Kampf:** Hrodgar wie bisher: auf seiner Beute sitzend, Raserei bei halber Kraft.
4. **Rückkehr:** Danach hat Aldric neue Zeilen. Er dankt, richtet sich auf und schwört, den Wächter
   gemeinsam zu stellen.
5. **Lohn:** Vor der Nebelwand leuchtet ein **goldenes Glutzeichen** am Boden. Wer es berührt, ruft
   Aldric als glühenden Phantomritter in den Bosskampf. Er zieht die Aufmerksamkeit des Wächters auf
   sich und kämpft mit Schwert und Schild. Er kann fallen; dann sitzt er nach der nächsten Rast
   wieder am Glutfeuer.
6. **Ausklang:** Nach dem Sieg hat Aldric eigene Schlussworte, und die Bilanz am Ende vermerkt die
   Quest.

**Technik und Aufgaben**
- **Gegner-KI:** Gegner greifen bisher nur den Spieler an. Damit der Wächter zwischen Spieler und
  Aldric wechseln kann, brauchen sie ein allgemeines Ziel. Das ist der größte Umbau.
- **Verbündeter:** Neue Klasse für den Begleiter auf Basis des Ritter-Modells, mit goldenem Phantom-
  Shader, eigener KI (zum Boss laufen, Combos, ausweichen, blocken) und Lebensbalken im HUD.
- **Gittertor:** Neues Interaktionsobjekt mit verschlossenem und geöffnetem Zustand. Die vorhandene
  Fallgitter-Animation lässt sich wiederverwenden.
- **Quest-Zustand:** Kerkerschlüssel, Questschritt und „Aldric beschworen“ werden im Spielstand
  gespeichert, mit eigenen Dialogzeilen je Schritt.
- **Ausgleich:** Mit Aldric bekommt der Wächter rund 25 % mehr Leben, damit der Kampf nicht zu
  leicht wird.
- **Geheimnisse:** Hrodgars Kammer ist dann eine Quest und kein Geheimnis mehr. Dafür kommt
  eine neue dritte Scheinmauer an eine andere Stelle, damit die Bilanz weiter vier Geheimnisse zählt.
- **Tests:** Quest-Ablauf (Schlüssel, Tor zu und offen, Rückkehr zu Aldric), Bot-Durchlauf
  mit Aldric im Bosskampf, Begehbarkeit am Tor.

## Danach: v0.8 – Build-Vielfalt
- **Ringe und Talismane:** 4–5 Stück mit klaren Effekten, z. B. längeres Paradefenster, mehr
  Seelen oder ein kürzerer Dash mit mehr Unverwundbarkeit.
- **Inventar- und Ausrüstungsmenü** mit Gegenstandstexten voller Lore.
- **Wurfmesser oder Glutzauber** als Fernkampf-Option.

## Später: v0.9 – Hinter dem Schleier
- **Die Aschenebene:** ein zweites Gebiet hinter dem Portal mit eigener Optik, neuen Gegnertypen
  und neuem Boss. Es löst den Teaser vom Ende ein.

## Ideenspeicher
Musik, die mit dem Kampf lauter wird · mehrere Spielstände · englische Sprachversion ·
Barrierefreiheit (Untertitelgröße, Farbe des Glints, leichter Modus) · Fotomodus · Erfolge ·
Feedback-Knopf im Pausemenü · Linux-Build
