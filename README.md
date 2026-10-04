# GBLRT — Gabe's Big Landing Rate Tool

A freeware landing-rate tool for Microsoft Flight Simulator 2024, by Gabe.

This repository is the official downloads and update channel. The current public release is [GBLRT 1.0.30](https://github.com/Gabe-RWY09/GBLRT/releases/tag/v1.0.30).

## Download and install

Download **GBLRT_Setup_1.0.30.exe** from [Releases](https://github.com/Gabe-RWY09/GBLRT/releases/latest). Exit an older copy through its tray menu, then run Setup and choose your installation folder and optional desktop shortcut. The compiled ZIP is available for manual extraction; extract the entire ZIP and run RUN_APP.bat.

Windows 10 version 1809+ / Windows 11 x64 and .NET Framework 4.7.2+ are required. Setup includes SimConnect and the Microsoft Visual C++ x64 runtime; prerequisite installation may require administrator approval. No SDK or development tools are needed for compiled downloads.

## SimBrief and flight analysis

Open **More features → Flight → SimBrief flight plan** to import by username/Pilot ID or saved OFP XML. Generate the current plan in SimBrief before departure. Enable **Check SimBrief at each takeoff** and save your preferences to fetch the latest plan automatically after confirmed departures. Your account and preferences persist across restarts and updates. When starting mid-flight with an FMC-only route, manually importing a plan also supplies the departure airport; manual departure entry remains available.

The first touchdown is compared with SimBrief's planned runway arrival: **On time** within 10 minutes early or late, **Early** or **Late** outside that window. You can change the saved window. Match the simulator's date/time to the plan; unavailable or conflicting information is shown as unavailable.

**More features → Analysis** provides:

- Flight reports with Flight, Approach, Rollout and Timeline tabs and text export. History also opens the report for a selected landing.
- Explained approach feedback with aircraft-specific speed/bank/descent and configuration targets.
- Rollout distance, time to 60 kt, estimated runway remaining and long-landing indication.
- A personal progress dashboard for the last 10/30/100 or all landings, filtered by aircraft and arrival airport.
- Two-landing comparisons with descent, IAS and G-force graphs.
- Estimated off-block and parking arrival, with gate punctuality separate from touchdown. These are movement/brake-based estimates; unobserved details remain unavailable.

## Landing capture and settings

Bounces retain the first touchdown rate, with later contacts in replay. Autoland logging uses AP master state at first touchdown: AP on is **Autoland**, AP off is **Manual**; missing state remains **Unknown**. Later AP changes do not rewrite it. Aircraft add-ons may hide AP state, so this label is not proof of a certified autoland mode.

**More features** sits beside Minimize and opens Flight, Analysis, Appearance, Updates & support and Integrations tabs. **Settings → Popup → Visible for → Until closed** keeps a popup visible until you press anywhere on it. Settings also offers a desktop shortcut.

## Updates and your data

Startup update checks are enabled for new users. A tray notification announces newer stable releases; check manually in **Settings → App & data → Check now**. Saved enabled and disabled choices are respected. Checks use only the official GBLRT GitHub channel. The app verifies download SHA-256 and size before offering **Install and restart**, and waits until you are no longer airborne or capturing a landing. Portable installations use manual replacement.

Normal settings, history, profiles and themes remain in `%APPDATA%\MSFS2024LandingRateExpansion` across upgrades. Uninstall also retains this data. For portable mode, preserve `Data` and `portable.flag` beside the EXE when replacing files. Update checks do not upload flight history or simulator telemetry. SimBrief requests use the account you supply; online services receive normal web request metadata.

## Bug reports and feature requests

**More features → Updates & support → Feedback** lets you preview and edit a bug report or feature request before continuing to GitHub. Diagnostics are optional and off by default. GitHub drafts are public when you submit them; GBLRT does not submit reports automatically. You can save a local text report instead. For private support, contact **Comrade_Gabe on Discord**. Include the version, aircraft and steps to reproduce, and remove personal information before sharing logs or screenshots.

## Freeware

GBLRT is free to use. Redistribution, resale and public distribution of modified versions require Gabe's written permission; see [LICENSE.txt](LICENSE.txt). Third-party runtimes remain subject to their separate terms, included with the app.

This repository publishes documentation and compiled downloads. GitHub's automatic Source code archives contain this documentation repository; the application source remains private.
