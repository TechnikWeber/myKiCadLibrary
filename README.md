# myKiCadLibrary

<p>
  <img alt="KiCad library" src="https://img.shields.io/badge/KiCad-symbols%20%2B%20footprints-blue">
  <a href="LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-green"></a>
</p>

The KiCad symbols and footprints I use in my boards that are not in the KiCad standard
library. Every part has its own folder with the symbol (`.kicad_sym`, plus the legacy
`.lib`/`.dcm`) and the footprint (`.kicad_mod`, plus legacy `.mod`).

| Folder | Part |
|---|---|
| [`173950336`](173950336) | Würth WPME-FDSM fixed step-down regulator module, SIP-3, 4.75–36 V in, 3.3 V / 0.5 A out |
| [`490107670612`](490107670612) | Würth REDFIT IDC SKEDD connector, 6 pins |
| [`490107671012`](490107671012) | Würth REDFIT IDC SKEDD connector, 10 pins |
| [`79528211`](79528211) | Würth WA-BCPH coin cell holder (THT) |
| [`ILI9341`](ILI9341) | 320×240 TFT touch display module with ILI9341 controller (PJRC) |
| [`STM32G071CBT6`](STM32G071CBT6) | STMicroelectronics STM32G071CBT6 (Cortex-M0+, LQFP-48) |
| [`TC2030-IDC`](TC2030-IDC) | Tag-Connect TC2030-IDC cable adapter, 6 pins |

## Use it

In KiCad: *Preferences → Manage Symbol Libraries* and *Manage Footprint Libraries* → add the
`.kicad_sym` file or the part folder of the part you need.

## Known issues

> [!WARNING]
> **ILI9341:** the footprint does not match the dimensions of the module that was bought
> ([AliExpress listing](https://de.aliexpress.com/item/32847628219.html)). Check pin spacing
> and mounting holes against your module before using it.

<img width="353" alt="ILI9341 footprint mismatch" src="https://github.com/user-attachments/assets/a9779d0d-d3de-4f62-8662-d29de5a86457" />

## License

[MIT](LICENSE) for my own work. Parts derived from manufacturer data (e.g. Würth, Tag-Connect)
are provided for convenience; the manufacturers' data sheets are authoritative.
