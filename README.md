# VIRUS LQP-79 - Arduino Game - HACK_UPDT

A port of the classic VIRUS LQP-79 game for Arduino-compatible devices. Originally created by TEAM a.r.g., this version has been adapted to run on custom Arduino hardware with an OLED display.

## 📋 Description

VIRUS LQP-79 is an action-packed game where you navigate through levels battling enemies and avoiding obstacles. This implementation is inspired by the Arduboy platform and optimized for DIY Arduino gaming devices.

## 🎮 Controls

| Button | Pin | Function |
|--------|-----|----------|
| **Up** | A3 | Move up |
| **Down** | D2 | Move down |
| **Left** | A1 | Move left |
| **Right** | D3 | Move right |
| **Select (Main)** | A2 | Primary select/action |
| **Select (Secondary)** | D4 | Secondary select/action |

## 🔌 Hardware Requirements

### Display
- **SDA**: A4
- **SCL**: D5

### Optional
- **Buzzer**: D11 (for sound effects)

## 📦 Installation

### Prerequisites

Before uploading the code to your Arduino, you **MUST** download the required libraries. These will be provided in a folder called **"MUST DOWNLOAD THESE LIBRARIES"**.

1. Extract the libraries folder
2. Copy all libraries to your Arduino libraries directory:
   - Windows: `Documents\Arduino\libraries\`
   - Mac: `~/Documents/Arduino/libraries/`
   - Linux: `~/Arduino/libraries/`
3. Restart the Arduino IDE
4. Open `VLQP_AB.ino`
5. Select your board and port
6. Upload to your device

## 🎯 Game Files

```
CODE/
├── VLQP_AB.ino          # Main game file
├── bitmaps.h            # Game graphics
├── bullet.cpp/.h        # Bullet mechanics
├── door.cpp/.h          # Door system
├── elements.cpp/.h      # Game elements
├── enemies.cpp/.h       # Enemy AI
├── game.cpp/.h          # Core game logic
├── globals.cpp/.h       # Global variables
├── level.cpp/.h         # Level management
├── menu.cpp/.h          # Menu system
├── pickup.cpp/.h        # Collectibles
├── player.cpp/.h        # Player mechanics
└── README.md            # This file
```

## 🎨 Credits

**Original Game:**
- **TEAM a.r.g.** - [team-arg.org](http://www.team-arg.org/more-about.html)
  - FUOPY
  - JO3RI
  - STG
  - CASTPIXEL
  - JUSTIN CYR

**Arduboy Version:** 1.6.0  
**Original Game:** [VIRUS LQP-79 Manual](http://www.team-arg.org/zmbt-manual.html)  
**Downloads:** [team-arg.org/zmbt-downloads](http://www.team-arg.org/zmbt-downloads.html)

**This Port:**
- Inspired by **Slimboy** (Arduboy clone)
- Follow on TikTok: [@Hack_updt](https://www.tiktok.com/@Hack_updt)

## 📄 License

This game is licensed under the **MIT License**.

```
Copyright (c) 2016 TEAM a.r.g.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 🔧 Troubleshooting

- **Display not working?** Check your I2C connections (SDA/SCL)
- **Buttons not responding?** Verify pin connections match the control scheme
- **Compilation errors?** Ensure all required libraries are properly installed
- **No sound?** The buzzer on D11 is optional and can be omitted

## 🌟 Support

If you enjoy this project:
- ⭐ Star this repository
- 🎥 Follow [@Hack_updt](https://www.tiktok.com/@Hack_updt) on TikTok
- 🔄 Share with other Arduino enthusiasts

---

**Happy Gaming! 🎮**
