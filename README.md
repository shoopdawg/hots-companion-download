# hots-companion ⚡
A lightweight, non-intrusive stats overlay for Heroes of the Storm loading screens.

![Overlay Screenshot](./images/preview.png)

## ✨ Features
* **Live Stats:** Pulls player MMR and win rates during the loading screen.
* **Architecture:** Python-based overlay using PyQt6 for transparent rendering.
* **Low Impact:** Sits in the system tray; zero impact on game performance.

## 🚀 Quick Start (v1.9.1)
1. **Download:** Grab the latest `hots-companion.zip` from [the website](https://shoopdawg.github.io/hots-companion-download/).
2. **Extract:** Unzip the folder anywhere on your PC.
3. **Run:** Double-click `hots-companion.exe`.
   * *Note: Click "More Info" -> "Run Anyway" if Windows SmartScreen appears.*
4. **Setup:** Enter your BattleTag (e.g., `Player#1234`) and point the app to your Replays folder.

## 🕹️ How to Use

### Moving the Overlay
The overlay is designed to be flexible for different resolutions:
* **Drag to Reposition:** Simply click and hold anywhere on the stats window to drag it to your preferred location (e.g., center-top or over the hero portraits).
* **Auto-Save:** The app remembers your last position; it will snap back to that spot every time you enter a loading screen.

### Management & Settings
* **System Tray:** The app runs in your system tray (near the clock). Right-click the icon to access **Settings** or **Exit**.
* **Launch on Startup:** To have the app ready for every game, right-click the tray icon and toggle **"Start with Windows"**. 
* **Manual Setup:** If you move your Replay folder, you can update the path via the **Setup Wizard** in the tray menu.

### Best Practices
* **Display Mode:** For the best experience, run Heroes of the Storm in **"Fullscreen Windowed"** mode. This allows the overlay to sit on top without flickering.

## 🛠 Technical Stack
* **Language:** Python 3.11
* **UI:** PyQt6 (Transparent Windows)
* **Backend:** heroprotocol (Blizzard's parsing library)
* **API:** Integration with Heroes Profile for live stats.

## 🔒 Safety & Privacy
This tool only reads your local `*.StormReplay` and `*.battlelobby` files. It does **not** inject code into the HotS game client, making it safe from anti-cheat flags.
