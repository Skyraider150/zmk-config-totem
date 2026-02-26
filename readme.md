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
- K and H swapped
- Ö, Ü and Tab added
- Homerow mods, without Shift
- Shift on right thumb, with tap-dance: double tap is CapsWord, triple tap is CapsLock
- Esc and Enter are Tap-hold layer keys
- SymNum and NavCtrl layers do not have tap-hold
- Combos for most commonly used symbols:
  - Left upper row: ', " and +
  - Left lower row: =, (, ), @
  - Right upper row: Backspace and Delete
  - Right lower row: Em-dash, !, ; and *
  - Middle row: \ and /

### Symbols-Numbers Layer

![symnum](/docs/images/symnum.png)

This layer is for accents, numbers and symbols not on the base layer

- Acutes and double acutes under their non-acute counterparts
- All symbols except the ones on base layer
- Numbers on left side for one-handed typing
- Homerow mods are duplicated here
- Sticky AltGr on right outer thumb

### Navigation-Controls Layer

![navctrl](/docs/images/navctrl.png)

This layer is for navigation and controls.

- The layer can be locked or unlocked by pressing the opposite outer thumb key
- Arrow keys and Home/End PgUp/PgDn on right hand for one-handed navigation
- Mods are on the left side
- Shift on opposite side
- Media controls (Prev, Next, Play/Pause)
- Cut, Copy and Paste for convenience when layer is locked
- Combos for jumping one word forward and backward

### Function-Bluetooth Layer

![fnbt](/docs/images/fnbt.png)

This layer is for numbers and F-keys.

- Mods on the left side
- F-keys on right side
- Sticky AltGr on right outer thumb
- Bluetooth functions on the left side

### Mouse Layer 

![mouse](/docs/images/mouse.png)

This layer is for mouse emulation and macros.

- Can be locked or unlocked by opposite outer thumb key
- Mouse pointer and scroll control
- Left and Right Click on thumb keys
- Mods (including Shift) on the right side bottom row
- Macros on the right bottom row

## Ipad compatiblity

Ipad_ activates or deactivates Base_ layer. Every layer has a corresponding Ipad layer (followed by a _) that works in Ipad Mode.

Some Bluetooth profiles are also configured to switch to Ipad mode (or back to Base mode). Currently, BT0 and BT2 are configured as Ipad mode profiles, and the rest as normal profiles.

### Differences

- Gui and Ctrl are swapped
- Í and 0 are swapped
- Symbol layer uses Ipad key combinations
- End and Home are Ctrl+Left and Ctrl+Right respectively
- Word End and Beginning use Alt instead of Ctrl
- Teams macros are absent
- Globe is added to HRMs on the pinky
