# 2 Choc 2 Flat v1.5 and v2.1

![2 Choc 2 Flat PCB](https://github.com/seancaulfield/2choc2flat/)
Low profile 60% PCB designed for Choc V2 switches in hot swap sockets. Based on the Plain60-C design. Four versions are provided:

* ISO(ish) without lighting
* ANSI without lighting
* ISO(ish) with RGB per-key and underglow
* ANSI with RGB per-key and underglow (TODO)

## Features

- Compatible with QMK Firmware
- Compatible with cases supporting the GH60 layout
- LED for capslock for non-RGB versions
- Minimal layout support due to hot swap sockets
- ANSI has 64 keys; ISO(ish) has 65 (split backspace)
- Both use 2U left shift keys to squeeze in the arrow cluster

## Notes/Cautions

ISO(ish) boards will need to get a custom plate cut, as there are no
commercially available ones I've found. Files for this are included in the
`plate` directory within the project directory for each ISO version.

The layout used is the 2U left shift 60% layout, which allows the arrow cluster
to be included. Check your keycap compatibility before using.

## Bill of materials (BOM)

For all versions:

* 64-65 Kailh Choc hot swap sockets (depending on variant)
* 64-65 SOD-323 diodes
* Gateron low-profile stabilizers (1 6.25U, 2-3 2U)
* Plate compatible with Gateron low-profile stabilizers
  * any Cherry plate mount stabilizer compatible should do
  * e.g. [this one at Adafruit](https://www.adafruit.com/product/5133)
  * DXF/SVG/EPS files for ISOish plates are in the project directories for them
* Waveshare RP2040 Tiny, which has the USB port attached via FFC
  * [Amazon](https://www.amazon.com/dp/B0C4FC84V9)
  * [Aliexpress](https://www.aliexpress.us/item/3256806201372671.html)

For non-RGB versions, you will also need:

* 2 1206 reverse mount LEDs (for capslock)
* 2 0603 ~470ohm resistors (for capslock LEDs)

For RGB versions, you will also need:

* 64-65 SK6812-E reverse mount NeoPixel RGB LEDs
* 16 NeoPixel Nano 2020 RGB LEDs
* 1 SN74LVC2G125DCT SSOP-8 buffer chip
* 0603 1u(ish) X5R capacitor
