# AGENTS.md

Guidance for AI coding assistants (Claude Code, Grok Build and others) working on this repository.

## What this project is

Project Game Maker is a planned game engine: professional power underneath, simple tools on top. Read [README.md](README.md) and [docs/architecture.md](docs/architecture.md) first.

## Current state

Planning only: there is no engine code yet. Work is organised into [Version 1](docs/version-1.md) (2D), [Version 2](docs/version-2.md) (3D) and [Version 3](docs/version-3.md) (top-notch). Version 1 comes first.

## Rules

- Follow the ground rules in [CONTRIBUTING.md](CONTRIBUTING.md): presets first, advanced options hidden, plain English, everything undoable, plain-text files.
- Planned stack: C++20, CMake, SDL3, bgfx, Box2D, Jolt, Dear ImGui, miniaudio, Lua. Ask before adding other dependencies.
- Keep changes small and tied to one issue.
- Never make the one-hour 2D side-scroller harder for a beginner.
- Only add third-party code or assets with compatible licenses, and record their source.
