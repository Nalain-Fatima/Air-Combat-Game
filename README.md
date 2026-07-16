# ✈️ Apex Strike — Air Combat

A browser-based 3D air combat game built with **Three.js** — no installs, no build step, just open the HTML file and fly. Featuring realistic flight physics, missile lock-on combat, AI dogfights, SAM defenses, and 7 selectable battle zones, all wrapped in a clean military-style HUD that works on both PC and mobile.

![Platform](https://img.shields.io/badge/platform-Web%20%7C%20Android%20%7C%20iOS-4fb2ff?style=flat-square)
![Engine](https://img.shields.io/badge/engine-Three.js-black?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-lightgrey?style=flat-square)

---

## 🎮 Play

- **Play instantly:** open [`air-combat-game.html`](./air-combat-game.html) in any modern browser — desktop or mobile.
- **Live demo (GitHub Pages):** `https://<your-username>.github.io/<your-repo>/air-combat-game.html`

No dependencies to install. Everything (engine, physics, audio, UI) runs from a single self-contained HTML file, loading Three.js from a CDN.

---

## ✨ Features

### Flight & Combat
- Smooth, stable flight model — clamped bank & pitch angles, coordinated turns, no unexpected flips or spins
- Machine gun with fast, accurate hit detection
- Lock-on homing missiles with a realistic acquisition system (lock speed depends on how centered the target is)
- Gravity-affected bombs with splash damage
- Countermeasure flares that decoy incoming missiles
- Afterburner boost with camera FOV kick, flame effects, and engine sound
- Camera shake on firing, missile launches, explosions, and taking damage

### World & Visuals
- 7 selectable battle zones, each with unique sky, lighting, fog, and terrain:
  - 🏜️ Desert Battlefield
  - ⛰️ Mountain Base
  - 🌊 Ocean War Zone
  - ❄️ Snow Region
  - 🌲 Forest Valley
  - 🌃 Night City
  - 🌅 Sunset Battlefield
- HDR-style gradient skies, layered volumetric clouds, animated ocean shader
- Military bases with hangars, control towers, and SAM turret defenses
- Cinematic explosions — fireballs, shockwave rings, drifting smoke, dynamic light flashes

### Enemy AI
- Enemy fighters patrol, intercept, and dogfight with lead-aim gunfire and break-off maneuvers
- Ground-based SAM sites track and fire homing missiles
- Difficulty scales with survival wave count

### UI / Controls
- Minimal, professional military HUD — radar, health, ammo counters, mission timer, lock indicator
- Touch joystick + on-screen fire/missile/bomb/boost/flare buttons for mobile
- Full keyboard + mouse support for PC
- Performance auto-tunes for mobile devices (lighter particles, capped pixel ratio)

---

## 🕹️ Controls

| Action | PC | Mobile |
|---|---|---|
| Fly (pitch/roll) | `W A S D` or Arrow Keys | Left joystick |
| Gun | `Space` | GUN button |
| Missile (hold to lock, release to fire) | `Q` | MSL button |
| Bomb | `E` | BOMB button |
| Flare | `F` | FLARE button |
| Boost / Afterburner | `Shift` | BOOST button |
| Change camera | `C` | CAM button |

---

## 🚀 Deploying to GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to `Deploy from a branch`.
4. Select the `main` branch and `/ (root)` folder, then save.
5. Your game will be live at:
   ```
   https://<your-username>.github.io/<your-repo>/air-combat-game.html
   ```

No build process, no server required — it's a static file.

---

## 📁 Project Structure

```
.
├── air-combat-game.html   # the entire game — engine, physics, UI, audio
└── README.md
```

---

## 🛠️ Tech Stack

- [Three.js](https://threejs.org/) (r128) — 3D rendering
- Vanilla JavaScript — game logic, flight model, AI, physics
- Web Audio API — synthesized engine, weapon, and explosion sound (no audio files needed)
- HTML5 Canvas — radar overlay
- CSS — HUD styling, responsive layout for mobile and desktop

---

## 🧭 Roadmap Ideas

- [ ] Multiplayer support (co-op / PvP dogfights)
- [ ] Additional aircraft with different flight characteristics
- [ ] Escort and base-defense mission modes
- [ ] Persistent leaderboard / high scores
- [ ] Weapon upgrades and loadout selection

Contributions and pull requests are welcome.

---

## 📜 License

Released under the [MIT License](./LICENSE) — free to use, modify, and share.

---

## 🙌 Credits

Built with Three.js. Terrain, clouds, aircraft, and effects are procedurally generated — no external art or audio assets required.
