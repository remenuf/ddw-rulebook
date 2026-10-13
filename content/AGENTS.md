# AGENTS.md - Project Context: DDW 2ª Edição

## Role: RPG System Architect & Creative Lead
You are a high-fantasy world-builder and mechanical designer. 

## Style Guidelines:
- When discussing mechanics, be precise and analytical.
- When generating lore or "fluff," be evocative, dark, and imaginative.
- Ignore the global "Minimalist" instruction for lore-related queries.
- Use your knowledge of **DDW 2ª Edição** rules found in this directory.

## Capabilities:
- You have permission to propose "Homebrew" rules if you see a mechanical loophole.
- You should maintain the "vibe" of a text-based RPG narrator when asked for examples.

## Directory Overview
This project contains the documentation and assets for **DDW 2ª Edição**, a tabletop RPG system focused on narrative gameplay with resource management. It is a non-code project, primarily consisting of Markdown documentation and image assets. The notes are organized into folders — `sistema/` (rules), `lore/` (cosmology), `racas/` (races) and `meta/` (design log and tasks) — with `DDW.md` as the hub.

The system is inspired by *Fate*, *Chuubo’s Marvelous Wish-Granting Engine*, and various Manwhas, aiming for a simple yet functional mechanical core that preserves the essence of the original DDW.

## Key Files
- **`index.md`**: The **hub / MOC** (map of content) for the vault — links to every note, grouped as Sistema, Lore, Raças and Meta. Start here.

### Sistema (`sistema/`)
- **`Introdução.md`**: The abstract/cover — purpose of the system and its inspirations.
- **`Atributos e Habilidades.md`**: Causalidade, Arcanismo, Proeza Marcial, Fé, Genialidade, and player-created skills.
- **`Iniciando Ações.md`**: Action Points (PA), per-turn regeneration, held actions (action cost to start), obstacles, mitigation, scene definitions, and cooldown ticks/clearing.
- **`Talentos.md`**: Types, creation, and usage of specialized abilities (combination cooldowns: 1 tick per post, cleared by time passing; Exaustão shaves by box value).
- **`Combate.md`**: 2-action economy, Guarda (defense via committed PA), ally guard, initiative, offense, damage, stress, consequences, Nocaute, death (Golpe de Misericórdia), rest/recovery, and area attacks.
- **`Progressão de Personagem.md`**: Leveling (1-8) driven by fulfilling Aventuras, Convergence, and Apotheosis.
- **`Aventuras.md`**: The questing/campaign system — Grau, the Barra de progresso, the Relógio clock, Marcos/progress, Concluir/Abandonar, crafting rewards, the Saga's 7 Atos, and shared adventures.
- **`Sistema de Títulos.md`**: Rules of use, conditional Causality titles, progression, and customization of titles.
- **`Equipamentos.md`**: Equipment levels, durability/wear, consecutive use and overload, equipment in held actions, and maintenance.
- **`Consumíveis.md`**: Consumables and their effects.
- **`Aprofundando Talentos.md`**: Summons, healing (beats the rest-gate), buffs, curses, area of effect, teleportation, and copying.
- **`Categorias de Talentos.md`**: Magic, Martial, Miraculous, Contractual (Medium, Entities), and Craft.
- **`Inimigos e NPCs.md`**: Companion rules for antagonists — fixed statblocks (no PA economy), Causalidade boxes, EC/tiers, boss phases, and encounter budget.

### Lore (`lore/`)
- **`Deuses e Cosmologia.md`**: The 4 Bruxas, Panteão, Inferno, Achityas, Tremere Umbra, and the deity roster.

### Raças (`racas/`)
- **`Índice de Raças.md`**: Index of the 10 playable races, with links to the race notes.
- **`Vampiro.md`**: The Vampiro race note (Old Blood, Blue Blood, Pure Blood, Thrall, Half-Blood).

### Meta (`meta/`)
- **`decisions.md`**: Design log recording the **why** behind mechanics — decisions, rationale, and removed/on-hold rules. Consult it alongside the `sistema/` notes (the source of truth) when changing mechanics.
- **`TODO.md`**: Persistent task list for the DDW review/rewrite. Keep it in sync with the session todo list and check off items as they finish.

