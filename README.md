# 2 Choc 2 Flat v1.5

![2 Choc 2 Flat PCB](https://github.com/seancaulfield/2choc2flat/)
Low profile 60% PCB designed for Choc V2 switches in hot swap sockets. Based on the Plain60-C design.

## Features
- Compatible with QMK Firmware and VIA Configurator (if you flash a VIA compatible .hex file)
- Compatible with cases supporting the GH60 layout
- LED for capslock (no RGB, no underglow)
- Minimal layout support due to hot swap sockets
- ANSI has 64 keys; ISO(ish) has 65 (split backspace)

## Bill of materials (BOM)


* 64-65 Kailh Choc hot swap sockets (depending on variant)
* 64-65 SOD-323 diodes
* 2 1x9 0.1" header
* 1 1x5 0.1" header
* 2 1206 reverse mount LEDs (for capslock)
* 2 0603 ~470ohm resistors (for capslock LEDs)
* Gateron low-profile stabilizers (1 6.25U, 2-3 2U)
* Plate compatible with Gateron low-profile stabilizers
  * any Cherry plate mount stabilizer compatible should do
  * e.g. [this one at Adafruit](https://www.adafruit.com/product/5133)
* Waveshare RP2040 Tiny, which has the USB port attached via FFC
  * [Amazon](https://www.amazon.com/dp/B0C4FC84V9)
  * [Aliexpress](https://www.aliexpress.us/item/3256806201372671.html)

