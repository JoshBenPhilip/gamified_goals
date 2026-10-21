# Life Quest

A stripped-down Habitica. You get an HP bar, an XP bar and a level, plus easy, medium and hard buttons for **+** (gain XP) and **−** (take damage). You set every number yourself.

## What you can set (Rules tab)

| Setting | Default | What it does |
|---|---|---|
| Max HP | 50 | Size of the health bar |
| Current HP | 50 | Your health right now |
| XP per level | 100 | XP needed for each level. It stays the same every level until you change it |
| Current XP / Level | 0 / 1 | Edit these directly if you want |
| + XP (easy / medium / hard) | 5 / 10 / 20 | XP gained when you tap + |
| − damage (easy / medium / hard) | 2 / 5 / 10 | HP lost when you tap − |
| Refill HP on level up | on | Same as Habitica |
| Lose a level when HP hits 0 | on | XP resets to 0 and HP refills. When off, HP just refills |

Leftover XP carries into the next level. The Log tab lists every tap, and **Undo** reverses the last one.

## Install on your phone

It's a Progressive Web App: plain HTML with no build step and no server code.

1. Host the folder on any static host. With GitHub Pages: repo **Settings → Pages → Deploy from branch**, pick the branch and `/ (root)`.
2. Open the Pages URL on your phone.
   - **iPhone (Safari):** Share → **Add to Home Screen**
   - **Android (Chrome):** ⋮ menu → **Install app** / **Add to Home screen**
3. It opens full screen like a normal app and works offline.

Progress is saved on the phone (browser storage). Use **Rules → Backup → Copy** to save a copy of your data somewhere safe. You can paste it back with **Restore from text**.

## Files

- `index.html`: the whole app (HTML, CSS and JS)
- `manifest.webmanifest`, `icons/`: home-screen install
- `sw.js`: offline cache
