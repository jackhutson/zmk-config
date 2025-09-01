# Cornish Zen Keymap Reference

## Layer Navigation

| Layer | Number | Access Method |
|-------|--------|--------------|
| QWERTY | 0 | Default layer |
| CURSOR | 1 | Hold BSPC (left thumb) |
| NUMBER | 2 | Hold ESC (right thumb) |
| SYMBOL | 3 | Hold SPACE (right thumb) |
| FUNCTION | 4 | Hold DEL (left thumb) |

## Layer 0: QWERTY (Base)

### Left Half

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 | Col 6 |
|-------|-------|-------|-------|-------|-------|
| ` | Q | W | E | R | T |
| CTRL | A/GUI | S/ALT | D/CTRL | F/SHFT | G |
| SHIFT | Z | X | C | V | B |
| | | | DEL/L4 | BSPC/L1 | ESC/L2 |

### Right Half

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 | Col 6 |
|-------|-------|-------|-------|-------|-------|
| Y | U | I | O | P | \ |
| H | J/SHFT | K/CTRL | L/ALT | ;/GUI | ' |
| N | M | , | . | / | SHIFT |
| ENTER | SPC/L3 | TAB | | | |

**Home Row Mods:**

- Left: A=GUI, S=ALT, D=CTRL, F=SHIFT  
- Right: J=SHIFT, K=CTRL, L=ALT, ;=GUI
- Index fingers (F/J) have special timing

## Layer 1: CURSOR (Navigation)

### Left Half

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 | Col 6 |
|-------|-------|-------|-------|-------|-------|
| CLEAR | SK SHFT | REDO | UNDO | BSPC | CUT |
| LOCK | GUI | ALT | CTRL | SHIFT | COPY |
| JUMP | SEL ALL | SEL LINE | SEL WORD | SEL NONE | PASTE |
| | | | TOG L1 | - | SCREEN |

### Right Half

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 | Col 6 |
|-------|-------|-------|-------|-------|-------|
| CUT | FIND | FIND PRV | FIND NXT | SK SHFT | CLEAR |
| COPY | LEFT | UP | DOWN | RIGHT | LOCK |
| PASTE | HOME | SK PGUP | PGDN | END | JUMP |
| SEL ALL | SEL WORD | SEL NONE | | | |

**Key mappings:**

- CLEAR = Ctrl+K
- REDO = Ctrl+Shift+Z  
- UNDO = Ctrl+Z
- CUT = Ctrl+X
- COPY = Ctrl+C
- PASTE = Ctrl+V
- FIND = Ctrl+F
- FIND PRV = Ctrl+Shift+G
- FIND NXT = Ctrl+G
- LOCK = Ctrl+L
- JUMP = Ctrl+J
- SCREEN = Screenshot macro
- SK = Sticky Key (tap to hold for next keypress)

## Layer 2: NUMBER

### Left Half

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 | Col 6 |
|-------|-------|-------|-------|-------|-------|
| - | - | REDO | UNDO | BSPC | A |
| - | GUI | ALT | CTRL | SHIFT | B |
| - | SEL ALL | SEL LINE | SEL NONE | _ | C |
| | | | - | - | - |

### Right Half

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 | Col 6 |
|-------|-------|-------|-------|-------|-------|
| % | 7 | 8 | 9 | : | K |
| + | 4 | 5 | 6 | - | J |
| * | 1 | 2 | 3 | / | G |
| , | 0 | . | | | |

**Notes:**

- Number pad on right side
- Letters A, B, C, K, J, G for hex input

## Layer 3: SYMBOL

### Left Half

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 | Col 6 |
|-------|-------|-------|-------|-------|-------|
| ! | { | [ | ] | } | ? |
| # | ^ | = | _ | $ | * |
| @ | < | \| | - | > | / |
| | | | % | ( | ) |

### Right Half

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 | Col 6 |
|-------|-------|-------|-------|-------|-------|
| & | - | - | - | - | - |
| ~ | SHIFT | CTRL | ALT | GUI | - |
| + | - | - | - | - | - |
| - | - | - | | | |

**Notes:**

- All symbols on left side
- Modifiers on right middle row

## Layer 4: FUNCTION

### Left Half

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 | Col 6 |
|-------|-------|-------|-------|-------|-------|
| BT 0 | BT 1 | BT 2 | BT 3 | BT 4 | BT CLR |
| - | GUI | ALT | CTRL | SHIFT | - |
| CAPS | SEL ALL | SEL LINE | SEL WORD | SEL NONE | - |
| | | | - | - | - |

### Right Half

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 | Col 6 |
|-------|-------|-------|-------|-------|-------|
| VOL UP | F7 | F8 | F9 | F10 | BRIGHT+ |
| VOL DN | F4 | F5 | F6 | F11 | BRIGHT- |
| MUTE | F1 | F2 | F3 | F12 | BRIGHT AU |
| SCREEN | ZOOM- | ZOOM+ | | | |

**Key mappings:**

- BT 0-4 = Bluetooth profile selection
- BT CLR = Clear bluetooth pairing
- BRIGHT AU = Auto brightness
- ZOOM- = Ctrl+Minus
- ZOOM+ = Ctrl+Equal
- SCREEN = Screenshot macro

## Macros

| Macro | Description | Keys Sent |
|-------|-------------|-----------|
| **select_line** | Select entire current line | HOME, Shift+END |
| **select_word** | Select current word | Ctrl+RIGHT, Ctrl+LEFT, Ctrl+Shift+RIGHT |
| **select_none** | Deselect all | DOWN, UP, RIGHT, LEFT |
| **select_all** | Select all text | Ctrl+A |
| **mac_shot** | Screenshot to clipboard | Ctrl+Shift+Cmd+4 |

## Hold-Tap Behaviors

### Homerow Mods (240ms timeout)

- **Tap**: Send the letter
- **Hold**: Activate modifier
- **Quick tap** (within 200ms): Always sends letter
- **Prior idle** (160ms): Reduces accidental mods

### Index Fingers (180ms timeout)

- Shorter timeout for better responsiveness
- More aggressive quick-tap (300ms)
- Lower idle requirement (100ms)

### Thumb Keys (200ms timeout)

- **Tap**: Send the key (DEL, BSPC, ESC, SPACE)
- **Hold**: Activate layer
- Balanced timing for comfort

## Tips

- **Sticky Keys (SK)**: Tap once to "hold" for the next keypress only
- **Toggle Layer**: Use `tog 1` on CURSOR layer to lock it on/off
- **Screenshot**: The mac_shot macro (SCREEN key) copies screenshot to clipboard
- **Selection Macros**: Available on CURSOR and FUNCTION layers for quick text selection

---
*Last updated from corneish_zen.keymap*
