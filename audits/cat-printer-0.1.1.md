# cat-printer 0.1.1 — audit

- Date: 2026-11-02
- Release: https://github.com/rimedot/cat-printer/releases/tag/v0.1.1
- Files and sha256: cat-printer.mevax f5a396585536b4b787dfde0938417769b54a58ea9efb9eb5de279e4c88a63f02
- Build attestation: verified with `gh attestation verify --repo rimedot/cat-printer` (built by this repo's release workflow).
- What was checked: the package holds manifest.json, plugin.js and LICENSE; plugin.js makes no network requests (no fetch, XMLHttpRequest or WebSocket); permissions are reading the current image and Bluetooth to printers named GT01, BLK or SC03h (service ae30); GPL-3.0-or-later because part of the printing code comes from NaitLee/Cat-Printer.
- Not checked: a line-by-line review of plugin.js beyond the checks above.
