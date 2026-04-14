# Getting the APK onto Jet's phone/tablet

## Step 1 — Create the GitHub repo

1. Go to https://github.com/new
2. Name it `princess-compendium`
3. Set it to **Public** (required for free GitHub Pages)
4. Click **Create repository**

## Step 2 — Push this folder to GitHub

Open a terminal in the `PrincessCompendium` folder and run:

```bash
git init
git add .
git commit -m "initial commit: princess compendium v1"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/princess-compendium.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your actual GitHub username.

## Step 3 — Enable GitHub Pages (so games load in the app)

1. Go to your repo on GitHub → **Settings** → **Pages**
2. Under **Source**, choose **Deploy from a branch**
3. Branch: `main`, folder: `/ (root)`
4. Click **Save**

Your games will be live at:
`https://YOUR_USERNAME.github.io/princess-compendium/`

## Step 4 — Update the URL in two files

Open these two files and replace `YOUR_USERNAME` with your actual GitHub username:

- `android/app/src/main/assets/lobby.html` — two occurrences of `YOUR_USERNAME`
- Commit and push: `git add . && git commit -m "set github pages url" && git push`

## Step 5 — Wait for the APK to build (~5 minutes)

1. Go to your repo on GitHub
2. Click the **Actions** tab
3. You'll see a workflow called **"Build APK"** running
4. Wait for the green tick ✅

## Step 6 — Download and install the APK

**Option A — From GitHub Releases (easiest):**
1. Go to your repo → **Releases** (right sidebar)
2. Click the latest release
3. Tap `princess-compendium.apk` to download it
4. Open the downloaded file and install

**Option B — From Actions artifact:**
1. Click the completed workflow run in the Actions tab
2. Scroll to **Artifacts** at the bottom
3. Download `princess-compendium-apk`

**On Android, to allow installation:**
- Settings → Security → Enable **"Install from unknown sources"** (or "Install unknown apps")
- On some phones: Settings → Apps → Special app access → Install unknown apps → Files/Chrome → Allow

---

## Adding new games later

1. Create a folder under `games/` with `index.html` and `manifest.json`
2. Push to `main`
3. GitHub automatically updates `games.json` (via the update-manifest workflow)
4. The app picks up the new game on next launch — **no APK update needed**

## Rebuilding the APK (only needed if you change the Android code)

Push any change to `android/` and the build workflow runs automatically.
Or go to **Actions** → **Build APK** → **Run workflow** to trigger it manually.
