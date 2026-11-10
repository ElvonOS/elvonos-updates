# ElvonOS updates

This repository hosts the ElvonOS update feed.

- `feeds/stable.json` – current stable release metadata
- `feeds/stable.json.minisig` – minisign signature of the feed

The feed is consumed by `elvonos-update check` on ElvonOS systems. The public
key is shipped in the ISO at `/usr/share/elvonos/update/elvonos.pub`.

Raw URLs:

```
https://raw.githubusercontent.com/ElvonOS/elvonos-updates/main/feeds/stable.json
https://raw.githubusercontent.com/ElvonOS/elvonos-updates/main/feeds/stable.json.minisig
```

Feed format and release process: see the main project documentation
(`documentation/10-free-update-system.md` and `11-free-update-system-howto.md`).
