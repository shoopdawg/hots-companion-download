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

## 🛠 Technical Stack
* **Language:** Python 3.11
* **UI:** PyQt6 (Transparent Windows)
* **Backend:** heroprotocol (Blizzard's parsing library)
* **API:** Integration with Heroes Profile for live stats.

## 🔒 Safety & Privacy
This tool only reads your local `*.StormReplay` and `*.battlelobby` files. It does **not** inject code into the HotS game client, making it safe from anti-cheat flags.
