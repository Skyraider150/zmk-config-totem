<picture>
  <source media="(prefers-color-scheme: dark)" srcset="/docs/images/TOTEM_logo_dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="/docs/images/TOTEM_logo_bright.svg">
  <img alt="TOTEM logo font" src="/docs/images/TOTEM_logo_bright.svg">
</picture>

# Five-layer Hungarian Totem

**This is a fork or GEIGEIGEIST's Totem**

[Here](https://github.com/GEIGEIGEIST/totem) you can find the hardware files and build guide.\
[Here](https://github.com/GEIGEIGEIST/qmk-config-totem) you can find the QMK config for the TOTEM.

TOTEM is a 38 key column-staggered split keyboard running [ZMK](https://zmk.dev/) or [QMK](https://docs.qmk.fm/). It's meant to be used with a SEEED XIAO BLE or RP2040.


![TOTEM layout](/docs/images/TOTEM_layout.svg)

## Layout

![keymap](/docs/images/keymap.png)

### General Principles

- Support Hungarian typing.
- Changing between operation systems should be as easy as possible
- Not too many layers
- No (or very few) combos (may be revisited in the future)

### Base Layer

![base](/docs/images/base.png)

The base layer is Colemak-DH with a few changes / additions:

- Z and Y swapped
- Ö, Ü and Tab added
- Homerow mods, except Shift, which is a thumb key without tap-hold
- Esc and Space are Tap-hold layer keys
- NumCtrl and FunNav layers do not have tap-hold
- . and - combo for em-dash

### NumCtrl Layer

![numctrl](/docs/images/numctrl.png)

This layer is for numbers, accents and commonly used controls

- Backspace and Del is here instead of thumb tap-holds: I often long-press them (no tap-hold) or press them quickly multiple times (thumbs are not good for that)
- One-Shot Mods (Gui, Alt and Ctrl) is present on the left hand for convenience and Callum-style mod use
- AltGr on right outer thumb
- Caps Lock and Caps Word are both enabled
- Brightness and Volume control
- Printscreen, Insert
- Ipad Mode (see Ipad compatibility section)

### FunNav Layer

![funnav](/docs/images/funnav.png)

This layer is for Fn keys and navigation.

- The layer can be locked or unlocked by pressing the opposite outer thumb key
- Arrow keys and Home/End PgUp/PgDn on right hand for one-handed navigation
- One-Shot Mods like on the NumCtrl layer
- Shift on opposite side
- Media controls (Prev, Next, Play/Pause)
- Browser navigation (Back, Forward, Refresh)
- Cut, Copy and Paste for convenience when layer is locked
- Home+PgDn for Word Beginning, PgDn+PgUp for Word End

### Sym Layer

![sym](/docs/images/sym.png)

This layer is for symbols that cannot be accessed with shift directly.

- OSM like in the NumCtrl layer
- AltGr on right outer thumb
- Repositioned some symbols for less hand movement

### BtMouse Layer 

![btmouse](/docs/images/btmouse.png)

This layer is for mouse emulation and Bluetooth functions.

- Can be locked or unlocked by opposite outer thumb key
- Mouse pointer and scroll control
- Left and Right Click on thumb keys
- OSM (including Shift) on the right side bottom row
- Macros on the right top row (Teams commands)

## Ipad compatiblity

Ipad Mode activates or deactivates Base Mac layer. Every layer has a corresponding Mac (Ipad) layer that works in Ipad Mode.

### Differences

- Gui and Ctrl are swapped
- Í and 0 are swapped
- Symbol layer uses Ipad key combinations
- End and Home are Gui+Left and Gui+Right respectively
- Word End and Beginning use Alt instead of Ctrl
- Teams macros are absent
