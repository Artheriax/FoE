# AGENTS.md

This file provides guidance to agents when working with code in this repository.

## Project Type

This is a **documentation-only project** containing worldbuilding/lore for a fantasy RPG setting called "Fragments of Eternity" (FoE). There is **no source code** - only markdown documentation files.

## File Structure

```
FoE/
├── README.md                          # Index and navigation guide
├── AGENTS.md                          # This file
├── world/
│   ├── Overview.md                    # High-level world primer (Hyperion, MOD, cosmology)
│   ├── Races.md                       # All races, hierarchy, and detailed descriptions
│   ├── Dimensions.md                  # All realms and dimensions
│   └── History.md                     # Significant historical events, organized by Era
├── systems/
│   ├── Arcane.md                      # Magic schools, Forces, Forbidden Magic, Enchantments
│   ├── Gazes.md                       # Ocular abilities (Standard → Ethereal)
│   ├── Sigils.md                      # Physical enhancement marks (Standard → Ethereal)
│   ├── Power-Sources.md               # Vitalis, Psyche, and Aeterium (power sources)
│   └── Monsters.md                    # All monster categories and essence types
├── organizations/
│   └── Organizations.md               # MOD structure, guilds (major and minor)
└── stories/
    ├── Characters.md                  # Character profiles (Sersey and main cast)
    └── Story-Arcs.md                  # Plot summaries for all stories and spin-offs
```

## Commands

**None available.** This is a pure markdown documentation project with no build system, no tests, and no linting.

- No `npm`, `yarn`, or package manager scripts
- No build scripts or compilation
- No testing framework

## Documentation Style

- Each markdown file covers a distinct category of worldbuilding
- Files use hierarchical headings (`#`, `##`, `###`, `####`) for organization
- Section dividers (`---`) separate major sections within a file
- Bold labels (e.g., **Description:**, **Nature:**) are used for consistent field formatting
- No code blocks or programming language syntax in documentation
- Pure prose/worldbuilding content

## Important Conventions

- Cross-reference between related files (e.g., `systems/Gazes.md` links to `systems/Sigils.md` concepts)
- Maintain consistent terminology across files (e.g., "MOD" for Monster Oversight Division)
- The lore follows a consistent cosmology: Mortal Realm (Hyperion) → Spirit/Dark/Holy/Unholy realms → Divine tier
- Character stories (Sersey, Nyari, Gaelira) are in `stories/Story-Arcs.md`; character profiles are in `stories/Characters.md`
- `systems/Power-Sources.md` covers Vitalis, Psyche, and Aeterium — distinct from monster Essences (covered in `systems/Monsters.md`)
