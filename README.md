# 🎮 3D 5v1 Stealth Hide & Seek: Relocation Lockdown

A browser-based, high-stakes 3D multiplayer game where **5 Seekers** armed with tazers hunt down **1 Hider** equipped with stealth gadgets and dynamic objective requirements. Built using **Three.js**, **Tailwind CSS**, and modern web APIs.

---

## 🌟 Key Features

* **5v1 Asymmetric Gameplay**: 5 Seekers vs 1 Hider.
* **Dynamic Relocation System**: To prevent passive hiding, the Hider is given randomized 20-second waypoints every 45 seconds. Failing to reach a destination in time temporarily disables invisibility and triggers map pings.
* **Invisibility & Stale Spot Mechanics**:
  * **Stationary**: 2-second stealth setup (`0s–1s`: 50% translucent, `1s–2s`: 100% invisible).
  * **Moving / Stale Spot**: Instantly reveals the Hider to all Seekers.
* **Cross-Platform Controls**:
  * **PC**: Full WASD movement, mouse pointer lock, and action hotkeys.
  * **Mobile / Touch**: Built-in virtual D-Pad, touch-drag camera control, and touch action buttons.
* **Gadgets & Abilities**:
  * **Hider**: Smoke Bomb (`Q` / `SMK`) and Hologram Decoy (`E` / `DEC`).
  * **Seekers**: Direct-fire Tazer Laser viewmodel (`Left-Click`).
* **Single-Player & Multiplayer Modes**:
  * Quick Play with AI Bots.
  * Custom lobby room code system.

---

## 🛠️ Tech Stack

* **Rendering Engine**: [Three.js](https://threejs.org/) (WebGL)
* **Styling & UI**: [Tailwind CSS](https://tailwindcss.com/) & FontAwesome Icons
* **Game Loop & Physics**: Custom 3D collision detection, bounding boxes, raycasting, and vector math

---

## 🎮 How to Play & Controls

### Objectives
* **Hider**: Survive the 5-minute round limit. Maintain invisibility by staying stationary when hidden, but continuously move to new waypoint relocation zones when assigned.
* **Seekers**: Track down the Hider and tag/taze them before time expires.

---

### PC Controls

| Action | Key / Input |
| :--- | :--- |
| **Move** | `W`, `A`, `S`, `D` |
| **Look Around** | Mouse |
| **Jump** | `Spacebar` |
| **Fire Tazer (Seeker)** | `Left-Click` |
| **Smoke Bomb (Hider)** | `E` |
| **Hologram Decoy (Hider)** | `Q` |
| **Unlock Cursor** | `ESC` |

---

### Mobile Controls

* **Left Side**: Virtual directional D-Pad (Up, Down, Left, Right).
* **Right Side Drag**: Touch look area to rotate camera view.
* **Action Buttons**: `JUMP`, `CROSSHAIR` (Fire Tazer), `SMK` (Smoke), `DEC` (Decoy).

---

## 🚀 Quick Start / Deployment

Since this project is contained within a single file, setup is minimal:

1. Clone or download this repository.
2. Save the main game file as `index.html`.
3. Open `index.html` in any modern web browser (Chrome, Firefox, Edge, Safari), or host it directly on platforms like **GitHub Pages**, **Vercel**, or **Netlify**.

---

## 📁 File Structure

```text
├── index.html        # Main HTML entrypoint containing styles, UI, Three.js engine & game logic
└── README.md         # Project documentation
```