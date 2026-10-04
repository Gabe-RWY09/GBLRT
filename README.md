# GBLRT — Gabe's Big Landing Rate Tool

A freeware landing-rate tool for Microsoft Flight Simulator 2024, by Gabe.

This repository is the official downloads and update channel. The current public release is
[GBLRT 1.0.26](https://github.com/Gabe-RWY09/GBLRT/releases/tag/v1.0.26).

Download the latest `GBLRT_Setup_<version>.exe` from
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

Autoland logging uses AP master state in the first touchdown frame: AP on is
**Autoland**, AP off is **Manual**. Later bounces or rollout AP changes do not
rewrite it. History shows a searchable Landing column; all five popup layouts
mark Autoland. Older unconfirmed records remain Unknown. Aircraft add-ons may
hide AP state from the standard SimVar, so this label is not proof of a certified
landing mode. Bounces retain the first touchdown rate, with later contacts in replay.
For an FMC-only route when starting mid-flight, use More features → Set departure
airport; the app leaves an unobserved origin unknown rather than guessing it.

260 app checks and 3 isolated install/upgrade/uninstall checks passed. The build
is unsigned; new simulator autoland acceptance, clean-PC production setup and
an actual installed update remain unverified. See the release notes and included
checklists. GitHub's automatic Source code archives contain this documentation
repository; the application source remains private/local.

More features sits beside Minimize and opens a window with Flight, Appearance,
Updates & support and Integrations tabs. Update checks use only the official
GBLRT GitHub channel. Saved settings remain in the existing data folder across
upgrades; enabled auto-open repairs its Windows command after an app move.
Both enabled and disabled preferences are respected.

Landing history and settings stay on your PC. Update checks do not upload flight
history or simulator telemetry. GitHub receives normal web request metadata.

Report bugs to **Comrade_Gabe on Discord**. Include the app version, aircraft,
steps to reproduce and relevant diagnostics. Remove personal information before
sharing logs or screenshots.

GBLRT is free to use. Redistribution, resale and public distribution of modified
versions require Gabe's written permission; see [LICENSE.txt](LICENSE.txt).
Third-party runtimes remain subject to their separate terms, included with the
app. This repository does not publish the application source.
