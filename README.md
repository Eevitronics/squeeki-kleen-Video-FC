# squeeki-kleen-Video-FC

> **Note:** This is a modified version of [squeeki-kleen Video FC](https://github.com/Gumball2415/squeeki-kleen-Video-FC) by Persune, adapted by Eevitronics. The MMCX connector has been replaced with solder-wire pads. See [CHANGES.md](CHANGES.md) for the full list of modifications, which are licensed under the TAPR Open Hardware License.

An open source hardware external composite video bypass preamplifier modboard
for the Famicom/NES

<img src="docs/squeeki-kleen Video FC.png" style="max-width:80%;" />

## Buy assembled boards

Assembled boards of this Eevitronics version are available from the
[Eevitronics Store](https://www.eevitronics.jp). Full design files, including
Gerbers and BOM, remain freely available in this repository under the TAPR
Open Hardware License.

This version is not affiliated with or supported by Persune. For support with
Eevitronics boards, please contact Eevitronics.

## About

I made a compact daughterboard composite video output based on the
[composite amplifier circuit from the AV Famicom](https://www.nesdev.org/wiki/PPU_pinout#Composite_Video_Output).
This is designed to make AV modding RF-only consoles such as the RF Famicom and the Toploading NES-101 compact and simple.

## How to install

TODO: image demonstrations.

1. If your board does not have tented vias, cover the area underneath the PPU with insulating tape. Be sure to also cover underneath the video/ground wire pads to avoid shorts.
2. To reduce stray inductive connections, isolate pin 21 of the PPU by cutting any traces connecting to it as close to the through-hole pad as much as possible.
3. If needed, add additional bypass capacitors in the empty C3 and C4 footprints.

## PCB specifications

Note that this project is optimized for JLCPCB manufacturing.

- 2 layers
- 50.80 x 17.78 mm
- 0.8 mm thickness
- Any surface finish
- Any soldermask/silkscreen color
- Tented vias
	- alternatively, cover area under board with kapton/insulative tape
	

## License

This is licensed under the [TAPR Open Hardware Licence](https://tapr.org/the-tapr-open-hardware-license/). Copyright Persune 2025. Modifications by Eevitronics 2026, see [CHANGES.md](CHANGES.md).

## Credits

Special thanks to:
- The NESDev community for advice and help
- lidnariq for advice
- Finny (grievre/arreffem) for inspiration
- j4m13c0 for testing the board (and notifying me of Q1 pinout error!)

## Support

If you enjoy this project or find it helpful, please support me using the links below!

- <a href='https://ko-fi.com/A0A63YA8J' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://storage.ko-fi.com/cdn/kofi3.png?v=6' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
- [Patreon](https://patreon.com/persune)
