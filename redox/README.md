# redox

Load the json file in the [QMK configurator for redox](https://config.qmk.fm/#/redox/rev1/LAYOUT) to see the layout.

## firmware tweaks

Combo ø/shift needs adjustment on the tapp-combo-mod delay

`redox/rev1/config.h` in the qmk firmawe folder:

```C
#define TAPPING_TERM 125
```

Could possibly be tweaked to different values.

## feedback loop when adjusting layout

1. upload json layout to https://config.qmk.fm/#/redox/rev1/base/LAYOUT

2. tweak and download

3. run:
```bash
cp $(ls -1v Downloads/redox_dvorak*.json | tail -n 1) /home/karl/git/keyboards/redox/redox_dvorak_no.json
```
4. `qmk flash redox_dvorak_no.json`

5. repeat