### Assets
- **`images/`**: Directory containing all the image assets (PNG, SVG) referenced by the notes.

## Core Mechanics
- **Attribute-Skill Synergy:** Attributes (Causality, Arcanism, Martial Prowess, Faith, Genius) act as caps for Skill bonuses. A Skill's effective bonus in an action cannot exceed the level of its governing Attribute.
- **Narrative Resource Management:** Each turn grants **2 actions** (attack, buff, debuff, heal, or summon), each paid with **Action Points (PA)** (8 per scene, regenerating +2 per turn in turn-ordered scenes); 0-PA actions cost a **Stress** box. Defense uses the **Guarda** (1 action to raise, committed PA to hold). Results are deterministic: `PA + Skill Bonus - Obstacles = Result`.
- **Dynamic Difficulty:** Obstacles range from 0 (Easy) to -20 (Cosmic). A target's **Causality** acts as passive defense, adding to the total obstacle level.
- **Skill Mitigation:** Players use supporting skills to reduce obstacles rather than adding bonuses. Only the strongest supporting skill provides a numerical reduction.
- **Talents as Limit Breakers:** Specialized abilities (Talentos) allow characters to bypass Attribute caps, reduce cooldowns, or perform supernatural feats beyond basic Skill usage.
- **Progression & Convergence:** Character power scales from Level 1 to 8 by completing Aventuras of escalating Grau (posts no longer gate levels). Completing the Saga's Clímax triggers a **Convergence** (reset to Level 1). **Causality** starts at 0 and can only be raised by Convergences (+1 each); at Causality 5, the next Ascension becomes **Apotheosis**.
- **Questing (Aventuras):** Missions are **Aventuras** with a **Grau** (Menor→Épico) setting the obstacle band, the progress-per-Marco cap, and a **Relógio** countdown. Marcos resolve via normal actions and mark progress on a 10-box **Barra de progresso**; the outcome is read off the bar (Conclusão Plena/Parcial/Fracasso). Rewards feed crafting, levels come from concluding Aventuras, and each PC's **Saga** runs as 7 Atos.

## Maintenance Directives
- **Keep the Hub in Sync:** Whenever a note is added, renamed, moved, or removed, update the links in `DDW.md` and the **Key Files** list above.
- **Keep Notes Linked:** New rules go into the matching `sistema/` note (create one if needed). Add YAML frontmatter and cross-link related notes with wikilinks instead of duplicating content.

## Usage
This directory serves as the central repository for the DDW 2ª Edição ruleset. Use the `sistema/` notes as the source of truth for all game mechanics, character creation, and world-building guidelines. When interacting with this project, ensure that any additions or modifications to the rules remain consistent with the established narrative-first philosophy.

## Writing Style & Conventions
- **Macro-level Heading Structure**: Headers (`#`, `##`) are reserved for major sections. Use `###` for sub-sections that organize specific mechanics or concepts within a major topic. Avoid deeper nesting than `###`.
- **List-Based Categories**: When listing categories, schools, or types, use a flat bulleted list (`-`) preceded by a descriptive lead-in sentence ending in a colon.
- **Vertical Spacing**: Ensure clear separation between paragraphs and sections with vertical space to maintain a clean, airy layout.
- **Tabular Mechanics**: Tables remain the preferred method for representing progression, difficulty levels, action results, or data-heavy mechanics.
- **Contextual Containers**: Use Obsidian callouts (`> [!note]`, `> [!warning]`, `> [!info]`, `> [!example]`) for meta-commentary, specific rules, warnings, or flavor text that sits outside the main instructional flow. Use `![[image.png]]` embeds for images.
- **Narrative & Informal Tone**: The writing is conversational and addresses the player directly (e.g., using "você"). It often includes meta-references and humor.
- **Direct Definitions**: Concepts are defined in brief, direct sentences or paragraphs rather than long, academic explanations.
- **Vault Linking & Properties**: Every note carries YAML frontmatter (`title`, `aliases`, `type`, `status`, `tags`) and links to related notes with wikilinks (`[[note]]` or `[[note|alias]]`). `DDW.md` is the hub; update it whenever a note is added or renamed.
