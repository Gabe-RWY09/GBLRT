# GBLRT — Gabe's Big Landing Rate Tool

A freeware landing-rate tool for Microsoft Flight Simulator 2024, by Gabe.

This repository is the official downloads and update channel. The first public
release is being prepared; no installer has been published here yet.

When a release is available, download its `GBLRT_Setup_<version>.exe` from
[Releases](https://github.com/Gabe-RWY09/GBLRT/releases). Run Setup, choose your
installation folder and optional desktop shortcut, then launch GBLRT. Windows
10 version 1809 or newer / Windows 11 x64 and .NET Framework 4.7.2 or newer are
required. Setup includes SimConnect and the Microsoft Visual C++ x64 runtime;
prerequisite installation may require administrator approval.

GBLRT checks this channel at every startup by default. A tray notification
announces newer stable releases; **More features → Check for updates** is also
available. The app verifies the download's SHA-256 and size before offering
**Install and restart**. Installation waits until you are no longer airborne or
capturing a landing. Update checks can be disabled in Settings, and an existing
disabled preference is preserved. Portable installations use manual replacement.

Landing history and settings stay on your PC. Update checks do not upload flight
history or simulator telemetry. GitHub receives normal web request metadata.

Report bugs to **Comrade_Gabe on Discord**. Include the app version, aircraft,
steps to reproduce and relevant diagnostics. Remove personal information before
sharing logs or screenshots.

GBLRT is free to use. Redistribution, resale and public distribution of modified
versions require Gabe's written permission; see [LICENSE.txt](LICENSE.txt).
Third-party runtimes remain subject to their separate terms, included with the
app. This repository does not publish the application source.
