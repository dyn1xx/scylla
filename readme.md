# handwired/scylla

![handwired/scylla](https://i.imgur.com/r4HrXX3.jpeg)

## Layout

### Layer 0

```
┌───┬───┬───┬───┬───┬───┐       ┌───┬───┬───┬───┬───┬───┐
│Esc│ 1 │ 2 │ 3 │ 4 │ 5 │       │ 6 │ 7 │ 8 │ 9 │ 0 │ + │
├───┼───┼───┼───┼───┼───┤       ├───┼───┼───┼───┼───┼───┤
│Tab│ Q │ W │ E │ R │ T │       │ Y │ U │ I │ O │ P │ ¨ │
├───┼───┼───┼───┼───┼───┤       ├───┼───┼───┼───┼───┼───┤
│Shf│ A │ S │ D │ F │ G │       │ H │ J │ K │ L │ ö │ ä │
├───┼───┼───┼───┼───┼───┤       ├───┼───┼───┼───┼───┼───┤
│Ctr│ Z │ X │ C │ V │ B │       │ N │ M │ , │ . │ - │ ' │
└───┴───┴───┼───┼───┼───┤       ├───┼───┼───┼───┴───┴───┘
            │MD1│Alt│Cps│       │MD1│Alt│Cps│
            └───┼───┼───┤       ├───┼───┼───┘
                │Spc│Sup│       │Ent│Bac│
                └───┴───┘       └───┴───┘
```

### Layer 1

```
┌───┬───┬───┬───┬───┬───┐       ┌───┬───┬───┬───┬───┬───┐
│Esc│F1 │F2 │F3 │F4 │F5 │       │F6 │F7 │F8 │F9 │F10│F11│
├───┼───┼───┼───┼───┼───┤       ├───┼───┼───┼───┼───┼───┤
│Tab│---│N7 │N8 │N9 │Nxt│       │Vo+│Pgu│Hme│B+ │ Å │F12│
├───┼───┼───┼───┼───┼───┤       ├───┼───┼───┼───┼───┼───┤
│Shf│---│N4 │N5 │N6 │Ply│       │Lft│Dwn│Up │Rgt│---│Mte│
├───┼───┼───┼───┼───┼───┤       ├───┼───┼───┼───┼───┼───┤
│Ctr│---│N1 │N2 │N3 │Prv│       │Vo-│Pgd│End│B- │---│Pts│
└───┴───┴───┼───┼───┼───┤       ├───┼───┼───┼───┴───┴───┘
            │MD1│Alt│Cps│       │MD1│Alt│Cps│
            └───┼───┼───┤       ├───┼───┼───┘
                │Spc│Sup│       │Ent│Bac│
                └───┴───┘       └───┴───┘
```

### Layer 2

```
┌───┬───┬───┬───┬───┬───┐       ┌───┬───┬───┬───┬───┬───┐
│Rst│---│---│---│---│---│       │---│---│---│---│---│---│
├───┼───┼───┼───┼───┼───┤       ├───┼───┼───┼───┼───┼───┤
│---│---│ @ │ < │ + │---│       │---│ ( │ [ │ { │   │---│
├───┼───┼───┼───┼───┼───┤       ├───┼───┼───┼───┼───┼───┤
│ | │ ! │ " │ # │ $ │ % │       │ & │ / │ ~ │ = │ ` │ * │
├───┼───┼───┼───┼───┼───┤       ├───┼───┼───┼───┼───┼───┤
│---│---│---│ > │ - │---│       │---│ ) │ ] │ } │   │---│
└───┴───┴───┼───┼───┼───┤       ├───┼───┼───┼───┴───┴───┘
            │MD1│Alt│Cps│       │MD1│Alt│Cps│
            └───┼───┼───┤       ├───┼───┼───┘
                │Spc│Sup│       │Ent│Bac│
                └───┴───┘       └───┴───┘
```

Make example for this keyboard (after setting up your build environment):

    make handwired/scylla:default

Flashing example for this keyboard:

    make handwired/scylla:default:flash

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Bootloader

Enter the bootloader in 3 ways:

* **Bootmagic reset**: Hold down the key at (0,0) in the matrix (usually the top left key or Escape) and plug in the keyboard
* **Physical reset button**: Briefly press the button on the back of the PCB - some may have pads you must short instead
* **Keycode in layout**: Press the key mapped to `QK_BOOT` if it is available
