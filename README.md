# DoubleAltGr

- Do you type a lot of diarctics (letters with accents) in your language?
- Are you tired of using just Right Alt to do it?
- Are you not using the old,normal Left Alt functions just like me?
- Do you use linux everyday?

**Introducing DoubleAltGr** - the patch to xkb level3 file that replaces the old Right Alt function to make it behave just like the left one - to make diarctics.

Just copy `level3` file as `/usr/share/X11/xkb/symbols/level3` and in layout file of your keyboard layout (ex. `/usr/share/X11/xkb/symbols/cz`) add after every line with `include "level3(ralt_switch)"` the code `include "level3(lalt_switch)"`.
Takes couple of minutes, but it's worth it.

## But if you are lazy piece of monkey...
...you can just copy already pathed keyboard layout of your language from the folder `layouts/` to `/usr/share/X11/xkb/symbols/`, but you still need to copy `level3` to `/usr/share/X11/xkb/symbols/level3`.
