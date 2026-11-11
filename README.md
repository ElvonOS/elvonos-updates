# ElvonOS updates

This repository hosts the ElvonOS update feed and mirrors the project
screenshots used by the README.

## Feed

- Primary (SourceForge):  
  <https://downloads.sourceforge.net/project/elvonos/feeds/stable.json>
- GitHub mirror:
  <https://raw.githubusercontent.com/ElvonOS/elvonos-updates/main/feeds/stable.json>
- Codeberg mirror:
  <https://codeberg.org/ElvonOS/elvonos-updates/raw/branch/main/feeds/stable.json>

Files:

- `feeds/stable.json` — current stable release metadata
- `feeds/stable.json.minisig` — minisign signature of the feed
- `elvonos.pub` — update public key (also shipped in the ISO at
  `/usr/share/elvonos/update/elvonos.pub`)
- `screenshots/` — English screenshots used by the project README

Every component listed in the feed is signed individually (minisign + sha256).
The client verifies the feed and each payload/script before use.

## Current components

| Component | Version | Type |
|---|---|---|
| `elvonos-apps` | `1.0.7-5` | payload (ElvonOS apps/scripts) |
| `flatpak-store` | `1` | script (Flathub setup) |
| `zz-auto-updates` | `2` | script (enable automatic updates) |

Updates are staged in the background and installed on shutdown/reboot
(ChromeOS-style), or applied manually with `elvonos-update apply`.

## Project

- Source code: <https://github.com/ElvonOS/elvonos> ·
  mirror <https://codeberg.org/ElvonOS/elvonos>
- Downloads and screenshots: <https://sourceforge.net/projects/elvonos/files/>
- Source tarball:
  <https://downloads.sourceforge.net/project/elvonos/releases/1.0.7/ElvonOS-1.0.7-src.tar.zst>
- License: GPL-3.0-or-later (original code); see `LICENSES.md` in the source.

## Documentation

Feed format, signing and release process:
<https://github.com/ElvonOS/elvonos/blob/main/documentation/15-free-updates.md>
