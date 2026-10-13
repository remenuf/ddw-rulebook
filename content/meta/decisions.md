---
title: Development Decisions
aliases:
  - Decisões
  - Design Log
type: meta
status: ativo
tags:
  - ddw
  - meta
---

# Development Decisions — DDW 2ª Edição

Design log for the mechanics in the `sistema/` notes. The rules notes are the **source of truth**; this file records the **why** and the history behind each decision. Newest decisions are appended in their relevant section.

## Difficulty Convention (Obstacles)

- Canonical model: negative obstacles are **subtracted** — `Resultado = PA + Habilidade/Talento + Obstáculo` (the Obstáculo is a negative number).
- Conversion for read-aloud target numbers: `Alvo = 2 + |Obstáculo|`.
- Teleporte tiers: `−2 … −18`.
- Rationale: one consistent formula across the book; removes sign confusion.

## Action Points (PA) & Committed PA

- Pool: **8 PA per scene**.
- Regeneration: **+2/turn**, only in turn-ordered (combat) scenes.
- Cost ladder: `0 / 1 / 2 / 4 / 8`.
- Removed the old "recover half on completion" clause.
- Held actions use **committed PA** (`máximo − comprometidos` ceiling); committed PA does **not** regenerate while held, is **not refunded on release**, and the ceiling refills on scene change.
- No attribute cap on PA. `turno = post`.

## Causalidade (Causality)

- Starts at **0**; raised **only** by Convergences (+1 each).
- Not purchasable at creation, nor with the Level 4 / Level 8 attribute points (text reads "exceto Causalidade").
- **Apoteose** at Causalidade 5.
- Rationale: rewards long-lived characters; being offline for Levels 1–8 is intentional.

## Conditional Causality Titles

- Situational bonus active while the title is equipped **and** its narrative condition holds.
- **Fixed +1, no scaling**; does not count as progression and adds nothing toward Apoteose; counts for all Causalidade uses.
- Examples: *Clérigo Sagrado*, *Protetor dos Inocentes*, *Soberano*, *Guardião do Posto*.

## Knockout, Death & Recovery

- **Nocaute** = *indefeso* (cannot act or defend; attacks ignore Defesa). Lasts until healed or a **Descanso Curto**; waking clears Estresse but keeps Consequências.
- Death only via **Golpe de Misericórdia** (a deliberate attack on an indefeso target) or an explicit story effect — never from a single hit or bad luck.
- **Última Resistência**: a PC facing a Golpe de Misericórdia gets one last desperate action; death remains possible but never arbitrary.
- **Tom da Mesa** callout: *Heroico* / **Sombrio (default)** / *Brutal*; always telegraph lethality.
- **Descanso Curto** (end-of-scene pause): clears Estresse, wakes the downed, heals Leve. **Descanso Longo** (between adventures): also heals Média. **Grave** requires a dedicated healing adventure.
- **Estresse is rest-gated, not scene-gated**: chained scenes with no rest (combat → chase → combat) carry Estresse across all of them.
- Consequence table recovery column rewritten to named rests.

## Action Economy, Guarda & Initiative

- **2 ações/turno** (attack, buff, debuff, heal, summon).
- Each action paid with PA: `(PA ou Equipamento) + Habilidade ou Talento`; a **0-PA** action costs a Stress box.
- **Held ações**: 1 ação to start + committed PA; maintenance costs PA only (no ação); release frees PA.
- **Defesa = Guarda**: a held stance, **1 ação to raise**, committed PA to hold, defends against **all** attacks. Without Guarda you only have **Defesa Passiva (Causalidade)**.
- **No core reaction mechanic** — reactive / last-second defense is Talent-only.
- **Defender um Aliado (Guarda Compartilhada)**: the Guarda always covers you; extend it to **one ally** (1 ação, same value/PA); overflow hits the attacked ally; protecting more than one ally, or at range, needs Talents.
- `Postura` renamed to **Guarda**.
- **Iniciativa**: players' side first, in free/agreed order; enemies ordered by **Talento → Habilidade → Causalidade → valor da Habilidade → dado**; ambush inverts by narrative.

## Equipment & Held Actions (Durability)

- Equipment substitutes PA: `Nível do Equipamento + (Habilidade ou Talento)`; Durabilidade Máx = `Nível × 2`.
- Durability loss = **Dificuldade Final** of the action; consecutive use without a PA interval doubles (×2, ×4…).
- Magic items get a per-scene durability shield equal to the user's **Arcanismo**.
- **Equipment in held ações**: holding drains durability every turn — common holds lose, per turn, durability = final difficulty; a **Guarda** wears **on impact** (durability = the difficulty of each blocked attack). Both are **linear** and exempt from the overload multiplier.
- Principle: **PA sustains (points locked), gear bursts or pinch-blocks (item wears)**. Gritty by choice — a shield is a save, not a wall.

## Consequences — Overflow Severity (B2)

