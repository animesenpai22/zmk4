# ZMK Config for Corne Keyboard

This is my personal ZMK configuration for my 42-key Corne keyboard.

## Features

- Custom key layout optimized for coding and general use
- Implementation of zmk-helpers (formerly zmk-nodefree-config)
- Balanced home row mods for better typing experience
- Multiple layers for different functionalities
- Custom macros and combos

## Layers

- **Base Layer (0)**: Main typing layer with home row mods
- **Number Layer (1)**: Numbers and basic operations
- **Symbol Layer (2)**: Symbols and special characters
- **Navigation Layer (3)**: Arrows, navigation keys, and macros
- **Settings Layer (4)**: Keyboard settings, Bluetooth controls
- **Mouse Layer (5)**: Pointer controls and media keys
- **Function Layer (6)**: Function keys and number pad
- **Control Layer (7)**: Control key combinations

## Useful Combos

- `Q+W`: Access Settings Layer
- `D+S`: Copy (Ctrl+C)
- `D+F`: Paste (Ctrl+V)
- `A+S`: Undo (Ctrl+Z)
- `A+D`: Redo (Ctrl+Shift+Z)
- `Left Thumb + Right Thumb`: Toggle Typing Layer
- `P+F`: Close (Alt+F4)
- `F+B`: Close Window (Ctrl+W)
- `Q+A`: Task Manager (Ctrl+Shift+Esc)
- `S+M`: Enter

## Building Firmware

To build the firmware:

1. Follow the [ZMK setup instructions](https://zmk.dev/docs/user-setup)
2. Clone this repository
3. Run the build command for your board

## Credits

- Uses [urob's zmk-helpers](https://github.com/urob/zmk-helpers)
