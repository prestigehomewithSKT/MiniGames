# MiniGames

A collection of browser-based mini games, installable as PWA apps on iPhone and Android.

## 🐍 Snake — Nokia 3310

Classic Nokia 3310 Snake with authentic pixel-green LCD aesthetic.

**Play:** `https://prestigehomewithskt.github.io/minigames/snake/`

### Features
- Nokia 3310 phone chassis design with LCD screen
- D-pad touch controls + swipe-to-steer on screen
- Keyboard controls (arrows / WASD)
- Web Audio beep sound effects
- Score display (0000 format) + high score tracker
- Name entry before first game
- Top 3 leaderboard shown after every game
- Installable as a home-screen app (PWA) — works offline

### Global Leaderboard Setup
Scores are saved locally by default (top 3 per device).  
To share scores across **all** devices:

1. Go to [console.firebase.google.com](https://console.firebase.google.com)
2. Create a new project (e.g. `snake-leaderboard`)
3. Left panel → **Build** → **Realtime Database** → **Create Database**
4. Choose a region → **Start in test mode** → Enable
5. Left panel → gear icon → **Project settings**
6. Scroll to **Your apps** → click `</>` → register the app
7. Copy the `firebaseConfig` object shown
8. Open `snake/index.html` and paste your values into `FIREBASE_CONFIG` at the top of the `<script>` section
9. Commit & redeploy — global scores now work!

### Install on iPhone
1. Open the URL above in **Safari**
2. Tap the **Share** button → **Add to Home Screen**
3. Tap **Add** — the game icon appears on your home screen
4. Launch it like a native app (no browser chrome)

### Install on Android
1. Open the URL above in **Chrome**
2. Tap the **⋮** menu → **Add to Home screen** → **Install**
