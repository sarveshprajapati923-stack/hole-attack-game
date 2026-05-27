# 🕳️ HOLE ATTACK .io — Complete Setup Guide

## 📁 File Structure (Sirf 1 File!)

```
hole-attack/
└── hole-attack-io.html    ← Yahi ek file hai poora game!
```

Bas itna hi! Koi backend, koi server, koi extra file nahi chahiye.

---

## 🚀 Kaise Chalayein?

### Option 1 — Direct Browser (Seedha)
1. `hole-attack-io.html` file apne phone/PC mein download karo
2. File par double-click karo
3. Browser mein khul jayega — DONE! 🎮

### Option 2 — GitHub Pages (Free Hosting)
1. GitHub par jaao → New Repository banao
2. `hole-attack-io.html` file upload karo
3. Settings → Pages → Source: main branch select karo
4. Tumhara link milega: `https://USERNAME.github.io/REPO/hole-attack-io.html`

### Option 3 — Netlify (Recommended - Free)
1. netlify.com par jaao
2. "Deploy manually" → folder drag karo
3. Instant live link milega!

### Option 4 — Vercel (Free)
1. vercel.com par jaao
2. HTML file upload karo
3. Live ho jayega seconds mein!

---

## 📱 Mobile Par Kaise Install Karein? (PWA Style)

### Android (Chrome):
1. Chrome mein file open karo
2. 3-dot menu → "Add to Home Screen"
3. App ki tarah install ho jayega!

### iPhone (Safari):
1. Safari mein open karo
2. Share button → "Add to Home Screen"
3. App icon milega!

---

## 🎮 Game Features

### Core Gameplay
- Mouse/Touch drag se black hole control karo
- Objects absorb karo — chhote pehle, bade baad
- Jitna bada hole, utne bade objects absorb kar sakte ho
- Score multiplier aur combo system

### Game Modes
| Mode | Description |
|------|-------------|
| ⏱️ TIMED | 60 seconds mein max score |
| ♾️ ENDLESS | Tab tak khelo jab tak hole shrink na ho |
| 💥 CHAOS | Chaos mode frequent trigger, max mayhem |

### 200 Level System
- Har level par difficulty badti hai
- Timer: Level 1 = 60s → Level 200 = 25s
- Objects: Level 1 = 18 → Level 200 = 55
- Score Bonus: Level 1 = ×1 → Level 200 = ×9
- Golden Rate bhi badti hai!

### Maps / Themes
- 🌐 Internet Room
- 💻 Hacker Setup  
- 🏫 School Classroom
- 🤖 AI Office
- 😂 Meme World
- 🌆 Tech City

### Skins (Shop Mein)
| Skin | Cost | Color |
|------|------|-------|
| VOID | Free | Cyan |
| GALAXY | 500 💰 | Purple |
| INFERNO | 800 💰 | Orange |
| FREEZE | 800 💰 | Ice Blue |
| RAINBOW | 1200 💰 | All Colors |
| TOXIC | 1000 💰 | Neon Green |
| LAVA | 1500 💰 | Red |
| STORM | 1500 💰 | Electric |
| GOLDEN | 2500 💰 | Gold (RARE) |
| DARK VOID | 3000 💰 | Deep Purple (RARE) |

### Boosters
| Booster | Cost | Effect |
|---------|------|--------|
| 🧲 Magnet | 200 💰 | Double suction range |
| ⚡ Double XP | 300 💰 | 2× XP + Score |
| ⏰ Time Extend | 250 💰 | +30 seconds |

### Daily Rewards (7-Day Cycle)
- Day 1: +100 💰
- Day 2: +150 💰
- Day 3: +200 💰
- Day 4: Time Booster
- Day 5: +300 💰
- Day 6: Double XP Booster
- Day 7: +500 💰 ⭐

### Daily Spin Wheel
- Har din 1 free spin
- Prizes: 50/100/200/500 coins + Boosters

### Achievements (15 Total)
- First Bite, Century, Voracious, Legendary...
- Combo King (10x), Unstoppable (25x)
- Level milestones: 10, 50, 100, 200
- Weekly Warrior (7-day streak)

### Rank Titles
| Level | Rank |
|-------|------|
| 1 | 🏅 Rookie Hole |
| 10 | ⚡ Void Crawler |
| 20 | 🌀 Event Horizon |
| 50 | 💀 Oblivion |
| 100 | 🌑 Black Hole God |
| 200 | 🌀 INFINITE HOLE |

---

## 🛠️ Technical Details

```
Technology:  Pure HTML + CSS + JavaScript
File Size:   ~97KB (single file)
No deps:     Koi library nahi, koi CDN nahi
Storage:     localStorage (browser mein save)
Audio:       Web Audio API (built-in)
Canvas:      2D Canvas API
Mobile:      Touch events + responsive
FPS:         60fps target
```

---

## 💰 Monetization Ready (Placeholders)

Game mein yeh placeholders already hain:
1. **Reward Ad** — Game over screen par "Watch Ad → Continue"
2. **Interstitial Ad** — Game over screen par
3. **Rewarded Ad** — Spin screen par "Watch Ad → Extra Spin"
4. **In-App Purchase** — Shop mein skin purchases

**AdMob ya AdSense integrate karne ke liye:**
```html
<!-- Game over screen mein yeh replace karo -->
<div class="ad-ph">...</div>
<!-- Apna ad code yahan daalo -->
```

---

## 🎨 Customization

### Logo/Name change karna ho:
```html
<!-- HTML mein dhundho: -->
<div class="game-logo">HOLE<br>ATTACK</div>
<!-- Apna naam daalo -->
```

### Color theme change:
```css
/* CSS mein top par: */
--c: #00f5ff;   /* Primary cyan */
--p: #ff006e;   /* Pink/Red */
--v: #7c3aed;   /* Purple */
--g: #39ff14;   /* Green */
--gold: #ffd700; /* Gold */
```

### New emoji objects add karne:
```javascript
// JS mein THEME_EMOJIS object mein add karo:
internet: ['🌐', '📡', ... , '🆕EMOJI'],
```

---

## 📊 Save Data (localStorage Keys)

| Key | Description |
|-----|-------------|
| ha4_lv | Player Level (1-200) |
| ha4_xp | Current XP |
| ha4_coins | Total Coins |
| ha4_hi | High Score |
| ha4_tabs | Total Absorbed |
| ha4_games | Games Played |
| ha4_eskin | Equipped Skin |
| ha4_skins | Owned Skins |
| ha4_achs | Unlocked Achievements |

---

## 🐛 Common Issues

**Q: Sound nahi aa raha?**
A: Pehle screen par tap/click karo, phir sound aayega (browser autoplay policy)

**Q: Data save nahi ho raha?**
A: Private/Incognito mode mein localStorage kaam nahi karta, normal mode use karo

**Q: Mobile par slow lag raha hai?**
A: Settings mein FPS off karo, aur graphics-heavy skins (Rainbow) avoid karo

**Q: Game full screen kaise karein?**
A: Mobile Chrome mein 3-dot menu → "Add to Home Screen" karo

---

## 📞 Version Info

```
Game:     HOLE ATTACK .io
Version:  v4.0
Date:     2026
Engine:   Vanilla JS + Canvas 2D
Levels:   200
Themes:   6
Skins:    10
Modes:    3
```

---

*Made with 🕳️ — Single HTML file, zero dependencies, infinite fun!*
