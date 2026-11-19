# Version 1: 2D

**Goal:** a complete, beginner-friendly 2D engine.

**Proof it works:** a beginner finishes a 2D side-scroller in about an hour.

## The one-hour side-scroller

| Time | What the beginner does |
|---|---|
| 0–5 min | Pick "2D side-scroller": player, camera and controls are ready |
| 5–15 min | Paint the level with a tile brush and a free art pack |
| 15–25 min | Drag in ready-made coins, spikes and enemies that already work |
| 25–40 min | Tune jump height, speed and enemies with sliders, no code |
| 40–50 min | Add music, sounds, a start screen and a win screen |
| 50–60 min | Play-test, then one-click export and share |

Every Version 1 feature exists to make this hour possible.

## What's included

### Foundations
- C++ core with SDL3: window, input, fixed-timestep game loop
- 2D renderer: sprites, tilemaps, camera, layers
- Entity-component system, prefabs, scenes saved as plain text

### Editor
- Scene view, inspector, drag and drop, undo/redo
- Game styles: **2D side-scroller** and **2D top-down**
- Tile brush for painting levels
- Backups and version history: every change saved, rewind any time

### Gameplay
- **Ready-made pieces** with built-in behavior: player, coins, spikes, enemies, doors, checkpoints, moving platforms
- Sliders for jump height, speed, gravity, enemy speed and so on
- **Collisions:** automatic shapes; solid / trigger / ignore; a "who hits whom" grid; simple effects (damage, bounce, collect, destroy, sound)
- Health, damage, lives, checkpoints and a game-over screen
- Save and load with save slots
- **Rule cards** (When → Then): enter area, pick up item, enemy defeated, timer → play sound, open door, show message, spawn enemies
- Simple enemy behaviors: patrol, chase, guard
- Basic 2D particle effects: dust, sparks, coin sparkle

### Interface, sound and controls
- Ready-made HUD, main menu, pause and settings screens
- Drag-and-drop UI builder, themes, custom labels and fonts
- Custom intros: splash screen with your logo
- Sound effects and music
- Custom controls: keyboard, mouse and controller; players can rebind keys

### Assets
- Import PNG, JPG, WAV, OGG
- Free asset library (first sources: Kenney and other CC0 sites), with automatic credits

### Sharing
- One-click export: Windows, Mac, Linux, Web
- Health check before building (missing files, errors)

### Help and AI
- Tutorial: "Your first 2D side-scroller in about an hour"
- "?" button on every panel, hover tips
- Basic MCP server, plain-text project files and a command-line build tool, so AI tools can help from day one

## Milestones

1. **Foundations:** window, game loop, input
2. **2D graphics:** sprites, tilemaps, camera
3. **Objects and collisions:** ECS, Box2D, the "who hits whom" grid
4. **The editor:** scene view, inspector, drag and drop, undo
5. **Ready-made pieces and sliders:** the side-scroller starter kit
6. **Rule cards, UI and sound**
7. **Export:** Windows, Mac, Linux, Web
8. **The one-hour test:** watch real beginners try it and fix what slows them down