- The player chooses which Stress boxes to burn; **overflow = the leftover**, and severity derives from it.
- Bands: **Leve** ≤2, **Média** ≤4, **Grave** ≤6.
- **Overflow carries**: each 6 points fill a Grave, then the remainder follows the bands — 7–8 → Grave + Leve; 9–10 → Grave + Média; 11–12 → Grave + Grave; **13+** fills all three slots → **Nocaute**.

## Area Attacks (C1)

- Marking a Stress box is the **surcharge for hitting multiple targets**, paid even on a miss or with no valid targets.
- The Attribute is added as part of the area compute and divided among targets whose Causalidade is ≥ the attacker's.
- With no Stress boxes left, the **Regra Global de Custos** applies (take a Consequência, then Nocaute).

## Cooldown, Scenes & Recovery (#8)

- **Cooldown = PA spent (min 1), measured in turns.** A **turn = a post**, in *any* scene (including free roleplay); cooldown ticks **−1 per post**.
- **Passage of time** (scene change, travel, waiting) **clears remaining cooldowns** — cooldown is, in practice, a scene-level limiter.
- **Exaustão** = marking a Stress box to shave the cooldown by its value (the `[2]` box clears 2 turns, the `[1]` box clears 1).
- **Held ações across scenes** are narrative-dependent (DM decides): buffs, transforms, construts and the Guarda tend to persist; instant effects end.
- **Cura beats the rest-gate**: it can restore Estresse whenever there's a pause to act (even between emended scenes) — it's paid magic, not automatic recovery.
- **Consumíveis**: the `Proeza Marcial + 1` per-scene limit resets **per scene** (kept simple — game over realism).

## Removed — Conceder o Golpe

- **Removed (on hold).** The mechanic let a defender drop the Guarda to gain PA, but its reward was ill-defined: it scaled with enemy damage, and there was no sensible refund when the Guarda was equipment-based.
- Cut for now; the free "lower your Guarda" already covers the intent. Revisit only if it earns a **distinct** trade.

## Aventuras (Questing / Missões)

- New note `sistema/Aventuras.md`, introducing **Aventuras** — the adventure/campaign layer for DDW's diceless core. Rationale: the system already leveled by "objectives/missions" without defining them, and the crafting notes referenced "Missões" and "Grandes Feitos" with no source of materials.
- **Generic term: Aventura.** One engine, six faction skins — Aventureiros *Missão*, Dead Garden *Caçada*, Gravekeeper *Sentença*, Ignoble *Favor*, Cavaleiros *Juramento/Voto*, Nobres *Desígnio*.
- **Grau** (Menor → Épico) maps to a suggested obstacle band (0/−2 → −16/−20), a **progress cap per Marco** (5/4/3/2/1), and **clock segments** (4/6/8/10/12). All share a **10-box Barra de progresso**.
- **Marcos** resolve with the normal action (`PA + Habilidade/Talento + Obstáculo`); progress = the **result ladder** (Ruína 0, Fracasso 0, Complicação 1 … Singular 5) **capped by Grau**. Chosen over flat rank-marking so the existing success scale is used.
- **Relógio** (new): +1 per Marco resolved, **+0 if won at Competente+** (efficiency), **+1 per round/post over the 1-round budget**, +1 extra on Fracasso, +2 on Ruína, +1 when the adversary advances. Filling it closes the deadline. This is the diceless pressure valve and the reason posts still matter after the level gate was removed.
- **Concluir** uses the Barra de progresso as raw likelihood (no extra roll): ≥8 **Conclusão Plena**, 5–7 **Conclusão Parcial** (reward −1 step + narrative cost), ≤4 **Fracasso**. Finishing with **≥ half the clock empty** grants the **Bônus de Diligência** (+1 material step and/or a Contato).
- **Abandonar** (dropping an Aventura) costs only the **Títulos bound to that Aventura** — kept deliberately simple; retaking it needs a follow-up Aventura of higher Grau, and the lore fallout (reputation, patrons, Fé) stays narrative.
- **Rewards** bridge to crafting: material level 1→5 by Grau, Títulos from Formidável up, gear at Extremo/Épico. Shared by participants. Named foes/dungeons keep the "double Causality" material ceiling from `Categorias de Talentos.md`.
- **Progression rewritten:** the **minimum-post requirement is removed**. Levels 2–8 now require concluding Aventuras of escalating Grau. Each PC owns a **Saga** (Grau Épico) structured as **7 Atos = the 7 levels**; its Clímax is the Feito Marcante → Convergência.
- **Shared Aventuras:** all participants receive progress and rewards; each counts the Aventura toward their Saga if it is relevant to it.
- Structural choices: a personal **Saga** (lifelong campaign), an initial hook, four ways Aventuras connect (secundária / adiada / cruzada / paralela), and the "a Marco must be a turning point" test.
- **Saga is optional:** it can be defined at creation or discovered during play, and levels advance with or without one. Acquiring a Saga may retroactively claim past Aventuras as its opening Atos; on Convergência the old Saga closes and a **new Saga** is born for the elevated character.
