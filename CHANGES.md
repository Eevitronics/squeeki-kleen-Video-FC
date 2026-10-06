# Modifications by Eevitronics

This repository is a modified version of
[squeeki-kleen Video FC](https://github.com/Gumball2415/squeeki-kleen-Video-FC)
by Persune (© Persune 2025), based on upstream commit `db85869` (v1.1.0).

**These modifications are licensed under the terms of the TAPR Open Hardware
License v1.0** (see `LICENSE.txt`), the same license as the original design.

The original, unmodified versions of every changed file are kept in this
repository's git history (all commits up to and including `db85869`).

## Changed files

### `squeeki-kleen Video FC.kicad_sch` (schematic)
- J4: replaced the MMCX coaxial connector
  (`Connector_Coaxial:MMCX_Molex_73415-0961_Horizontal_0.8mm-PCB`, `Conn_Coaxial`)
  with a 2-pin solder-wire connection
  (`Connector_Wire:SolderWire-0.25sqmm_1x02_P4.2mm_D0.65mm_OD1.7mm`, `Conn_01x02`)
  for video out and ground.
- C3/C4 (unpopulated): value field changed from `~` to empty.
- Re-saved in KiCad 10.

### `squeeki-kleen Video FC.kicad_pcb` (PCB layout)
- J4 footprint changed from MMCX connector to solder-wire pads, with routing
  updated to suit.
- Added silkscreen labels `V` (video out) and `G` (ground) for the J4 pads.
- Added silkscreen text `Adapted by Eevitronics | Aug 2026`.
- Removed the QR code graphic and the `JLCJLCJLCJLC` order-number placeholder.
- The original "squeeki-kleen! Video FC / v.1.1.0 © Persune 2025" silkscreen
  and OSHW logo are kept unchanged.
- Re-saved in KiCad 10.

### `squeeki-kleen Video FC.kicad_pro` (project settings)
- Updated by KiCad 10 (new default settings), and Gerber plot output directory
  set to `gerber_jlcpcb/`.

### `docs/squeeki-kleen Video FC.png`
- Updated render of the modified board.

## New files
- `gerber_jlcpcb/`: Gerber and drill files for JLCPCB manufacture
  (also bundled as `Archive.zip`).
- `squeeki-kleen Video FC.csv`: bill of materials.
- `bom/ibom.html`: interactive BOM / assembly guide.

## Documentation
- `README.md`: added a note that this is a modified fork, a "Buy assembled
  boards" section, and updated MMCX references in the install steps and PCB
  specifications to match the solder-wire pads.
