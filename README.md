# Project Game Maker

**A game engine with professional power underneath and simple tools on top.**

Project Game Maker aims to be a game engine that is as capable as the big engines, but simple enough that a complete beginner can finish their first game in about an hour. Presets come first, sliders when you want more, and code only if you choose it.

> **Status:** Planning. No engine code yet. This is the best time to join and help shape it.

---

## The big idea

- **Simple on top, powerful underneath.** Every feature starts as a preset or a few clicks. Advanced options stay hidden until you click "Show more".
- **The one-hour test.** A beginner should be able to make and share a complete 2D side-scroller in about an hour. If they can't, something needs to get simpler.
- **Grows with you.** Bigger games take longer, but they add *pieces*, not complexity. Power unlocks step by step: sliders, then visual nodes, then Lua.
- **Works with what people already have.** It imports the standard files that Unity and Unreal use (FBX, glTF, OBJ, PNG, WAV and more).
- **AI-friendly.** Claude, Claude Code, Grok and other AI tools can help build games through a built-in MCP server.

## Built in versions

The full vision is huge, so it's split into versions. Each one is useful on its own, and each builds on the last. Contributors can own a version, or a feature inside one, and everything combines into one engine.

| Version | Goal | Proof it works |
|---|---|---|
| [**Version 1: 2D**](docs/version-1.md) | A complete, beginner-friendly 2D engine | A beginner finishes a 2D side-scroller in about an hour |
| [**Version 2: 3D**](docs/version-2.md) | Full 3D games: first-person, third-person, isometric | A beginner makes a small 3D adventure in a weekend |
| [**Version 3: Top-notch**](docs/version-3.md) | Modern-game graphics, big worlds, multiplayer | A small team ships a polished, modern-looking game |

## Documents

- [Architecture](docs/architecture.md): how the engine is built, layer by layer
- [Full feature list](docs/features.md): every planned feature, with the version it belongs to
- [Version 1](docs/version-1.md) · [Version 2](docs/version-2.md) · [Version 3](docs/version-3.md): what each version includes and its milestones
- [Contributing](CONTRIBUTING.md): how to help
- [AGENTS.md](AGENTS.md): guidance for AI coding assistants working on this repo

## Planned tech

- **Language:** C++ (engine core), Lua (beginner-friendly game scripting)
- **Window and input:** SDL3
- **Rendering:** bgfx to start; a modern Vulkan / DirectX 12 / Metal renderer for top-tier graphics in Version 3
- **Physics:** Box2D (2D), Jolt (3D)
- **Editor UI:** Dear ImGui
- **Audio:** miniaudio
- **Model import:** ufbx / cgltf

These choices are open to discussion. Open an issue if you'd suggest something different.

## How to help

Start with [CONTRIBUTING.md](CONTRIBUTING.md). In short: pick a version, pick a feature, open an issue to claim it, and send a pull request.

## License

[MIT](LICENSE). Anyone can use, change and build on the engine, and games made with it belong to their creators.
