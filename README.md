# BLE Wireless Corne ZMK Firmware

This repository contains the ZMK configuration for the **Wireless Corne** with full support for ZMK Studio and nice!views.

## Keymap

![keymap image](./keymap-drawer/blecorne.svg)

## Keyboard Features

- Based on Corne KBD
- BoardSource SMT Wireless PCB;
- Low Profile version;
- Choc Black Cloud Series Tactile Switches (40g)
- Nuphy nSa keycaps
- 1200mAh batteries (+5 months of battery life)

## Hardware Information

### Expansion Pinout

The 8-pin header on each side (identical, not mirrored) is read from left to right. These are perfect for screens (nice!view / e-ink) or custom hardware.

| Pin | GPIO | Note                  |
| --- | ---- | --------------------- |
| 1   | 0.07 |                       |
| 2   | 0.21 |                       |
| 3   | 0.12 |                       |
| 4   | 0.23 |                       |
| 5   | VCC  | Switched via pin 0.31 |
| 6   | GND  |                       |
| 7   | 0.19 |                       |
| 8   | 0.05 |                       |

### Battery Information

The PCB features a micro JST connector (BM02B-ACHSS-GAN-ETF) and labeled solder pads (+/-) for custom installs. **Max Dimensions:**

- **Choc:** 30x17x3mm
- **MX:** 30x17x6mm

## Flashing

1. Edit `config/blecorne.keymap`
2. Push -> GitHub Actions builds automatically
3. Download `.uf2` from Actions -> Artifacts
4. USB -> double tap reset -> drag `.uf2` to the drive
5. Flash both halves separately (`_left` and `_right`)

## Links

- [Miryoku](https://github.com/manna-harbour/miryoku)
- [Wireless SMT Corne Docs](https://boardsource.xyz/blogs/guides/wireless-smt-corne-docs)
- [ZMK Docs](https://zmk.dev/docs)
- [Keymap Editor](https://nickcoutsos.github.io/keymap-editor/)
- [ZMK Power Profiler](https://zmk.dev/power-profiler)
- [Lily58 ZMK Config](https://github.com/braun-steven/lily58-wireless-view-zmk-config/tree/main)
