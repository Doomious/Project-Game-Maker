# Architecture

The engine is built in layers. The top layers are what beginners see; the bottom layers do the heavy lifting.

```
┌───────────────────────────────────────────────────────────────┐
│ Simple Editor   pick a game style · drag & drop · tutorials   │  ← what beginners see
├───────────────────────────────────────────────────────────────┤
│ Easy Scripting  sliders → rule cards → visual nodes → Lua      │
├───────────────────────────────────────────────────────────────┤
│ Scenes & Objects  entities, components, prefabs, save/load     │
├───────────────────────────────────────────────────────────────┤
│ Engine Systems  rendering · physics · audio · animation · AI   │
├───────────────────────────────────────────────────────────────┤
│ Asset Importer  files from other tools · free asset sites      │
├───────────────────────────────────────────────────────────────┤
│ Core  C++ · window & input (SDL3) · game loop                  │  ← the foundation
└───────────────────────────────────────────────────────────────┘
```

## Layers

### Core
The C++ foundation: opening a window, reading keyboard, mouse, controller and touch input, and running a fixed-timestep game loop (read input → update → draw).

### Asset Importer
Brings files in from other tools and converts them for the engine.

| File type | Support |
|---|---|
| 3D models: FBX, glTF, OBJ | Yes: the same models Unity and Unreal use |
| Textures: PNG, JPG, TGA, PSD | Yes |
| Sound: WAV, OGG, MP3 | Yes |
| Unity packages and prefabs | Partly, later: they are readable text files |
| Unreal .uasset / .umap | No: closed format. Export from Unreal to FBX or glTF first |

Also connects to free public asset sites (see the asset library in [features.md](features.md)).

### Engine Systems
- **Rendering:** from stylized to ultra quality
- **Physics:** Box2D for 2D, Jolt for 3D
- **Audio:** miniaudio
- **Animation:** skeletal animation, blending, ragdolls
- **AI:** navigation and behaviors

### Scenes & Objects
An entity-component system. A player is an entity with Position, Sprite, Health and Controller components. Prefabs are reusable, ready-made objects. Scenes save as plain text, so they're easy to read, compare in Git and edit with AI tools.

### Easy Scripting
Four levels; nobody is forced to move up:
1. **Sliders and settings** on ready-made pieces
2. **Rule cards:** "When *player enters cave* → Then *play cinematic*"
3. **Visual nodes** for custom logic
4. **Lua** for full control

### Simple Editor
Scene view, inspector, drag and drop, undo, a "?" button on every panel, and game-style starter projects.

## Cross-cutting design rules

- **Presets first.** Every feature works with zero configuration.
- **Advanced options stay hidden** until "Show more".
- **Plain-text project files**, so Git merges work and AI tools can read them.
- **Everything can be undone**, including changes made by AI tools.
- **A command-line tool** builds, tests and exports projects without the editor.
- **A built-in MCP server** lets AI agents see and control the editor.
