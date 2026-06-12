# ⚡ MathStorm
### Secondary School Mathematics Minigame

---

## 📖 Overview

**MathStorm** is a fast-paced, browser-based minigame designed to reinforce secondary school mathematics in a fun and engaging way. Players must catch falling answer bubbles that correspond to equations displayed on screen — all before the timer runs out!

Built entirely in a **single HTML file** using pure HTML, CSS, and JavaScript (no frameworks, no external assets). Background music is generated procedurally using the **Web Audio API**.

---

## 🎮 How to Play

1. Open `index.html` in any modern web browser.
2. Click **▶ Play Now** on the start screen.
3. Read the instructions, then click **🚀 Let's Go!** to begin.
4. A maths equation with a missing value `?` appears in the centre of the screen.
5. **Click the bubble** containing the correct answer before it falls off the screen.
6. Survive all **10 rounds** to complete the storm!

### Controls
| Action | Input |
|--------|-------|
| Answer a question | Click the correct bubble |
| Pause / Resume | Press `Escape` |
| Mute / Unmute | Click the 🔊 button in the HUD |

---

## ⭐ Scoring System

| Event | Points |
|-------|--------|
| Correct answer | **100 pts** base |
| Time bonus | **+10 pts** × seconds remaining |
| Combo ×2 | Score × 2 multiplier |
| Combo ×3 | Score × 3 multiplier |
| Combo ×4 (max) | Score × 4 multiplier |
| Wrong answer | 0 pts + lose 1 life |
| Timeout | 0 pts + lose 1 life |

### Stars Per Round
| Speed | Stars Awarded |
|-------|---------------|
| ≥ 12 seconds remaining | ⭐⭐⭐ |
| 7 – 11 seconds remaining | ⭐⭐ |
| < 7 seconds remaining | ⭐ |
| Wrong / timeout | ☆☆☆ |

---

## ❤️ Lives

- Players start with **3 lives**.
- A life is lost for each **wrong answer** or **timeout**.
- Losing all 3 lives ends the game immediately.

---

## 🔥 Combo System

Answering questions correctly in a row builds a combo:

| Streak | Multiplier | Label |
|--------|------------|-------|
| 2 in a row | ×2 | 🔥 ×2 COMBO! |
| 3 in a row | ×3 | ⚡ ×3 STORM! |
| 4+ in a row | ×4 | 💥 ×4 BLITZ! |

Any wrong answer or timeout **resets** the combo.

---

## 🧮 Mathematics Topics

MathStorm covers **10 secondary school mathematics topics**:

| Topic | Example Questions |
|-------|-------------------|
| **Algebra** | Solve for x: `2x - 4 = 10` |
| **Fractions** | `3/4 × 20 = ?` |
| **Percentages** | `20% of 80 = ?` |
| **Indices** | `2⁵ = ?`, `√144 = ?` |
| **Geometry** | Area, perimeter, angles |
| **Ratio & Proportion** | Simplify ratios, find unknowns |
| **Linear Equations** | Evaluate `y = 2x + 1` |
| **Statistics** | Mean, median, mode |
| **Trigonometry** | `sin 90°`, `cos 0°`, `tan 45°` |
| **Quadratics** | Solve `x² = 64` |

---

## 🔊 Audio

All audio is **synthesised in real-time** using the Web Audio API — no external sound files are required.

| Sound | Trigger |
|-------|---------|
| 🎵 Background music | Plays during gameplay (chiptune, BPM 140) |
| ✅ Correct SFX | Ascending three-note chime |
| ❌ Wrong SFX | Low buzzer sound |
| ⏱️ Timeout SFX | Two-tone warning |
| 🔥 Combo SFX | Four-note ascending fanfare |
| 🎉 Victory SFX | Seven-note melody on game complete |
| 💀 Game Over SFX | Descending sawtooth tones |

The background music features 5 layered tracks:
- **Lead melody** (square wave)
- **Counter melody** (triangle wave)
- **Walking bass line** (sawtooth wave)
- **Pad chords** (sine waves)
- **Drum kit** (kick, snare, hi-hat via noise buffers)

---

## 🗂️ File Structure

```
game_1_mathstorm/
├── index.html      ← Complete game (single file)
└── README.md       ← This file
```

---

## 🌐 Browser Compatibility

| Browser | Support |
|---------|---------|
| Google Chrome | ✅ Full |
| Mozilla Firefox | ✅ Full |
| Microsoft Edge | ✅ Full |
| Safari | ✅ Full (click to unlock audio) |
| Opera | ✅ Full |

> **Note:** Web Audio API requires a user interaction (click) before audio can start. Clicking **Play Now** satisfies this requirement automatically.

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

## 👨‍💻 Technical Details

| Property | Value |
|----------|-------|
| Language | HTML5, CSS3, Vanilla JavaScript (ES5-compatible) |
| Audio | Web Audio API (procedural synthesis) |
| Graphics | CSS animations + Canvas (starfield) |
| File size | ~67 KB (single file) |
| Dependencies | Google Fonts (Inter, Orbitron) — optional |
| Framework | None |

---

*MathStorm — Making maths exciting, one bubble at a time! 🌪️*
