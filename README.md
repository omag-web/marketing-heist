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
| F | Full screen (or the corner button that appears when you move the mouse) |
| B or . | Blank screen (clicker "blank" button) |
| M | Sound on / off |
| 1–6 | Reveal: select crew (resets the 2:00 pitch clock) |
| D | Reveal: mark selected crew's pitch done |
| 1–2 / 0 | Vault: spotlight a question (each has its own clock: 12 and 18 min) / clear |
| H or ? | Key reference overlay (don't press it live) |
| Shift+R, Shift+R | Reset the entire session |

**Plot twist guard:** from The Heist, the first → only arms the twist (a tiny red dot appears bottom-right). Press → again within 2.5 seconds to fire the alarm. The twist timer starts automatically.

**Timers keep running** if you leave a phase, so an accidental arrow press loses nothing. State survives a browser refresh. Open `index.html?reset` to start clean after rehearsing.

## Logo

`assets/MH-Logo.png` is the full lockup (transparent background, built for the dark stage). It's used on the opening and closing screens. `assets/logo-mark.png` (vault + spy) is the small top-bar mark. To swap either one, replace the file or edit the `logo` / `logoMark` paths at the top of the script in `index.html`. If a file is missing, a built-in vault-dial placeholder shows instead.

## Music

`assets/Sly Minor Motif.mp3` loops on the opening and closing screens. It fades in over 4 seconds, fades out over 3 seconds when you move to another phase, and fades out and back in at every loop point. Browsers block audio until the first click or key press, so at the venue click the page once (or press F for full screen) and the music fades up from silence. M mutes music and effects together. Adjust `musicVolume` at the top of the script in `index.html`.

## Deploy

GitHub repo → Settings → Pages → Deploy from branch → `main` / root. Keep a local copy of the folder on the presenter laptop as the offline fallback.
