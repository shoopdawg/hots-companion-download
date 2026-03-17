# hots-companion ⚡
A lightweight, non-intrusive stats overlay for Heroes of the Storm loading screens.

![Overlay Screenshot](./images/preview.png)

## ✨ Features
* **Live Stats:** Pulls player MMR and win rates during the loading screen.
* **Architecture:** Python-based overlay using PyQt6 for transparent rendering.
* **Low Impact:** Sits in the system tray; zero impact on game performance.
* ### 📊 Interactive Stats
* **Hover for Details:** During the loading screen, hover your mouse over any player's name to reveal a tooltip. This displays:
    * Win percentages for their most played heroes.
    * Recent match performance.
    * Specific MMR brackets.
* **Level-Based Coloring:** * **Low Level:** Standard white/grey.
    * **Mid Level:** Bronze/Silver/Gold accents.
    * **High Level (1000+):** Vibrant Platinum/Teal glow.

## Requirements
- Windows 10 or 11 (64-bit)
- [PowerShell 7](https://aka.ms/powershell) (`pwsh` on PATH) — required by the lobby parser
- Heroes of the Storm installed and launched at least once

## 🚀 Quick Start (v1.9.1)
1. **Download:** Grab the latest `hots-companion.zip` from [the website](https://shoopdawg.github.io/hots-companion-download/).
2. **Extract:** Unzip the folder anywhere on your PC.
3. **Run:** Double-click `hots-companion.exe`.
   * *Note: Click "More Info" -> "Run Anyway" if Windows SmartScreen appears.*
4. **Setup:** Enter your BattleTag (e.g., `Player#1234`) and point the app to your Replays folder.

## 🕹️ How to Use

### Controlling the Overlay
The app features a **Toggle Button** that stays on screen so you can quickly show/hide your stats.

* **Moving the Button:** To reposition the toggle button, **hold down the `Alt` key** and then click and drag the button to your desired location.
* **Toggling Stats:** A simple click on the button (without Alt) will show or hide the stats overlay.
* **Repositioning Stats:** Like the button, you can move the main stats window by **holding `Alt`** and dragging the window.

### Display Mode
* **Crucial:** Heroes of the Storm **must** be in **"Windowed (Fullscreen)"** mode. If you run in "Fullscreen," Windows will hide the overlay behind the game.

### 📊 Interactive Stats
* **Hover for Details:** During the loading screen, hover your mouse over any player's name to reveal a tooltip. This displays:
    * Win percentages for their most played heroes.
    * Recent match performance.
    * Specific MMR brackets.
* **Level-Based Coloring:** * **Low Level:** Standard white/grey.
    * **Mid Level:** Bronze/Silver/Gold accents.
    * **High Level (1000+):** Vibrant Platinum/Teal glow.


### Management
* **System Tray:** Right-click the icon near your clock to exit or re-run the Setup Wizard.
* **Auto-Save:** The app automatically saves the position of both the button and the overlay, so they stay where you put them across sessions.

## 🛠 Technical Stack
* **Language:** Python 3.11
* **UI:** PyQt6 (Transparent Windows)
* **Backend:** heroprotocol (Blizzard's parsing library)
* **API:** Integration with Heroes Profile for live stats.

## 🔒 Safety & Privacy
This tool only reads your local `*.StormReplay` and `*.battlelobby` files. It does **not** inject code into the HotS game client, making it safe from anti-cheat flags.

## 🛠️ Open Source & Privacy
The **hots-companion** is built with transparency in mind. 
* **Safe:** No code injection; it only reads local files.
* **Source Code:** While this repository serves as the public distribution point, the source code is hosted in a private development repo. I am currently working on auditing the code for a full public source release soon!
