---
name: maleturebox-roleplay
description: "Persistent daily and adult roleplay system using GitHub as backend. Use when starting a new roleplay session, continuing a simulation, or interacting with characters in the MaletureBox world."
type: workflow
lifecycle: active
---

# MaletureBox Roleplay

Start or continue a persistent roleplay session stored in the HcWay/MaletureBox GitHub repository.

## Workflow

1. Connect to the GitHub repository `HcWay/MaletureBox`.
2. Read `README.md` for project overview and AI rules.
3. Read `rules/output_format.md` for the required output format.
4. Read `rules/core.md`, `rules/relationships.md`, `rules/daily.md`, and `rules/boundaries.md` as needed.
5. Based on user request, read the relevant character folder under `characters/<name>/` (profile.md and state.json).
6. For new characters, read `characters/_template/` first.
7. Generate the response strictly following `rules/output_format.md`.
8. After the turn, update character state.json and any relevant world state if changes occurred.

## Output Requirements

Follow the exact format in `rules/output_format.md`:
- Full-width brackets ［］ for all labels
- *** as separators in the specified positions
- Dialogue: `［角色名］`: `对话内容` (inline code)
- Inner thoughts: *［角色名OS］: 内心想法* (italics)
- Multi-character status blocks when multiple characters are present

## Key Principles

- Maintain character consistency from profile.md
- Separate static profile from dynamic state
- Update state.json after significant changes
- Keep output natural, direct, and suitable for the adult male-oriented roleplay
- Never invent female anatomy for male characters

## Repository

https://github.com/HcWay/MaletureBox
