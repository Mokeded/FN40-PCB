# FN40 PCB

KiCad PCB design for the **FN40**, a hotswap 40%-style mechanical keyboard (internal project name `4060`).

## Contents

- `4060.kicad_pro` / `4060.kicad_sch` / `4060.kicad_pcb` — KiCad project, schematic, and board files
- `4060.kicad_prl` — KiCad project local settings
- `4060.json` — layout/keyboard-layout-editor data
- `4060.svg` — rendered board image
- `4060.round-tracks-config` — config for the KiCad round-tracks plugin
- `4060-backups/` — autosaved backups of the board file
- `footprints/Switch_Keyboard_Hotswap_Kailh.pretty/` — Kailh hotswap socket footprint library
- `acheron_Components.pretty-master/`, `acheron_Connectors.pretty-master/` — third-party footprint libraries from [Acheron](https://github.com/acheron-project) (also kept as `.zip` archives)
- `random-keyboard-parts.pretty/` — additional footprint library
- `fp-lib-table` / `fp-info-cache` — KiCad footprint library table and cache
- `fabrication-toolkit-options.json` — settings for the [KiCad Fabrication Toolkit](https://github.com/bennymeg/kicad-fabrication-toolkit) plugin used to generate manufacturing files
- `freerouting.dsn` / `temp-freerouting.dsn` — Specctra DSN exports for autorouting with [Freerouting](https://github.com/freerouting/freerouting)
- `kbplacer.log` — log output from the [KiCad KBPlacer](https://github.com/adamws/kicad-kbplacer) plugin used for switch placement
- `production/` — generated manufacturing outputs, including `4060.zip` (Gerbers/drill files), `bom.csv` (bill of materials), `positions.csv` (pick-and-place data), `designators.csv`, and `netlist.ipc`

## Getting started

1. Install [KiCad](https://www.kicad.org/) (developed with KiCad 7/8).
2. Open `4060.kicad_pro` in KiCad.
3. Footprint libraries referenced by `fp-lib-table` are included in this repo — no extra setup should be required.

## Fabrication

Manufacturing-ready files (Gerbers, drill files, BOM, and pick-and-place data) are available in `production/`. These were generated with the KiCad Fabrication Toolkit plugin; re-run it after any board changes to refresh the outputs.

## Credits

- Footprint libraries by [Acheron](https://github.com/acheron-project)
- Hotswap socket footprints from the [Switch_Keyboard_Hotswap_Kailh](https://github.com/) footprint library
