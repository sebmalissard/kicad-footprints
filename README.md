# KiCad Footprint Libraries

This repository contains the official KiCad footprint libraries.

**The libraries in this repository are intended to be used with KiCad version 8.**

Each footprint library is stored as a directory with the `.pretty` suffix. The footprint files are `.kicad_mod` files within.

Contribution guidelines can be found at http://kicad.org/libraries/contribute
The library convention can be found at http://kicad.org/libraries/klc/

Other KiCad library repositories are located:

* **Symbols:** https://gitlab.com/kicad/libraries/kicad-symbols
* **3D Models:** https://gitlab.com/kicad/libraries/kicad-packages3d
* **Templates:** https://gitlab.com/kicad/libraries/kicad-templates

----------------------------------------------------------------------------------------------------

This is a fork of the official KiCad footprint libraries.

Installation
```
git clone https://github.com/sebmalissard/kicad-symbols ${HOME}/Workspace/KiCad/kicad-footprints
```
Synchronize fp-lib-table
```
meld ${HOME}/.config/kicad/fp-lib-table ${HOME}/Workspace/KiCad/kicad-footprints/fp-lib-table
```

Update KICAD8_FOOTPRINT_DIR in KiCad pcbnew, go to "Preferences" > "Configures Paths..." (example with HOME=/home/seb).
```
KICAD8_FOOTPRINT_DIR = /home/seb/ws/kicad/kicad-footprints
```

Source of added libraries:
* Promicro: https://github.com/Biacco42/ProMicroKiCad.git
