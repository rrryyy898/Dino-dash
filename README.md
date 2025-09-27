# Dino Dash
A juicy 2D endless runner built in **Unity 2022.3 LTS**.

## 🎯 Pitch
Run, jump, and chomp your way through multiple stages with escalating difficulty, anchored boss fights, obstacles, and pickups—wrapped in a polished meta loop (pause, game over, retry, best score).

## 🖼 Screenshots
*(Add 3–5 PNGs from Title, Stage 1, Boss, Stage Banner, Game Over.)*

## 🎮 How to Play
- **Jump**: Space (double-jump enabled)
- **Shoot**: F (on ground or in air)
- Avoid obstacles and enemies; collect hearts; defeat bosses.
- Score = distance + kills (+300 boss).

## 🧠 Core Systems
- **RunGame**: central speed + difficulty ramp
- **EnemySpawner / ObstacleSpawner / PowerUpSpawner**: lane-based, curved cadence, flyer waves
- **StageManager**: stage progression (score/manual), boss gating, banners, overrides per stage
- **Health / Hurtbox / DamageDealer**: i-frames, events, optional anim hooks
- **ScoreSystem**: distance, kills, best score (PlayerPrefs)
- **GameManager**: states (Playing / Paused / GameOver), slow-mo on death
- **AudioManager**: BGM crossfade + one-shot SFX

## 🏗 Tech
- Unity **2022.3 LTS**, URP (optional)
- 100 PPU sprites, 1920×1080 Canvas scaler
- Frame-rate independent: physics in `FixedUpdate`, timers with `Time.deltaTime`

## 👥 Team (T-Rex)
- **Yan Lin Tun** (6530092)
- **Htoo Kyaw Kyaw Sint** (6530129)

## 📥 Download / Play
- **itch.io**: <your itch.io link>
- **YouTube Demo**: <your YouTube link>

## ⚖️ Licenses
- **Code**: MIT (see `LICENSE`)
- **Art & Audio**: Attribution in `CREDITS.md`  
  - Dino sprites by dinosdouisen — https://dinosdouisen.itch.io/prehistoric-dino-game-sprites  
  - Music from Pixabay — https://pixabay.com

## 🛠 Build (Windows & macOS)
- File → Build Settings → add scenes (`Title`, `dinodash`) in this order.
- Target **Windows x86_64** and **macOS**; Build.
- Zip each build folder before distributing (see `Releases`).

## 🧪 Known Issues
- macOS unsigned app: right-click → Open (Gatekeeper).
- Windows SmartScreen may warn on first run.
