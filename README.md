# 🎰 Lottery Game

> A browser-based betting game with a spinning wheel, sound effects, and real stakes — built in vanilla HTML, CSS, and JavaScript.

Start with $2000. Spread your bets across numbers 0–9 using sliders. Hit "Place Bet", watch the wheel spin, and either hear the cha-ching or the 8-bit lose sound. Simple, addictive, and built entirely from scratch.

---

## 🎯 What It Does

You allocate your balance across any combination of numbers using sliders, place your bet, and a spinning wheel randomly picks the winner. Land on your number and you get **9× your bet** back. Miss and you lose what you wagered.

---

## ✨ Features

- 🎡 Animated spinning wheel with 10 segments (0–9)
- 🎚 Per-number bet sliders — bet on as many numbers as you want simultaneously
- 💵 Live balance tracker — updates after every round
- 🔊 Sound effects: win sound, lose sound, and spinner sound during the spin
- ⚠️ Warning system — prevents invalid bets (overbetting your balance)
- 🎨 Styled with a dark overlay on a custom background image

---

## 🛠 Tech Stack

| | |
|---|---|
| Structure | HTML5 |
| Styling | CSS3 (conic-gradient wheel, animations) |
| Logic | Vanilla JavaScript |
| Audio | HTML `<audio>` API |

---

## 📂 Project Structure

```
Lottery-Game/
├── index.html          # Game layout and wheel
├── styles.css          # Grid, blocks, wheel styling
├── script.js           # Bet logic, spin animation, win/loss calculation
├── background.jpg      # Background image
├── tomato.png          # (if present)
├── cha-ching-7053.mp3          # Win sound
├── spinner-sound-36693.mp3     # Spin sound
└── 8-bit-video-game-lose-sound-version-1-145828.mp3  # Lose sound
```

---

## 🚀 How to Run

No install needed. Just:

1. Clone or download the repo
2. Open `index.html` in any browser

```bash
git clone https://github.com/withaarav/Lottery-Game.git
cd Lottery-Game
open index.html   # Mac
# or double-click index.html on Windows
```

---

## 💡 How It Works

### Betting
Each number (0–9) has a slider capped at $500. You can bet on multiple numbers at once — the total across all sliders is deducted from your balance when you place the bet.

### Spinning
The wheel spins with a CSS rotation animation, landing on a randomly generated number (0–9). The arrow at the top points to the result.

### Payouts
- **Win:** if the wheel lands on a number you bet on → you receive `bet × 9`
- **Loss:** if no match → you lose your total wagered amount
- **Expected value:** −10% per round (house edge built in — 9× payout on a 1-in-10 game)

---

## 🧠 What I Learned

- Building interactive UIs with only vanilla JS — no frameworks
- Using CSS `conic-gradient` to create a styled pie/wheel
- Triggering and controlling CSS animations from JavaScript
- Managing game state (balance, bets, results) purely in the browser
- Integrating the HTML Audio API for event-based sound effects

---

## 🔮 What's Next

- [ ] Persist balance across sessions with localStorage
- [ ] Add a spin history / last 10 results tracker
- [ ] Mobile-responsive layout
- [ ] Multiplayer mode

---

## 📬 Contact

Made by [Aarav Porwal](https://github.com/withaarav) · with.aarav@gmail.com
