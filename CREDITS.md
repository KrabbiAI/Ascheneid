# Mitwirkende & Lizenzen

## Spiel
- Design & Umsetzung: DobbyLabs, mit Claude (Anthropic)
- Engine: [Godot Engine 4.7](https://godotengine.org) – MIT

## 3D-Modelle & Animationen – CC0
- KayKit Dungeon Remastered 1.0
- KayKit Character Pack: Adventurers 1.0 (Ritter; Barbar als Mini-Boss Hrodgar; Schurke mit Kapuze als Ser Aldric,
  Mantel von uns aschgrau umgefärbt; im Intro die Eidbrüder: zwei umgefärbte Ritter mit eigenen Aufsätzen
  (Helmbusch, Hörnerhelm, in Blender gebaut) und der Magier, silberblau umgefärbt)
- KayKit Character Pack: Skeletons 1.0 (u. a. Skelettmagier als Knochenseher; der Endboss als Gekrönter Wahn mit
  eigener Krone, aufgebrochener Brust, Kronzepter und umgefärbtem Atlas, in Blender gebaut)

von Kay Lousberg – [kaylousberg.com](https://kaylousberg.com), Quelle: github.com/KayKit-Game-Assets

## Zusätzliche Modelle über Poly Pizza
In Blender importiert und als GLB nach `assets/models/props/` exportiert:
- „Coffin“ (zwei Varianten), „Gravestone“, „Post With Skull“ – Kay Lousberg – CC0
  (poly.pizza/m/ySERERWPgE, /m/WqqeFNrp0e, /m/lrEHKjTy29, /m/gjX6yrxFfq)
- „Practice Dummy“, „Skull“, „Bone“, „Crown“ – Quaternius – CC0
  (poly.pizza/m/1pYOHhwjXP, /m/DJT7N0HuVB, /m/uMs0lDp1u3, /m/i0PZVuVlYv)
- „Throne“ – Poly by Google – **CC-BY 3.0** (poly.pizza/m/bpFCWQSs-aT,
  creativecommons.org/licenses/by/3.0)

## Das Vergessene Refugium (Hub)
In Blender importiert, angepasst und als GLB nach `assets/models/hub/` exportiert:
- „Gravestone“ (zwei Varianten), „Grave“, „Damaged Grave“, „Crypt“, „Post Lantern“, „Iron Fence“,
  „Damaged Iron fence“, „Fence Gate“, „Skull Candle“ – Kay Lousberg – CC0, über Poly Pizza
  (poly.pizza/m/lrEHKjTy29, /m/ErfdU1GJSD, /m/znGrV0V80y, /m/KWtVNrHXVR, /m/iV5x01FYAl, /m/ZSQ65S4lEu,
  /m/MDROOJeCSQ, /m/HfWdsZogtr, /m/h5P9Kuk0V5, /m/94tuTO5eJv)
- „Dead Tree“ (zwei Varianten), „Twisted Tree“ (ohne Laub) – Quaternius – CC0, über Poly Pizza
  (poly.pizza/m/Mcd2zYqyww, /m/oM95bD8buf, /m/8oraKn9m0x)
- „AngelStatue“ – Zsky – **CC-BY 3.0**, über Poly Pizza (poly.pizza/m/6v4CL0nKfT,
  creativecommons.org/licenses/by/3.0)
- „Neo-gothic Church“ – HugoHesseling – **CC-BY 4.0**, über Sketchfab
  (sketchfab.com/3d-models/neo-gothic-church-d514c4e08fc5436ca7f0b227e5437f9e,
  creativecommons.org/licenses/by/4.0) – von uns ohne Treppe, mit geöffnetem Portal, gestreckt und mit
  entsättigter, verkleinerter Textur als Kathedrale des Refugiums
- Texturen „Forest Ground 01“ (Rob Tuytel) und „Mossy Cobblestone“ (Sơn Nguyễn) – CC0, über
  [Poly Haven](https://polyhaven.com) (`assets/textures/hub/`, 1K)
- Himmel mit Blutmond und Sternen, Portalschein, Buntglasfenster: eigene Shader (`assets/shaders/hub_sky.gdshader`,
  `door_glow.gdshader`, `stained_glass.gdshader`)
- Großes Tor und Portalsäulen: eigene Modelle, in Blender gebaut (`assets/models/hub/tor_*.glb`, `portalsaeule.glb`)
- Musik „Refugium“ und die ferne Glocke: eigens mit ffmpeg erzeugt (die Glocke aus Kenneys „bong_001“, CC0)

## Unity Asset Store
- Dobby – „Demon Imp – Hand Painted Series“, BitGem, Unity Asset Store, Lizenz: Standard Unity Asset Store EULA
  (Single Entity). In Blender aufbereitet (Material, Clips geteilt, Sprech-Clip ergänzt), `assets/models/dobby/`

## Texturen – CC0, über [Poly Haven](https://polyhaven.com)
- „Rock Surface“ und „Dirt“ (Steinoberflächen der Gruft, als Detailschicht über der KayKit-Palette;
  `assets/textures/`, 1K)

## Musik – CC0, über [OpenGameArt.org](https://opengameart.org)
- „Lament of the War“ – Cethiel (Bosskampf, Phase 2)
- „Dramatic Boss Encounter“ – cynicmusic (Auftritt des Wächters)
- „Epic Endgame Cinematic“ – cynicmusic (Finale und Abspann)
- „Dungeon Ambience“ – yd (Untermalung beim Erkunden)
- „Fantasy Choir 3“ – César da Rocha (Intro-Sequenz)
- „Battle Theme A“ – cynicmusic (Kampf gegen Hrodgar)

Nach OGG konvertiert und lautheitsnormalisiert (`assets/audio/music/`).

## Soundeffekte
- Kenney RPG Audio, Impact Sounds (u. a. Schritte auf Stein und Erde), Interface Sounds – [kenney.nl](https://kenney.nl) – CC0
- Kampfgeräusche, Feuer, Atmosphäre, Titel- und Bossmusik (Phase 1): eigens synthetisiert
  (`tools/synth_audio.py`)
- Aschewirbel (Brummen, Sog, Aufprall), Mimik (Knurren, Zuschnappen, Atem) und das Keuchen der Figur: eigens mit ffmpeg
  synthetisiert bzw. aus Kenney-Klängen gemischt (`assets/audio/fx/`)

## Tastensymbole – CC0
- Kenney Input Prompts 1.5 (Xbox, PlayStation, Steam Deck, Switch) – [kenney.nl](https://kenney.nl) –
  Auswahl in `assets/ui/prompts/`

## Schriften – SIL Open Font License 1.1
- Cinzel & Cinzel Decorative – Natanael Gama
- EB Garamond – Georg Duffner, Octavio Pardo

Lizenztexte der Schriften: `assets/fonts/OFL-*.txt`
