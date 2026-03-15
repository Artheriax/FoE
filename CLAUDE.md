# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

---

## Project Overview

**Fragments of Eternity (FoE)** is a comprehensive worldbuilding documentation project for a fantasy RPG setting centered on **Hyperion** — a world where magic and technology fuse, power is capped by race, and rare birth traits (Gazes and Sigils) defy those limits.

This is **pure documentation** (markdown files only) — no code, build system, or tests. Common tasks involve expanding existing content, adding new characters/organizations, maintaining cross-references, and refining the world's internal consistency.

---

## Directory Structure

```
├── world/                     # World geography, history, races, dimensions
│   ├── Overview.md           # High-level worldbuilding primer
│   ├── Races.md              # All races from Higher Ones to Humans
│   ├── History.md            # Era index — links to world/history/ subfiles
│   ├── Timeline.md           # Chronological event overview across all eras
│   ├── Dimensions.md         # Realms and dimensions (Luminara, Gehenna, etc.)
│   └── history/              # Full era records
│       ├── Pre-Record.md
│       ├── Second-Era.md
│       ├── Third-Era.md
│       ├── Fourth-Era.md
│       ├── Mid-Era.md
│       ├── Fifth-Era.md
│       ├── Sixth-Era.md
│       ├── Seventh-Era.md
│       └── Modern-Era.md
├── systems/                  # Game mechanics and power systems
│   ├── Arcane.md             # Magic schools index — links to systems/arcane/ subfiles
│   ├── Gazes.md              # Gazes index — links to systems/gazes/ subfiles
│   ├── Sigils.md             # Sigils index — links to systems/sigils/ subfiles
│   ├── Power-Sources.md      # The three Sources: Vitalis, Psyche, Aeterium
│   ├── Monsters.md           # Monster classification and Essence extraction
│   ├── arcane/               # Magic school detail files
│   │   ├── Holy-Unholy.md    # Luminancy and Umbraturgy
│   │   ├── Elemental.md      # Six elemental schools + Forces
│   │   ├── Keystone.md       # Temporal, Spatial, Cosmic
│   │   ├── Echo-Enchantment.md  # Echo Magic, Enchantment, Institutional Applications
│   │   └── Forbidden.md      # All six forbidden magic schools
│   ├── gazes/                # Gaze tier detail files
│   │   ├── Standard-Gazes.md # 12 Standard Gazes with bearers
│   │   ├── Supreme-Gazes.md  # 6 Supreme Gazes with case origins
│   │   ├── Absolute-Gazes.md # 7 Absolute Gazes, all sealed/theoretical
│   │   └── Ethereal-Gazes.md # 7 Ethereal Gazes, all unconfirmed
│   └── sigils/               # Sigil tier detail files
│       ├── Standard-Sigils.md # 6 Standard Sigils + Dual Sigils section
│       ├── Supreme-Sigils.md # 4 Supreme Sigils
│       ├── Absolute-Sigils.md # 5 Absolute Sigils, all sealed
│       └── Ethereal-Sigils.md # 5 Ethereal Sigils
├── organizations/            # MOD, guilds, noble houses, and other factions
│   ├── Organizations.md      # Index and summaries
│   ├── MOD.md                # Magic Oversight Division (detailed)
│   ├── Eternal-Guard.md      # Cosmic oversight authority
│   ├── House-Dravenmore.md   # Noble research house
│   ├── Aethelgard-Consortium.md  # Largest guild
│   ├── Solaris-Vanguard.md   # Oldest guild
│   ├── Umbra-Shroud.md       # Specialized guild
│   ├── Keepers-of-Nil.md     # Immortal organization
│   └── Minor-Guilds.md       # Smaller factions
└── stories/                  # Narrative content
    ├── Characters.md         # Cast index — links to stories/characters/ subfiles
    ├── Story-Arcs.md         # Plot summaries
    ├── characters/           # Individual character profiles
    │   ├── Sersey.md
    │   ├── Artem.md
    │   ├── Thorne.md
    │   ├── Lyra.md
    │   ├── Kaelen.md
    │   ├── Rook.md
    │   ├── Nyari.md
    │   └── Gaelira.md
    ├── Serseys-Journey/      # 5-book series
    ├── Origins/              # Prequel
    ├── Nyaris-Rise-of-Fame/  # Spin-off
    └── Politics-of-Blood/    # Spin-off
```

---

## Key Architectural Concepts

### Power Hierarchy

The world operates on a **ceiling-breaking** model:

- **Base Ceiling**: Determined by race (Humans < Mortal Races < Middle Races < High Races < Celestials → Primordials → Ascendants → Eternarcs → Higher Ones)
- **Gazes & Sigils**: Rare birth traits that defy racial ceilings
- **Sources**: Three types of energy pools (Vitalis/Physical, Psyche/Mental, Aeterium/Cosmic)
- **Essences**: Harvested from monsters; power-ups for hunters

Gazes and Sigils both follow a **four-tier structure**:
- **Standard** (rarest of common)
- **Supreme** (doctrine: 3,000 bearers, 1.5k noted in Sigils)
- **Absolute** (sealed Eternal Guard records; official MOD position: "no confirmed mortal bearers")
- **Ethereal** (theoretical/unconfirmed)

