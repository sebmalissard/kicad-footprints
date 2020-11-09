## :warning: Deprecation warning

On Oct 1, 2020 this repository, including issues and pull requests, will be archived and transferred to [gitlab.com](https://gitlab.com/kicad/libraries/kicad-footprints/). In order for your pull requests and issues to be imported into GitLab you must set your email address on GitHub to public and use the same address for your GitLab account. Or login to GitLab at least once using the GitHub icon. Otherwise the importer can't correlate the account information and the issues/comments on GitLab will be owned by `kicad-bot` ([importer documentation](https://docs.gitlab.com/ee/user/project/import/github.html#how-it-works)).

---

# KiCad Footprint Libraries

This repository contains the official KiCad footprint libraries.

**The libraries in this repository are intended to be used with KiCad version 5 or with a nightly that supports rounded rectangle and polygon pads.**

Each footprint library is stored as a directory with the `.pretty` suffix. The footprint files are `.kicad_mod` files within 

Weekly builds can be found at https://kicad.github.io/footprints

Contribution guidelines can be found at http://kicad-pcb.org/libraries/contribute
The library convention can be found at http://kicad-pcb.org/libraries/klc/

Other KiCad library repositories are located:

* **Symbols:** https://github.com/kicad/kicad-symbols
* **3D Models:** https://github.com/kicad/kicad-packages3d
* **Templates:** https://github.com/kicad/kicad-templates

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

Update KISYSMOD in KiCad pcbnew, go to "Preferences" > "Configures Paths..." (example with HOME=/home/seb).
```
KISYSMOD = /home/seb/Workspace/KiCad/kicad-footprints
```

Source of added libraries:
* promicro: https://github.com/Biacco42/ProMicroKiCad.git
* Teensy: https://github.com/XenGi/teensy.pretty
* pololu: Add footprint for md15a (motor drive basd on VNH5019 chip)
