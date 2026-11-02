# Quest Log — hosting on GitHub Pages + syncing to your phone

## 1. Put it online (about 5 minutes, free)
1. Sign in at github.com and click **New repository**. Name it e.g. `quest-log`. Keep it **Public** (free GitHub Pages needs that; your save is NOT stored here — see below).
2. Click **uploading an existing file**, drag in everything from this folder (`index.html`, `manifest.json`, the three `icon-*.png` files), and **Commit**.
3. Go to **Settings → Pages**. Under *Build and deployment*, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, **Save**.
4. After a minute your game is at `https://YOUR-USERNAME.github.io/quest-log/`.

## 2. Make a token for syncing (once)
1. GitHub → **Settings → Developer settings → Personal access tokens → Tokens (classic) → Generate new token (classic)**.
2. Name it `quest-log-sync`, tick ONLY the **gist** permission, choose an expiry, and generate. Copy it now (GitHub shows it once).

## 3. Connect your first device
1. Open the game, scroll to the bottom → **Cloud Sync**.
2. Paste the token, leave Gist ID blank, press **Connect**. Your current save is uploaded to a new *secret* Gist, and the Gist ID appears.

## 4. Connect your phone
1. Open the Pages URL on your phone. Optionally use *Share → Add to Home Screen*.
2. Cloud Sync → paste the same token and the Gist ID → **Connect**. Your save downloads.

## Using it
- Changes upload a few seconds after you make them and download when you reopen the app. **Sync now** forces it.
- If both devices changed without syncing, the game asks which save to keep.
- Your token is stored only in that browser (not in the save, the exports, or the repo). Treat it like a password. Disconnecting a device removes it from that browser.

## Things to know
- The save lives in your private Gist, not in the public repo. The public repo only contains the game itself.
- Progress made before connecting is on the browser where you made it. Connect from the browser holding your real save FIRST (or Export it and Import on the new site).
