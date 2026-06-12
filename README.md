# ⚡ MathStorm: Base Defense
### Secondary School Mathematics Action Game

---
## 🔗 Quick Access
https://tky2006.github.io/mathStrom/

---
## 📖 Overview

**MathStorm: Base Defense** is a fast-paced, action-oriented HTML5 Canvas minigame designed to reinforce math skills without feeling like a traditional quiz. Players take control of a central base and must defend it from incoming numbered asteroids.

Instead of answering multiple-choice questions, players engage in "Math Combat." By shooting "Ammo" numbers at the incoming enemies, the values are added together. If the sum matches the round's Target Number, the enemy is destroyed!

Built entirely in a **single HTML file** using HTML5 Canvas, CSS, and Vanilla JavaScript. Audio is generated procedurally using the **Web Audio API**.

---

## 🎮 How to Play

1. Open `index.html` in any modern web browser.
2. Click **Start Game** on the main menu.
3. Your base is in the center of the screen. Your cannon aims wherever your mouse cursor points.
4. **HUD / Information:** Look at the top of the screen to see your current Round (out of 10) and the Target Number.
5. **Select Ammo:** Look at the bottom of the screen to see your available Ammo numbers. Select an ammo type by clicking on it or pressing numbers `1` through `5` on your keyboard.
6. **Fire!** Click the mouse to shoot your selected Ammo at the incoming asteroids.
7. **Math Combat:**
   - When your Ammo hits an asteroid, their values are added together.
   - If `Ammo + Asteroid = Target Number`, the asteroid explodes!
   - If they do NOT equal the target number, the asteroid absorbs your ammo, getting larger and changing its value to the sum.
8. Protect your base! If an asteroid hits the center, you lose a life.

---

## ⭐ Scoring & Progression

| Action | Result |
|--------|--------|
| Destroy Asteroid | **+100 pts** |
| Absorb Ammo (wrong math) | Asteroid grows larger, value changes |
| Base Hit | Lose 1 Life |
| 500 Points Scored | Advance to next Round (New Target, Faster Enemies) |
| Complete 10 Rounds | **Victory!** Game Complete |

---

## ❤️ Lives

- Players start with **3 lives**.
- A life is lost every time an asteroid collides with the central base.
- Losing all 3 lives results in a **Game Over**.

---

## 👨‍💻 Technical Details

| Property | Value |
|----------|-------|
| Architecture | Single-Page Application (SPA) |
| Language | HTML5, CSS3, Vanilla JavaScript (ES6) |
| Rendering | HTML5 `<canvas>` API (2D Context) |
| Audio | Procedural Web Audio API (No external mp3/wav files) |
| Dependencies | Google Fonts (Orbitron, Inter) |

### Key Systems:
- **Custom Physics Engine:** Handles velocity vectors, bounding-circle collision detection, and particle physics.
- **Dynamic Targeting:** Procedurally generates valid enemy and ammo values to guarantee solvability based on the round's target.
- **Procedural Audio:** Synthesizes retro sound effects (explosions, lasers, hits) in real-time.

---

## 🚀 Running the Game

Simply open `index.html` in a web browser — **no installation, no server, no internet required** (fonts load from Google Fonts if online; otherwise browser defaults are used).

```
double-click index.html
```

Or via a local server:
```bash
# Python 3
python -m http.server 8000

# Then open: http://localhost:8000
```

---

*MathStorm — Defend the base with the power of addition! 🌪️*
