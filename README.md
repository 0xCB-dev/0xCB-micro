# 0xcb-micro
## 1% - 65% keyboard controller with RGB underglow and a backlight driver

Licence | OSHWA | Tindie
:-------------------------:|:-------------------------:|:-------------------------:
![](https://github.com/0xCB-dev/0xcb-micro/blob/main/LICENSE.svg) | [![](https://github.com/0xCB-dev/0xcb-micro/blob/main/PCB/rev1.0/OSHWA.svg)](https://certification.oshwa.org/de000114.html) | <a href="https://www.tindie.com/stores/0xcb/?ref=offsite_badges&utm_source=sellers_conorlburns&utm_medium=badges&utm_campaign=badge_large"><img src="https://d2ss6ovg47m0r5.cloudfront.net/badges/tindie-larges.png" alt="I sell on Tindie" width="200" height="104"></a>

#### Flashing

* `qmk clone`
* `cd qmk_firmware`
* `export LTO=Y`
* To go to bootloader hold the ESC key (row0 col0 / the key on the PCB) while plugging in (or short RST from the ISP header to GND).
* `make 0xcb/micro:via:flash`

### Assembly:

You can use the [humanpnp](https://files.0xcb.dev/0xCB/micro/humanpnp.html) to easily place components.

### PCB:
KiCad 5.99
[Schematic](https://github.com/0xCB-dev/0xcb-micro/blob/main/PCB/rev1.0/Schematic-Static.pdf)

Top | Bottom
:-------------------------:|:-------------------------:
![](https://github.com/0xCB-dev/0xcb-micro/blob/main/PCB/rev1.0/top.png)  |  ![](https://github.com/0xCB-dev/0xcb-micro/blob/main/PCB/rev1.0/bottom.png)

#### BOM:
| References          | Value       | Quantity |Part Nb.          |
|---------------------|-------------|----------|------------------|
| C2, C3, C4, C5, C10 | 100n        | 5        |C478888           |
| C6, C9              | 1u          | 2        |C29936            |
| C7, C8              | 22p         | 2        |C85969            |
| C1                  | 10u         | 1        |C85713            |
| R5, R6, R8          | 10k         | 3        |C98220            |
| R1, R2              | 5.1k        | 2        |C23186            |
| R3, R4              | 22          | 2        |C174301           |
| R7, R9              | 330         | 2        |C104763           |
| D1                  | 1N4148WT    | 1        |C511874           |
| D2                  | WS2812B     | 1        |C114586           |
| U2                  | ATMEGA32U4  | 1        |ATMEGA32U4RC-MU-ND|
| U1                  | USBLC6-2SC6 | 1        |C7519             |
| Y1                  | 16MHz       | 1        |C389842           |
| F1                  | 1A          | 1        |C369150           |
| FB1                 | 600R        | 1        |C74330            |
| Q1                  | FDS9926A    | 1        |C693202           |
| J1                  | USB         | 1        |C168688           |