### Institutional Authority

- **MOD (Magic Oversight Division)**: Absolute authority on hunters, essences, dungeon activity — ~344k active registered hunters
- **Eternal Guard**: Supersedes MOD on extinction-level threats, sealed phenomena, and forbidden research (Wall of Nihility, Entity Zero, certain forbidden magic schools)
- **Guilds**: MOD-regulated operational vehicle for hunters (Aethelgard, Solaris Vanguard, Umbra Shroud are major)
- **Keepers of Nil**: Immortal non-registered organization; oldest known survivor; closest to understanding the Wall of Nihility

### Tone & Voice

- **MOD documentation**: Bureaucratic, institutional, with sealed-file euphemisms
- **Historical records**: Formal, with cross-references and "status" annotations
- **System files (Gazes, Sigils)**: Mix of academic and bureaucratic; includes both theory and MOD regulations
- **Lore**: Mythic but grounded; mysteries are genuinely mysterious (Entity Zero, Nihility Magic)

---

## Editing Conventions

### File Naming

All files use **kebab-case with title capitalization**: `Power-Sources.md`, `Keepers-of-Nil.md`, `Book-I-Serseys-Awakening.md`.

### Markdown Formatting

- `---` (horizontal rule) separates major sections.
- Every file opens with **1-3 thematic introductory paragraphs** before diving into structured content.
- **Bold labels** for metadata fields: `**Status:**`, `**Summary:**`, `**Race:**`, `**Age:**`, etc.
- History status tags: `*[Pre-Record]`, `*[Classified]`, `*[Contested]`, `*[Speculation]*`

### Cross-Referencing

Files use two cross-reference patterns:

1. **Italic arrow format** (at section ends, pointing to related content):
   ```markdown
   *-> `systems/Gazes.md` -- Standard through Ethereal Tiers | MOD Registry Overview*
   ```

2. **Full record links** (in index files pointing to detailed files):
   ```markdown
   **Full record:** `organizations/MOD.md`
   ```

3. **Inline cross-references** in history entries:
   ```markdown
   **Cross-Reference:** `world/History.md` — The Compact Defiant; `systems/Sigils.md` — Soul Anchoring
   ```

When adding a new figure, event, or concept, **search for related cross-references** in existing files and update them. If a character appears in both History.md and Characters.md, ensure both files link to each other.

### Story File Formatting

- Written in **present tense, third person**, literary prose style.
- Chapter breakdowns use: `- **Ch. 1-3:**` or `- **Act I -- Title:**`
- Character profiles use structured fields: Race, Age, Background, Personality, Goal.

### Tables for Statistics

Use tables for population counts, classifications, and tier structures. Example (from memory):

| Metric | Count |
|--------|-------|
| Standard Gazes (1 in 100k) | ~150,000 bearers |
| Supreme Gazes (1 in 5M) | ~3,000 bearers |
| Absolute Gazes | All sealed Eternal Guard |

Keep these calibrated: if you change registry numbers, update the memory file and any dependent tables.

### Named Figures & Historical Anchoring

When adding a character or historical figure:
1. Pick an Era (Pre-Record, Second Era, Third Era, etc.)
2. Add entry to `world/history/[Era].md` with Status, Summary, Significance, Cross-Reference
3. Add full detail to relevant file (`stories/characters/[Character].md`, etc.)
4. Link both directions

### Duplication & Avoidance

If content appears in multiple files, it should be:
- **Summary here** → **full record in specialized file** (e.g., Organizations.md summarizes, MOD.md details)
- Linked via the "Full record:" pattern

Do NOT duplicate full biographical entries across multiple files unless they play distinct roles in each context.

---

## Common Editing Tasks

### Adding a New Character

1. Create full profile in `stories/characters/[Character].md` with name, race, key abilities/Gaze/Sigil
2. Add cast index row to `stories/Characters.md` (name, race, role summary, link to character file)
3. If they have a historical significance, add entry to the appropriate `world/history/[Era].md`
4. Link to the relevant tier file (e.g., `systems/gazes/Standard-Gazes.md` or `systems/sigils/Standard-Sigils.md`) if they're a notable bearer
5. Add to `organizations/[Guild].md` if they're affiliated
6. Update memory file if this is a multi-session character arc

### Adding a Historical Event

1. Determine the Era (reference `world/History.md` era index for timeline)
2. Add entry to `world/history/[Era].md` with: **Status**, **Summary**, **Significance**, **Cross-Reference**
3. Link to relevant system sub-files (if it involved a Gaze evolution, link to `systems/gazes/[Tier]-Gazes.md`; if it sealed forbidden research, link to `systems/arcane/Forbidden.md`)
4. Update any organization files if the event shaped their institutional response

### Expanding a Power System

Systems files (Gazes, Sigils, Arcane, Monsters) follow a consistent structure:

