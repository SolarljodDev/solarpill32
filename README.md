# SolarPill32

A small, STM32-pin-compatible development/breakout board built around the
**CH32V303CBT6** (WCH, RISC-V32, LQFP-48). Footprint and pinout follow the
classic "blue pill / black pill" layout used by STM32F103C8T6 boards, so it
can be used as a drop-in RISC-V alternative in existing STM32 blue/black pill
projects and carriers.

## Board

- MCU: CH32V303CBT6, LQFP-48, 7x7 mm, 0.5 mm pitch (custom footprint
  `LQFP-48_7x7mm_P0.5mm.kicad_mod` included, as it's not in stock KiCad
  libraries).
- 4-layer PCB: top/bottom signal layers plus dedicated GND and 3V3 inner
  planes.
- Designed in KiCad 9.

## Repository contents

| Path | Description |
|---|---|
| `ch32_v303cb.kicad_pro/.kicad_sch/.kicad_pcb` | Main board project (schematic, layout) |
| `filter.kicad_sch` | Hierarchical sheet: power supply filtering |
| `LQFP-48_7x7mm_P0.5mm.kicad_mod` | Custom footprint for the CH32V303CBT6 |
| `SW_conv/` | Secondary small PCB project: switching converter module |
| `gerber/` | Exported Gerber + drill files for fabrication |

Files that KiCad regenerates automatically (autosave backups, `.lck` lock
files, `fp-info-cache`, local `.kicad_prl` view-state files, editor history)
are intentionally excluded — see `.gitignore`.

## License

Hardware design files (schematics, PCB layout, footprints, Gerbers) in this
repository are licensed under the
[CERN Open Hardware Licence Version 2 - Strongly Reciprocal (CERN-OHL-S-2.0)](LICENSE).
