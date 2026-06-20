# 🚀 Rocket Game — Python & Pygame

> A 2D interactive rocket game with smooth controls, collision detection, and progressive difficulty — built with Python and Pygame.

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)
![Pygame](https://img.shields.io/badge/Pygame-2.x-green?style=flat&logo=python)
![Game](https://img.shields.io/badge/Type-2D%20Game-orange?style=flat)
![FPS](https://img.shields.io/badge/FPS-60-red?style=flat)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat)

---

## 🎮 Gameplay Demo

> _(Gameplay screenshot ya GIF record karke yahan daalo — OBS Studio ya ShareX se free mein record kar sakte ho)_

```
Controls:
  ↑  Arrow Up    →  Thrust / Move Up
  ←  Arrow Left  →  Move Left
  →  Arrow Right →  Move Right
  P              →  Pause
  R              →  Restart
  ESC            →  Quit
```

---

## 📋 About The Project

A **2D rocket game** built entirely with Python and Pygame featuring smooth physics-based movement, real-time collision detection, progressive difficulty levels, and a score tracking system. Designed to run at a stable 60 FPS for a smooth gameplay experience.

**Key Highlights:**
- Smooth 60 FPS gameplay with frame-rate controlled game loop
- Real-time collision detection between rocket and obstacles
- Progressive difficulty — speed and obstacles increase as score rises
- Score tracking with high score saving
- Clean sprite-based rendering with Pygame

---

## ✨ Features

- ✅ Smooth rocket movement with arrow key controls
- ✅ Real-time collision detection
- ✅ Progressive difficulty — gets harder as you score more
- ✅ High score tracking (saved locally)
- ✅ Pause / Resume functionality
- ✅ Game Over screen with restart option
- ✅ Stable 60 FPS game loop
- ✅ Sound effects _(optional — add your own .wav files)_

---

## 🛠️ Tech Stack

| Component | Technology |
|-----------|-----------|
| Language | Python 3.x |
| Game Engine | Pygame 2.x |
| Physics | Custom 2D movement logic |
| Rendering | Sprite-based 60 FPS loop |
| Data | Local high score file (`.txt`) |
| Version Control | Git & GitHub |

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- Pygame
- Git

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/tomerarvind195-byte/rocket-game.git
cd rocket-game

# 2. Install Pygame
pip install pygame

# OR install all dependencies
pip install -r requirements.txt

# 3. Run the game
python main.py
```

---

## 🎮 How to Play

| Key | Action |
|-----|--------|
| `↑` Arrow Up | Thrust rocket upward |
| `←` Arrow Left | Move left |
| `→` Arrow Right | Move right |
| `P` | Pause / Resume |
| `R` | Restart game |
| `ESC` | Quit game |

**Objective:** Navigate the rocket through obstacles as long as possible. Score increases over time. The game gets faster and harder as your score climbs — beat your high score!

---

## 🧠 Game Architecture

```
main.py
    │
    ├── Game Loop (60 FPS)
    │       │
    │       ├── Event Handler     ← keyboard input
    │       ├── Update()          ← move rocket, spawn obstacles
    │       ├── Collision Check() ← detect hits
    │       └── Render()          ← draw everything on screen
    │
    ├── Rocket (Player)
    │       ├── position (x, y)
    │       ├── velocity
    │       └── sprite image
    │
    └── Obstacle Manager
            ├── spawn new obstacles
            ├── increase speed over time
            └── remove off-screen obstacles
```

---

## 📁 Project Structure

```
rocket-game/
│
├── main.py              # Game entry point & main loop
├── rocket.py            # Rocket (player) class
├── obstacle.py          # Obstacle spawning & movement
├── collision.py         # Collision detection logic
├── score.py             # Score tracking & high score saving
├── highscore.txt        # Local high score storage
├── requirements.txt
├── assets/
│   ├── images/
│   │   ├── rocket.png
│   │   └── obstacle.png
│   └── sounds/
│       ├── thrust.wav
│       └── explosion.wav
└── README.md
```

---

## 🔮 Future Improvements

- [ ] Add multiple levels with different backgrounds
- [ ] Add power-ups (shield, slow-motion, extra life)
- [ ] Implement online leaderboard using Django backend
- [ ] Add animated sprite sheets for rocket and explosions
- [ ] Background parallax scrolling effect
- [ ] Mobile version using Kivy or web version using Pygame CE

---

## 🤝 Contributing

1. Fork the repository
2. Create a new branch (`git checkout -b feature/power-ups`)
3. Commit your changes (`git commit -m 'Add shield power-up'`)
4. Push to the branch (`git push origin feature/power-ups`)
5. Open a Pull Request

---

## 👨‍💻 Author

**Arvind Kumar**

- 🌐 [LinkedIn](https://www.linkedin.com/in/arvind-kumar-399a60338)
- 💻 [GitHub](https://github.com/tomerarvind195-byte)
- 📧 tomerarvind195@gmail.com

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

> ⭐ Agar yeh game enjoy kiya toh **star** zaroor karo aur apna high score comments mein share karo!
