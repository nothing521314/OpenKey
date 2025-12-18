# OpenKey

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

OpenKey is an open-source Vietnamese input method application that allows users to type Vietnamese characters on macOS, Windows, and Linux (in development). It supports multiple typing methods including Telex, VNI, and more, with advanced features like spell checking, auto-correction, and customizable macros.

## Features

- **Multiple Input Methods**: Support for Telex, VNI, and Simple Telex typing methods
- **Spell Checking**: Built-in Vietnamese spell checking with auto-correction
- **Smart Mode Switching**: Automatically switches between Vietnamese and English modes based on application context
- **Macro Support**: Create custom shortcuts and macros for frequently used text
- **Unicode Support**: Full Unicode support including precomposed and decomposed forms
- **Cross-Platform**: Available for macOS, Windows, and Linux (in development)
- **Modern Orthography**: Support for modern Vietnamese spelling rules
- **Customizable Hotkeys**: Configurable keyboard shortcuts for mode switching
- **Quick Telex**: Enhanced typing with quick consonant combinations (cc=ch, gg=gi, etc.)

## Usage

### Basic Typing

- **Telex**: Type Vietnamese using Telex method (e.g., `viet` + `nam` = `việt nam`)
- **VNI**: Use VNI input method with numeric accents
- **Simple Telex**: Simplified Telex without tone marks

### Mode Switching

- Default hotkey: `Control + Command + Space` (macOS) or `Control + Z` (Windows)
- Right-click the menu bar icon to switch modes manually

### Features

- **Spell Check**: Automatically corrects common typing errors
- **Auto Capitalization**: Capitalizes the first letter of sentences
- **Macro Expansion**: Type shortcuts to expand to full text
- **Quick Corrections**: Press backspace to undo incorrect transformations

## Building from Source

### Prerequisites

- macOS Mojave (10.14) or later
- Xcode 10 or later

### Build Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/nothing521314/OpenKey.git
   cd OpenKey
   ```

2. Open the project in Xcode:
   ```
   open Sources/macOS/OpenKey.xcodeproj
   ```

3. In Xcode, go to Product → Archive

4. After archiving completes, click "Distribute App"

5. Choose a location to save the built application

### Troubleshooting

If you encounter a "invalid in C99" error during build, add the following declaration at the top of `MJAccessibilityUtils.m`:

```objc
extern BOOL AXAPIEnabled();
```

## Contributing

We welcome contributions! Please:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

OpenKey is released under the [GNU General Public License v3.0](LICENSE).

## Credits

OpenKey is developed by the OpenKey community. Special thanks to all contributors and users.
