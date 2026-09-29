# Serial — Releases

Public downloads and the [Sparkle](https://sparkle-project.org) auto-update feed
for **Serial**, a native macOS terminal for serial consoles — routers, switches,
firewalls, microcontrollers — over USB serial, Telnet with RFC 2217, SSH and
Bluetooth LE UARTs.

## Download

**[Download the latest release →](https://github.com/jjnicolas/Serial-releases/releases/latest)**

Unzip and move `Serial.app` to `/Applications`. It's Developer ID signed and
notarized by Apple, and updates itself from here via Sparkle. Requires macOS 26
on Apple silicon.

## What's in each release

Builds are published as assets on [GitHub Releases](https://github.com/jjnicolas/Serial-releases/releases),
not as files in the repo:

| Asset | Purpose |
|-------|---------|
| `Serial-X.Y.Z.zip` | The notarized app build for that version. |
| `appcast.xml` | The Sparkle feed, with release notes embedded. The app polls the copy on the latest release (`SUFeedURL`). |

Each download in the appcast is signed with an EdDSA key; the app verifies the
signature against its embedded public key before installing.

## Source

Source code lives in **[jjnicolas/Serial](https://github.com/jjnicolas/Serial)**
(private). For issues, feedback, or feature requests,
[open an issue here](https://github.com/jjnicolas/Serial-releases/issues).

Serial is part of Julien Nicolas's apps & utilities — see them all at
**[apps.tnfnet.org](https://apps.tnfnet.org)**.

---

*Releases are generated and published by `make release` in the source repo —
they aren't edited by hand.*
