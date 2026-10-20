# Marketing Heist · Mission Control

Projector-only presentation for the Marketing Functional Area session at the 2026 NLC-RISC Staff Conference. One audience-facing screen, fixed 1920×1080 stage (scales to any 16:9 display), no dependencies, works offline by double-clicking `index.html`.

## Keys

| Key | Action |
|---|---|
| → / Page Down | Next phase |
| ← / Page Up | Previous phase |
| Space | Start / pause timer |
| + / − | Add / remove 1 minute |
| R, R | Reset current timer (press twice) |
| F | Full screen |
| B or . | Blank screen (clicker "blank" button) |
| M | Sound on / off |
| 1–6 | Reveal: select crew (resets the 2:00 pitch clock) |
| D | Reveal: mark selected crew's pitch done |
| 1–3 / 0 | Vault: spotlight a question / clear |
| H or ? | Key reference overlay (don't press it live) |
| Shift+R, Shift+R | Reset the entire session |

**Plot twist guard:** from The Heist, the first → only arms the twist (a tiny red dot appears bottom-right). Press → again within 2.5 seconds to fire the alarm. The twist timer starts automatically.

**Timers keep running** if you leave a phase, so an accidental arrow press loses nothing. State survives a browser refresh. Open `index.html?reset` to start clean after rehearsing.

## Logo

Put the logo files in an `assets/` folder and set them at the top of the script in `index.html`:

```js
logo: 'assets/logo.png',          // full lockup, opening + closing screens
logoMark: 'assets/logo-mark.png', // small icon for the top bar (optional)
logoHasTagline: true,             // if the artwork already includes the tagline
```

If a file is missing, the built-in vault-dial placeholder shows instead.

## Deploy

GitHub repo → Settings → Pages → Deploy from branch → `main` / root. Keep a local copy of the folder on the presenter laptop as the offline fallback.
