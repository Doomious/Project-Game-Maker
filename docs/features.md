# Full feature list

Every planned feature, grouped by area. The tag after each one shows which version it belongs to: **V1** (2D), **V2** (3D) or **V3** (top-notch). A feature tagged "V1 → V2" starts simple and grows.

## Getting started

### Game styles (one click when starting a project, switch any time)
- **2D:** side-scroller or top-down; flat camera, sprites, tilemaps, 2D physics (V1)
- **First-person:** mouse-look camera, WASD movement, jumping, crosshair (V2)
- **Third-person:** orbit camera that avoids walls, walk/run/jump animations (V2)
- **Isometric:** fixed angled camera, click-to-move, grid placement (V2)

### Grows with you
| Time | Example games | What you add |
|---|---|---|
| About an hour | 2D side-scroller, simple puzzle game | Ready-made pieces and sliders |
| A weekend | Top-down adventure, 3D platformer | Visual scripting for your own rules |
| A few weeks | Third-person action, isometric RPG | Inventory, quests, dialogue, saving |
| A few months | Open worlds, online multiplayer | Lua scripting and pro tools |

Rules: bigger games add pieces, not complexity. Power unlocks step by step. Advanced options stay hidden until "Show more".

## Assets

### Importing (V1 → V2)
FBX, glTF, OBJ, PNG, JPG, TGA, PSD, WAV, OGG, MP3. Unity packages partly (V3). Unreal .uasset is not supported: export to FBX or glTF first.

### Free asset library (V1 → V3)
Search public asset sites inside the editor, preview with the license shown, drag in, and credits are saved automatically. A "free for anything" (CC0) filter is on by default.

| Site | What you get | License |
|---|---|---|
| Poly Haven | 3D models, textures, sky lighting | CC0 |
| ambientCG | Materials and textures | CC0 |
| Kenney | Game-ready 2D and 3D packs, UI, sounds | CC0 |
| Quaternius | Low-poly characters and props | CC0 |
| Sketchfab | Huge library of 3D models | Varies, often needs credit |
| Freesound | Sound effects | Varies |
| OpenGameArt | Sprites, music, models | Varies |

Each site's terms for automated downloading need checking before building its integration.

## Characters and animation

### Easy bones / rigging (V2)
1. Pick a body type: human, four-legged animal, bird, custom
2. Drag a few markers onto the chin, wrists, elbows and knees
3. Auto-rig: the engine builds the bones and the skin weights
4. Test poses, then add ready-made walk, run and jump animations

Imported rigged models keep their bones. Advanced users can edit bones by hand.

### Character creator (V3)
- Bases: human, elf, orc, robot, creature; sliders for height, build, face and age; hair, skin, eyes, scars, tattoos; clothes and armor that fit any body
- For your game: design heroes and NPCs, save as presets
- For your players: tick "Character creation screen"; you choose which sliders players get
- Import: rigged FBX/glTF, VRM (for example VRoid Studio), MakeHuman, Blender

### Animation extras (V2)
Ragdolls, feet that land on slopes and stairs, smooth blending between moves.

## Building worlds

### Terrain builder (V2)
Start from a preset (field, hills, island, mountains, desert, snow) → sculpt with brushes → paint the ground (slopes turn rocky automatically) → spray trees, grass and rocks; draw rivers, lakes and paths.

### Building builder (V2)
Draw the floor plan on a grid → drag on doors, windows and stairs → pick a style (cabin, castle, modern, sci-fi) and the roof builds itself → add floors and furniture.

### Water (V2, advanced flow V3)
- **Lake or pond:** click a dip in the terrain; drag the handle to set the level
- **Ocean:** tick "Ocean" in world settings; calm-to-stormy slider
- **River:** draw a line from high to low; it carves its bed and flows downhill
- **Waterfall:** appears wherever a river runs over a cliff
- **Pool or puddle:** drag a box into any building or hollow
- Physics: floating and sinking by weight, swimming and diving with a breath meter, currents, boats and rafts, splashes and ripples
- Looks: clear, tropical, murky swamp, icy; colour and clarity sliders
- Advanced, off by default: flowing water that pours and fills containers (V3)

### Weather (V2)
- Presets with strength sliders: sunny, cloudy, rain, snow, fog, wind
- Weather mixes that change over time, day and night cycle, climate zones
- The world reacts: puddles, snow piles up, trees sway, water gets choppy
- Optional gameplay effects: fog shortens view, rain makes ground slippery, NPCs head indoors

### Lighting and textures (V2)
- Lighting: mood presets, drag-in lights, follows time of day and weather, "Too dark?" and soft-shadow fix-it buttons
- Materials: presets, sliders (colour, shininess, roughness, wear, wetness), tiling, material from a photo
- Live preview and before/after view