1. **Introduction** — Conceptual overview
2. **Classification Tiers** — Standard/Supreme/Absolute/Ethereal (or equivalent)
3. **MOD Registry Overview** — Population counts, regulatory framework
4. **Individual Entries** — Detailed descriptions per type
5. **Evolution/Lineage** — How abilities relate and progress
6. **Case Origins** — Historical incidents that defined the system

When expanding:
- Add named historical bearers/case origins (real consequences)
- Keep population counts consistent with memory file
- Include MOD regulatory tone (registration requirements, amplitude ratings, sealed restrictions)

### Adding an Organization

1. Create detailed file in `organizations/[Name].md`
2. Add summary to `organizations/Organizations.md` with motto, scope, and link
3. Cross-reference in relevant history events (e.g., if they responded to a crisis)
4. Link to character profiles of key figures
5. Note any institutional precedents or MOD relationships

---

## Consistency & Track Record

### Population Calibration

All population statistics are grounded in Hyperion's ~15 billion people. When adding prevalence estimates:

- Standard Gazes: 1 in 100k (~150k bearers)
- Supreme Gazes: 1 in 5M (~3k bearers)
- Standard Sigils: 1 in 250k (~60k bearers)
- Absolute tier: All sealed; official MOD claim is zero confirmed mortal bearers (technically accurate at MOD access level)

Update `memory/MEMORY.md` if these change.

### Era Timeline

Eras are referenced as Pre-Record, Second, Third, Fourth, Mid-Era (Ashenmoor), Fifth, Sixth, Seventh, Modern. If adding a new era or reshuffling timeline, document the change in memory.

### Sealed/Classified Information

Use sparingly. The pattern is:

- **MOD knows but doesn't disclose** — "sealed above Registry access"
- **Eternal Guard knows, MOD doesn't** — "sealed at Eternal Guard authority"
- **Nobody knows** — "theoretical," "unconfirmed," "scholarly debate"

When in doubt, default to "nobody knows for certain."

---

## Git Workflow

This is a documentation-only repository. Standard git practices:

- **Commit frequently**: Each logical addition (new character, expanded system section, new event) is a good commit point
- **Clear messages**: "Add [what]" (e.g., "Add Valdren Ashcrast historical overview"), "Expand [what]" (e.g., "Expand Keepers of Nil lore and references"), "Fix [issue]" (typos, broken links)
- **Cross-reference cleanup**: If you update a file, search for backtick references and verify links still point to correct sections

---

## Auto-Memory & Development Continuity

This project uses `memory/MEMORY.md` to track:

- Population calibration numbers (so population stats don't drift)
- Session-by-session enhancements (which files got major work)
- Key lineage chains (who evolved what Gaze/Sigil)
- Institutional precedents (cases that set policy)
- Unresolved questions or reserved content (e.g., Artem's Wall relationship)

When starting a session:
1. Read the memory file for context on what's been decided
2. Add new major enhancements to memory after implementing them
3. Remove or update any memory entries that turned out to be wrong

---

## Quick Reference: Important Files by Task

| Task | File(s) |
|------|---------|
| Add a character | `stories/characters/[Character].md` (profile), `stories/Characters.md` (cast index row), `world/history/[Era].md` (if historical), relevant tier file |
| Add a Gaze/Sigil type | `systems/gazes/[Tier]-Gazes.md` or `systems/sigils/[Tier]-Sigils.md`, `stories/characters/[Bearer].md` (if notable), `world/history/[Era].md` (if notable) |
| Document an event | `world/history/[Era].md` (main entry), cross-reference to systems sub-files and organizations affected |
| Expand MOD policy/rules | `organizations/MOD.md`, update relevant system files with regulatory notes |
| Add organization | `organizations/[Name].md` (new), `organizations/Organizations.md` (summary) |
| Explain power system | `systems/Power-Sources.md`, `systems/Monsters.md`, `systems/Arcane.md` |
| Clarify a mystery | `world/Dimensions.md` (for spatial mysteries), `world/history/[Era].md` (for historical), system sub-files (for power mechanics) |

---

## Known Patterns & Reserved Content

- **Entity Zero**: Source of all Cosmic power; substrate from which sources were separated; "pre-intentional" per Eternal Guard archives; all research sealed
- **Wall of Nihility**: Inverted substrate boundary; one sealed Ethereal claimant (status unknown); zero-engagement research policy enforced
- **Absolute Gazes/Sigils**: All sealed; official MOD records show zero confirmed mortal bearers; Absolute framing is that confirmed mortal bearers exist but access is above MOD level
- **Keepers of Nil**: Oldest non-registered organization; membership restricted to immortals; closest to understanding the Wall
- **Artem**: Ethereal Sigil of Transcendent Adaptation; Gazes of Null, Mimicry, and Convergence (all Ethereal; three simultaneous Gazes is an undocumented anomaly); heterochromia — Null eye permanent/unchanging, Mimicry eye shifts with active pattern; predates Hyperion; walks out of the Wall in Book V. Full character entry in `stories/characters/Artem.md`; full story in `stories/Origins/Origins.md`

---

## Git Ignore & Configuration

- `.gitattributes` is present; follows standard markdown settings
- `.vscode/settings.json` exists; no special LSP requirements for markdown

All content is committed; no sensitive data in this repository.
