# Reven's Keychron-mod V6 keymap

Some basic changes to keymap

## changes

### Layers
The layers are somewhat modified to meet my needs and adapt to my keycaps. You might want to edit if you are
going for a stock V6 experience.

### Num Lock
I wanted the num lock key to be reversed: off when num lock is on, which for me is the default state.

I took the functions from `keyboards/keychron/v6/v6.c` (line 90 and line 95) and added a modified version of that
to my keymap.

The flag that turns on that functionality is in `keyboards/keychron/vr/ansi/config.h`. This is also where the
indicator LEDs rerference is defined.

### Layer highlight
I added another function to highlight the keys with function in the ffn layer for windows. It works really well,
except if the RGB is togled off, in which case the highlights don't revert when releasing the key. It's probably
a really easy fix, but I'm leaving it for now.

## refs

If anything doesn't work as expected there is info in the docs:

https://docs.qmk.fm/#/feature_rgb_matrix?id=indicators