### Graphics quality (V1 → V3)
Stylized (V1/V2) → Standard (V2) → High (V3) → Ultra / Cinematic (V3). Creators pick one look; players' games auto-detect the best setting; upscaling (DLSS, FSR); fine-tune under "Show more".

## Gameplay

### Collisions (V1 → V2)
- Automatic collision shapes; solid, trigger or ignore
- "Who hits whom" grid of tick boxes (player, enemy, bullet, pickup, world)
- Cause and effect: damage, knockback, bounce, break or shatter, stick, sound, sparks and dust, bullet holes and scorch marks, camera shake, destroy, start a rule
- Material-aware effects (V2)

### Triggers and behaviors (V1 → V2)
- **Rule cards:** When (enter area, pick up item, enemy defeated, timer, low health, night falls) → Then (play cinematic or sound, spawn enemies, open door, start quest, show message, save checkpoint, change weather or music)
- **Enemy behavior:** patrol, guard, hunt, ambush, sniper; sliders for aggression, courage, sight and hearing; take cover, call for help, flee, search
- **Friendly behavior:** villager, guard, merchant, companion, animal; daily schedules; greet, run from danger, follow, help in fights
- Any rule or behavior opens as visual nodes, then Lua

### NPC interaction (V2)
Click any character → "Make it a…" talker, quest giver, shopkeeper, companion, or enemy/target. Roles mix. NPCs remember player choices; quests update automatically.

### Weapons and armor (V2)
- Guns, melee, bows and throwing, shields, magic and sci-fi, armor
- Import or pick a model → pick its type → drag the grip point → tune with sliders
- Works with any character, first- and third-person; enemies use the same weapons

### Core systems
- Health, damage, lives, checkpoints, game over (V1)
- Saving and loading: slots (V1), autosave and cloud saves (V2)
- Progression: XP, levels, skill trees, stats (V2)
- Loot, crafting and economy (V2)
- Vehicles and mounts (V2)

## Look, sound and feel
- Particle effects: 2D basics (V1), full 3D presets (V2)
- Audio: sound and music (V1); adaptive music, 3D sound, ambient zones, mixer (V2)
- Camera tools: shake, zoom, follow, photo mode (V2)

## Interface

### Custom user interface (V1 → V2)
- Ready-made screens: HUD, main menu, pause and settings (V1); inventory, dialogue, map and quest log (V2)
- Pick a screen → drag in pieces → connect with dropdowns (no code) → pick a theme
- Resizes for any screen; mouse, controller and touch; live preview

### Menus, intros and labels (V1 → V2)
- Custom menus: drag-and-drop pages, linked pages, live/video/image backgrounds, transitions, menu music
- Custom intros: splash screens (V1), timeline intros and cinematic openings (V2), skip button
- Custom labels: rename everything, name tags, item names, signs, damage numbers, tooltips, own fonts; labels translate automatically

### Custom controls (V1 → V2)
- Action table: name an action, assign keyboard/mouse, controller and touch inputs
- Press, hold, double-tap, combos; sensitivity, dead zones, invert look, vibration; per-mode controls (walking, driving, flying); correct button icons per device
- Players adjust their own controls on every platform: PC (rebind keys), console (remap buttons and sticks), phone (move, resize and remap touch buttons)

## Cinematics and video (V2)
Place cameras or record a path → timeline (characters, cameras, lights, music, subtitles) → play in-game as a cutscene, or render MP4/MOV/image frames up to 4K.

## Behind the scenes
- AI navigation (V2)
- Controls on every device (V1 → V2)
- Big worlds that load in pieces (V3)
- Performance helper (V2)

## Sharing your game

### One-click export
Pick platforms → health check → click Build → share (ready-to-play file, itch.io, Steam).
- Windows, Mac, Linux, Web (V1)
- Android, iOS (V2): need a Mac and an Apple developer account for iOS
- Consoles (V3): need approval from each company

### Players and publishing
- Accessibility (V1 basics → V2)
- Translations (V2)
- Achievements and leaderboards (V3)
- Online multiplayer (V3)
- Modding support (V3)

## Help and learning
- "?" button on every panel, step-by-step walkthroughs, hover tips, learn-by-building mini-projects, a stuck helper
- One tutorial per area: first side-scroller in an hour, game styles, importing and licenses, bones and animation, physics, scripting, cinematics, export, NPCs

## For creators
- Backups and version history (V1)
- Team collaboration (V3)

## AI agent support (V1 → V3)
- Built-in **MCP server** (local and over the web), so Claude, Claude Code, Grok and other MCP-compatible tools can connect
- AIs can build scenes, write and fix scripts, take screenshots, play-test, export, import assets and set up animations
- Every AI change is undoable; big actions need approval
- Plain-text project files, a command-line tool, and an AGENTS.md guide in every project
