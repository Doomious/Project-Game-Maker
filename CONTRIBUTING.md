# Contributing to Project Game Maker

Thanks for helping! This project is in the planning stage, so every contribution shapes what the engine becomes.

## How the work is split

The engine is built in three versions:

- [Version 1: 2D](docs/version-1.md): **start here.** Everything else builds on it.
- [Version 2: 3D](docs/version-2.md)
- [Version 3: Top-notch](docs/version-3.md)

You can help with a whole version or a single feature inside one. Features can be built in parallel as long as they follow the [architecture](docs/architecture.md), so separate pieces combine into one engine later.

## How to help

1. **Pick something.** Browse the version docs or the [full feature list](docs/features.md).
2. **Claim it.** Open an issue titled with the version and feature, for example `[V1] Tile brush`, and say you're working on it. This stops two people building the same thing.
3. **Discuss the approach** in the issue before writing lots of code, especially for anything touching the core.
4. **Branch.** Work on a branch named like `v1/tile-brush`.
5. **Pull request.** Open a PR that links the issue. Keep PRs small and focused.

Not a programmer? Help is still very welcome: design ideas, UI mockups, tutorials, testing with beginners, art for the starter kits, and documentation.

## Ground rules for every feature

These keep the engine simple, however big it gets:

- **Presets first.** A feature must work with zero setup.
- **Hide advanced options** behind "Show more".
- **Plain English** in every label and message. No jargon.
- **Everything undoable.**
- **Plain-text files** for scenes and settings, so Git merges work.
- **Add a tutorial** (or a tutorial outline) for any new user-facing feature.
- **The one-hour test:** nothing may make the 2D side-scroller harder for a beginner.

## Code style (once code exists)

- C++20, formatted with clang-format (config to come)
- Lua for game scripting
- CMake build
- Small, well-named functions; comments explain *why*, not *what*

## Licensing

By contributing, you agree your work is released under the project's [MIT License](LICENSE). Only add third-party code or assets whose license allows it, and note the source and license in your PR.
