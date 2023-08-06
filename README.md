# Breadboard Regulator

This project aims to replicate the work of [MB102 breadboard power supply module](https://microcontrollerslab.com/mb102-breadboard-power-supply-module-pinout-and-how-to-use-it/), by receiving input from DC barrel jack and convert it into 5V and 3.3V output.

## Components

- [PRT-10811 DC barrel jack](https://www.tokopedia.com/freelab/socket-dc-in-female-jack-dc-barrel-soket-5-5x2-1mm-pcb)
    - Datasheet:
        - [Sparkfun](https://cdn.sparkfun.com/datasheets/Prototyping/18742.pdf)
- [LM7805 IC](https://www.tokopedia.com/rajaavr/ic-regulator-7805-l7805cv-lm7805-voltage-regulator-5-volt)
    - Datasheet:
        - [Sparkfun](https://www.sparkfun.com/datasheets/Components/LM7805.pdf)
        - [DatasheetPDF](https://datasheetspdf.com/pdf-file/766812/ThinkiSemiconductor/LM7805/1)
    - Dependencies:
        - Input diode: [BAT 43 Schottky Diode](https://www.tokopedia.com/elantech/bat43-dioda-vishay-small-signal-schottky-diode-bat-43-elantech)
        - Input capacitor (C-in): [0.33 μF polarized capacitor](https://www.tokopedia.com/elantech/elco-0-33uf-50v-nichicon-fg-fine-gold-0-33-uf-kapasitor-elantech)
        - Input-output noise filtering capacitor(s): [0.1 μF ceramic capacitor](https://www.tokopedia.com/cncstorebandung/10pcs-capacitor-ceramic-kapasitor-keramik-100nf-104-0-1uf-50v-10pcs)
        - Output capacitor (C-out): [0.1 μF polarized capacitor](https://www.tokopedia.com/elantech/elco-0-1uf-50v-nichicon-fg-fine-gold-0-1-uf-kapasitor-elantech-fw)
        - [Red LED 5mm](https://www.tokopedia.com/starlectric/led-5mm-merah-5pcs-pack) (for power indicator)
        - [Pin header 2.54mm](https://www.tokopedia.com/starlectric/header-pin-1x40-40pin-male)
- [LD1117V33 IC](https://www.tokopedia.com/ecadio/ic-regulator-33v-ld1117v33-ld33v)
    - Datasheet:
        - [Addicore](http://www.st.com/st-web-ui/static/active/en/resource/technical/document/datasheet/CD00000544.pdf)
        - [Sparkfun](https://www.sparkfun.com/datasheets/Components/LD1117V33.pdf)
    - Dependencies:
        - Input diode: [BAT 43 Schottky Diode](https://www.tokopedia.com/elantech/bat43-dioda-vishay-small-signal-schottky-diode-bat-43-elantech)
        - Input-output capacitor (C-in and C-out): [10 μF](https://www.tokopedia.com/elantech/elco-10uf-50v-nichicon-fw-gold-10-uf-kapasitor-capacitor-elantech)
        - Input-output noise filtering capacitor(s): [1 μF](https://www.tokopedia.com/elantech/1uf-105-mlcc-multilayer-ceramic-capacitor-1-uf-kapasitor-elantech)
        - [Red LED 5mm](https://www.tokopedia.com/starlectric/led-5mm-merah-5pcs-pack) (for power indicator)
        - [Pin header 2.54mm](https://www.tokopedia.com/starlectric/header-pin-1x40-40pin-male)
- Output: TBD

## How to Use

Open `breadboard-regulator.kicad_pro` file using KiCAD.

NOTE: I'm using KiCAD 7.0.6 for development. Please check if you have the same or compatible version.
