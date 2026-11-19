# Version 2: 3D

**Goal:** full 3D games: first-person, third-person and isometric, still simple to make.

**Proof it works:** a beginner makes a small 3D adventure (a village, a quest, a few enemies) in a weekend.

Builds on everything in [Version 1](version-1.md).

## What's included

### Graphics
- 3D renderer at **Stylized** and **Standard** quality: realistic materials, soft shadows, good lighting
- **Lighting:** mood presets (golden hour, spooky night, neon city), drag-in lights, "Too dark?" fix-it button
- **Materials:** presets (wood, metal, stone, glass), sliders for colour, shininess, roughness and wear, texture tiling, material from a photo
- 3D particle effects: fire, smoke, explosions, magic
- Camera tools: shake, zoom, follow, photo mode

### Game styles
- **First-person:** mouse-look, WASD, crosshair
- **Third-person:** orbit camera that avoids walls
- **Isometric:** angled camera, click-to-move, grid placement

### Import
- 3D models: FBX, glTF, OBJ, with their bones and animations

### Characters and animation
- **Easy bones (auto-rig):** pick a body type → drag a few markers → bones built automatically → test poses
- Ready-made walk, run and jump animations
- Animation blending, feet that land on slopes and stairs, ragdolls

### World building
- **Terrain builder:** presets, sculpt brushes, ground painting, spray trees, grass and rocks
- **Building builder:** draw a floor plan, drag on doors and windows, pick a style, the roof builds itself
- **Water:** click a dip to make a lake, draw a river, tick "Ocean"; floating and sinking, swimming and diving, currents, boats
- **Weather:** sunny, cloudy, rain, snow, fog, wind; weather mixes, day and night, climate zones; the world reacts

### Gameplay
- 3D physics with Jolt
- **NPCs:** "Make it a…" talker, quest giver, shopkeeper, companion, enemy or target
- Dialogue with choices; quests that update automatically
- Enemy behaviors (patrol, guard, hunt, ambush) and friendly behaviors (daily schedules, run from danger)
- AI navigation around obstacles
- **Weapons and armor:** guns, melee, bows, shields, magic, armor; set the grip point, tune with sliders
- Inventory, loot, crafting, shops and currency
- Progression: XP, levels, skill trees, stats
- Vehicles and mounts: cars, bikes, horses, boats
- Material-aware collision effects: metal sparks, wood splinters, water splashes

### Scripting
- **Visual nodes** for custom logic
- **Lua** for full control

### Cinematics
- Place cameras, record camera paths, timeline with keyframes
- Play in-game as a cutscene, or render to MP4/MOV up to 4K

### Interface
- Ready-made inventory, dialogue box, map and quest log screens
- Custom intros built on a timeline

### Sharing and players
- Export to Android and iOS
- Touch controls players can move and resize
- Accessibility: subtitles, colourblind modes, difficulty options
- Translations

### Help
- Tutorials for every Version 2 feature
- Performance helper: says in plain English what's slowing the game down
