# Mitwirkende & Lizenzen

## Spiel
- Design & Umsetzung: DobbyLabs, mit Claude (Anthropic)
- Engine: [Godot Engine 4.7](https://godotengine.org) – MIT

## 3D-Modelle & Animationen – CC0
- KayKit Dungeon Remastered 1.0
- KayKit Character Pack: Adventurers 1.0 (Ritter; Schurke mit Kapuze als Ser Aldric,
  Mantel von uns aschgrau umgefärbt; im Intro die Eidbrüder: zwei umgefärbte Ritter mit eigenen Aufsätzen
  (Helmbusch, Hörnerhelm, in Blender gebaut) und der Magier, silberblau umgefärbt; Skelett und Animationen des
  Barbaren für den Mini-Boss Hrodgar, dessen Körper, Rüstung und Äxte eigene Modelle sind)
- KayKit Character Pack: Skeletons 1.0 (Skelett und Animationen der Gruftgegner Aschengebein, Grabjäger,
  Sargträger und Kerzenkantor, deren Knochenkörper umgefärbt und mit eigenen Teilen, Waffen und Schilden in Blender umgebaut
  sind; der Endboss als Gekrönter Wahn mit eigener Krone, aufgebrochener Brust, Kronzepter und umgefärbtem Atlas,
  in Blender gebaut)

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
- Pancake, der Friedhofshund (`pancake.glb`): „Shiba Inu“ – Quaternius – CC0, über Poly Pizza
  (poly.pizza/m/y4wdQpg767), von uns zum Corgi umgebaut (Fell, Halstuch, Knickohr) und um eigene Animationen ergänzt
- Pancakes Hütte (`pancake_huette.glb`), in Blender aus Teilen umgebaut: „Hut“ – Quaternius – CC0
  (poly.pizza/m/4MJWbyd6vw), „Bowl Small“ und „Bone“ – Kay Lousberg – CC0 (poly.pizza/m/IRGuF4UebO, /m/gVLnQi8VrX),
  alle über Poly Pizza
- Der Eidhof (Kathedralenvorplatz): die knienden Eidritter-Statuen (`eidritter_kniend_a.res`, `_b.res`) sind der
  Ritter aus KayKit „Adventurers“ (Kay Lousberg, CC0) mit Schwert, von uns neu posiert (kniend), mit eigenem
  Helmbusch zu Stein gebacken (`tools/eidhof_statue.gd`); ebenso die zwei stehenden Wächter auf den Sockeln an der
  Treppe (`eidhof_waechter.res`, `tools/eidhof_waechter.gd`): derselbe Ritter mit KayKit-Zweihänder, gestreckt,
  mit eigenem geschlossenem Visier; Kerzen und Banner aus KayKit „Dungeon Remastered“ (CC0);
  Hofmauer, Torpfeiler, Pflaster, Bänke und die gestürzte Glocke sind eigene, im Spiel erzeugte Geometrie

## Die Eishöhlen
In Blender in unseren Stil umgebaut (Farben, Reif, eigene Eiskristalle, leuchtende Augen) und als GLB nach
`assets/models/eis/` exportiert:
- Raureifwolf: „Wolf“ – Quaternius – CC0, über Poly Pizza (poly.pizza/m/P1gU3Qkr9r)
- Kristallkriecher: „Spider“ – Quaternius – CC0, über Poly Pizza (poly.pizza/m/yRYJiAJyiM)
- Firnschrat und Wächter am Fall: eigene Modelle, in Blender gebaut, auf dem Skelett und mit den Animationen von
  KayKit „Adventurers“ (Kay Lousberg, CC0)
- Gierige Eistruhe und Marten: KayKit (Kay Lousberg, CC0) mit eigenem Raureif
- Frostgebein („Raureifgebein“) und Eiswandler („Glasknochen“): eigene Modelle auf dem Skelett und mit den
  Animationen von KayKit „Skeletons“ (Kay Lousberg, CC0), mit eigenen Waffen
- Höhlenhülle, Felsbrocken, Glimmpilze: eigene Modelle (in Godot erzeugt bzw. in Blender gebaut); Schnee-Textur
  „Snow 02“ – Rob Tuytel – CC0, über [Poly Haven](https://polyhaven.com/a/snow_02) (`assets/textures/eis/`, 1K)
- Zelte und Schlafrolle: „Tent“ und „Bedroll“ – Kenney – CC0, über Poly Pizza (poly.pizza/m/LrTs3hVGXv, /m/12PaVpBY04),
  umgefärbt, mit Schnee
- Requisiten der Expedition und des Bergwerks, umgefärbt und teils mit Schnee (`assets/models/eis/props/`), über Poly Pizza:
  „minecart“, „Broken Cart“, „Shovel“, „Wooden Torch“, „Mineral“, „Rocks“, „Flag“, „Metal Support“, „Stone Wall“, „Tripod“,
  „Wooden Wall“ – Quaternius – CC0 (poly.pizza/m/ypAEwOy2Cn, /m/NBDHe8J7f9, /m/oNBQSf87ZJ, /m/pNsfJzhXiD, /m/STixpWYaTd,
  /m/gYhoEOKItJ, /m/FuOkF3WBrx, /m/ZyUjmgnTyw, /m/tdeAOh3LQV, /m/sVTKUSz3m2, /m/8C9NBoi9cA); „Pickaxe“ – Kenney – CC0
  (poly.pizza/m/UHZH2OoWCS); „Crystal“ (zwei Varianten) – iPoly3D – CC0 (poly.pizza/m/WzWPKHFMkL, /m/nyCeR6poJX)
- Bruchstück einer Wächterstatue (`assets/models/eis/props/statue_bruch.glb`): „Armor Metal“ – Quaternius – CC0, über
  Poly Pizza (poly.pizza/m/TMUoxILh9w), von uns verschweißt, vereinfacht, in Stein umgefärbt und mit abgebrochenem
  Hals, Armstumpf, Bruchstücken und Schnee zum gestürzten Statuentorso umgebaut
- Fallende Eiszapfen: eigenes Modell (in Godot erzeugt)
- Klänge der Eishöhlen (Eis knackt und zerspringt, Tropfen, fernes Ächzen des Eises, Pfeifen im Wind, Brummen der
  stillen Räume) und die Musik „Der Wächter am Fall“ und „Die Erstarrten Schüler“: eigene Arbeit, synthetisiert
  (`tools/synth_ice_audio.mjs`) und mit ffmpeg normalisiert (`assets/audio/fx/`, `assets/audio/music/`)

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
- „Spider Invasion“ – Tozan (Kampf gegen Vethra, Phase 1; als Schleife geschnitten)
- „Determined Pursuit (Epic Orchestra Loop)“ – Emma_MA (Kampf gegen Vethra, Phase 2)

Nach OGG konvertiert und lautheitsnormalisiert (`assets/audio/music/`).

## Soundeffekte
- Kenney RPG Audio, Impact Sounds (u. a. Schritte auf Stein und Erde), Interface Sounds – [kenney.nl](https://kenney.nl) – CC0
- Kampfgeräusche, Feuer, Atmosphäre, Titel- und Bossmusik (Phase 1): eigens synthetisiert
  (`tools/synth_audio.py`)
- Aschewirbel (Brummen, Sog, Aufprall), Mimik (Knurren, Zuschnappen, Atem) und das Keuchen der Figur: eigens mit ffmpeg
  synthetisiert bzw. aus Kenney-Klängen gemischt (`assets/audio/fx/`)
- Warnglocke roter Angriffe (`rote_warnung.ogg`) und das tiefe Dröhnen der Portale (`portal_hum.ogg`): eigene Arbeit,
  mit ffmpeg synthetisiert (`tools/synth_warn_portal_audio.sh`); ebenso der tiefe Warnklang echt unblockbarer
  Angriffe (`rote_warnung_tief.ogg`, `tools/synth_unblockbar_audio.sh`)
- Pancakes Laute (`assets/audio/fx/pancake_*.ogg`), zugeschnitten und lautheitsangeglichen, alle CC0:
  Winseln „dog small whine wants attention“ (kyles, freesound.org/s/455745), „dog whining for attention“ (GeorgeWL,
  freesound.org/s/859937) und „Dog Whimpering“; Bellen „Very Small Dog Barking“ – beide aus der Red Library
  „Animals: Dogs“ (Craig Smith, USC, archive.org/details/Red_Library_Animals_Dogs); Knurren „Dog Shih Tzu Growling 03“
  (Glitchedtones, freesound.org/s/372537); Zähneklappern „Dog Teeth Clattering Clicking“ (qubodup,
  freesound.org/s/841350); Schnüffeln „Dog Sniffing (Near Distance)“ (ralph.whitehead, freesound.org/s/331449);
  Schnarchen „Small Dog Snoring 2“ (Filmscore, freesound.org/s/516872)
- Platschen im schwarzen Wasser des Eisdoms (`assets/audio/fx/wasser_platsch*.ogg`): „40 CC0 water / splash / slime
  SFX“ – rubberduck – CC0, über [OpenGameArt.org](https://opengameart.org/content/40-cc0-water-splash-slime-sfx),
  zugeschnitten und lautheitsangeglichen
- Vethra, die Herzweberin (`assets/audio/fx/spinne_*.ogg`, `netzschuss.ogg`), alle CC0, über OpenGameArt.org,
  zugeschnitten und lautheitsangeglichen: Klicken, Zischen und Netzschuss aus „80 CC0 creature SFX“ und Teil 2 –
  rubberduck; Schrei aus „High pitch scream sounds(2)“ – pauliuw

## Tastensymbole – CC0
- Kenney Input Prompts 1.5 (Xbox, PlayStation, Steam Deck, Switch) – [kenney.nl](https://kenney.nl) –
  Auswahl in `assets/ui/prompts/`

## Schriften – SIL Open Font License 1.1
- Cinzel & Cinzel Decorative – Natanael Gama
- EB Garamond – Georg Duffner, Octavio Pardo

Lizenztexte der Schriften: `assets/fonts/OFL-*.txt`
