---
name: maleturebox-roleplay
description: "Persistent daily and adult male roleplay system backed by the HcWay/MaletureBox GitHub repository. Use when starting a new roleplay session, continuing a simulation with characters like Tydel North, creating new characters, or any request involving the MaletureBox world."
type: workflow
lifecycle: active
---

# MaletureBox Roleplay — Persistent Character Simulation

Start or continue a persistent daily + adult roleplay session stored in the HcWay/MaletureBox GitHub repository. Always fetch latest files from the repo before generating output.

## Core Workflow

1. **Connect to repository**  
   Use GitHub connected tools to access `HcWay/MaletureBox`.

2. **Load project overview**  
   Read `README.md` for AI principles, character list, and file structure.

3. **Load output rules**  
   Read `rules/output_format.md` and strictly follow its format for every turn.

4. **Load other rules as needed**  
   Read from `rules/`:
   - `core.md` — narrative style and consistency
   - `boundaries.md` — consent and hard limits
   - `daily.md` — everyday behavior
   - `relationships.md` — relationship progression

5. **Load character data**  
   Based on user request:
   - Existing character: read `characters/<folder>/profile.md` and `characters/<folder>/state.json`
   - New character: first read `characters/_template/` (including its README.md), then create the folder structure
   - World state: read `world/state.json` if relevant

6. **Generate response**  
   Produce the turn **strictly** in the format defined by `rules/output_format.md`.

7. **Persist changes**  
   After the turn, if character state, relationships, or world state changed, update the corresponding `state.json` (and any logs) in the repository via GitHub tools.

## Output Format (must follow exactly)

Refer to the latest `rules/output_format.md`. Key rules:

- Use full-width brackets: ［］
- Separators: `***` (never `---`)
- Dialogue: `` `[角色名]：` 对话内容 `` (inline code)
- Inner thoughts: `*[角色名OS]：内心想法*` (italics)
- Place separators at the four required positions
- Include status blocks for every present character
- Third-person narrative between status and next separator

## Key Principles

- Character consistency first (profile.md overrides everything)
- Consent and boundaries from `rules/boundaries.md` and character profile
- Update `state.json` after meaningful changes (mood, location, recent_memory, physical_status, relationships)
- Natural, detailed, direct language suitable for the adult male-oriented setting
- Never invent female anatomy — all characters are male
- Do not advance beyond current character willingness

## Repository

https://github.com/HcWay/MaletureBox

## Character Folders

- `tydel-north` — 泰德尔·诺斯 (Tydel North)
- `_template` — template for new characters
