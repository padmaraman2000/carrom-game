# 🎯 CarromKing — Play & Win

A complete, beautiful **Carrom Board Game** built with HTML5 Canvas. Play locally with 2–4 players, challenge AI, earn coins, and upgrade your board!

---

## 🎮 Game Features

### Game Modes
| Mode | Players | Description |
|---|---|---|
| 2 Players (Local) | 2 | Same device, pass & play |
| 4 Players (Local) | 4 | Same device, 4-way game |
| vs Computer (AI) | 1 | Play against AI bot |

### 🪙 Coin System
| Action | Coins |
|---|---|
| Win a game | +50 🪙 |
| Lose a game | -20 🪙 |
| Pocket the Queen | +3 pts (in game) |
| Striker pocketed | -1 pt (penalty) |

### 🛒 Board Shop
Buy premium boards & strikers with earned coins!

| Item | Price |
|---|---|
| Classic Wood Board | Free |
| Green Felt Board | 200 🪙 |
| Black Marble Board | 350 🪙 |
| Golden Board | 500 🪙 |
| Neon Glow Board | 800 🪙 |
| Diamond Elite Board | 1,500 🪙 |
| White Striker | Free |
| Fire Red Striker | 150 🪙 |
| Ocean Blue Striker | 150 🪙 |
| Gold Striker | 300 🪙 |
| Neon Green Striker | 500 🪙 |
| Rainbow Striker | 1,000 🪙 |

### 📊 Features
- ✅ Real physics engine (friction, collision, restitution)
- ✅ Aim & power system
- ✅ Timer per turn (30s / 60s / unlimited)
- ✅ AI opponent
- ✅ Leaderboard (local)
- ✅ Board & Striker shop
- ✅ Toast notifications
- ✅ Mobile touch support
- ✅ Queen (Red piece) = +3 points
- ✅ Striker pocketed = -1 penalty
- ✅ Custom winning target (21 / 29 / 50 points)

---

## 🕹️ How to Play

1. **Aim** — Click/tap near the striker and drag to aim
2. **Power** — Drag further for more power (watch power bar)
3. **Shoot** — Release to shoot the striker
4. **Score** — Pocket opponent's pieces to earn points
5. **Queen** — Pocket the red queen for +3 bonus points!
6. **Win** — First to reach target score wins!

---

## 🌐 Play Online

👉 [Play Now](https://YOUR-USERNAME.github.io/carrom-game/)

---

## 🚀 Publish to Play Store (Step-by-Step)

### Method: PWA + TWA (Trusted Web Activity)
This converts your web game into a Play Store app!

### Step 1 — Host the Game Online
```
1. Create GitHub repo → carrom-game → Public
2. Upload index.html
3. Settings → Pages → main → Save
4. Game URL: https://YOUR-USERNAME.github.io/carrom-game/
```

### Step 2 — Create PWA Files
Add these files to your GitHub repo:

**manifest.json:**
```json
{
  "name": "CarromKing",
  "short_name": "CarromKing",
  "description": "Play Carrom, Win Coins, Buy Upgrades!",
  "start_url": "/carrom-game/",
  "display": "standalone",
  "background_color": "#1a0800",
  "theme_color": "#f5a623",
  "icons": [
    { "src": "icon-192.png", "sizes": "192x192", "type": "image/png" },
    { "src": "icon-512.png", "sizes": "512x512", "type": "image/png" }
  ]
}
```

**In index.html `<head>`, add:**
```html
<link rel="manifest" href="manifest.json"/>
<meta name="theme-color" content="#f5a623"/>
```

### Step 3 — Install Tools
```bash
# Install Node.js first from nodejs.org

# Install Bubblewrap (Google's TWA tool)
npm install -g @bubblewrap/cli

# Initialize
bubblewrap init --manifest https://YOUR-USERNAME.github.io/carrom-game/manifest.json

# Build APK
bubblewrap build
```

### Step 4 — Create Google Play Account
1. Go to play.google.com/console
2. Pay one-time $25 registration fee
3. Create Developer Account

### Step 5 — Upload to Play Store
1. Build → `output/app-release-signed.apk`
2. Play Console → Create App → Game
3. Fill in:
   - **App name:** CarromKing
   - **Description:** Play classic carrom, earn coins, buy premium boards!
   - **Category:** Games → Board Games
   - **Content Rating:** Everyone
4. Upload APK
5. Add screenshots (4–8 screenshots)
6. Submit for Review (3–7 days)

### Step 6 — App Details to Fill
```
Title: CarromKing — Play & Win
Short Description: Classic carrom with coins, upgrades & multiplayer!
Full Description:
  🎯 Play the classic carrom board game on your phone!
  
  ✅ 2-Player & 4-Player local multiplayer
  🤖 AI opponent to practice
  🪙 Earn coins by winning games
  🛒 Buy premium board designs & strikers
  🏆 Compete on leaderboard
  
  How to play:
  • Aim the striker by dragging
  • Pocket pieces to score points
  • Queen gives +3 bonus points!
  • First to 21 points wins!
```

---

## 📱 App Icon Required Sizes

| Size | Usage |
|---|---|
| 192×192 px | PWA icon |
| 512×512 px | Play Store icon |
| 1024×500 px | Feature graphic |
| 1080×1920 px | Screenshots |

---

## 🛠️ Run Locally

```bash
# Just open in browser!
open index.html

# For PWA features, use a local server:
npx serve .
# Then open http://localhost:3000
```

---

## 📁 File Structure

```
carrom-game/
├── index.html      ← Complete game
├── manifest.json   ← PWA manifest (add this)
├── icon-192.png    ← App icon (create this)
├── icon-512.png    ← App icon large (create this)
└── README.md       ← This file
```

---

## 📜 License

MIT — Free to use, modify, and publish.

---

## 💡 Tips for Play Store Success

1. **Good screenshots** — Show the game in action
2. **Localize** — Add Hindi, Tamil descriptions (India = biggest carrom market!)
3. **Share on social media** — WhatsApp groups love carrom games
4. **Update regularly** — Add new boards, game modes
5. **Rating prompts** — Ask users to rate after a win
