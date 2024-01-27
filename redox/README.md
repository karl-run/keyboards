# redox

Load the json file in the [QMK configurator for redox](https://config.qmk.fm/#/redox/rev1/LAYOUT) to see the layout.

# firmware tweaks

Combo ø/shift needs adjustment on the tapp-combo-mod delay

`redox/rev1/config.h` in the qmk firmawe folder:

```C
#define TAPPING_TERM 125
```

Could possibly be tweaked to different values.
