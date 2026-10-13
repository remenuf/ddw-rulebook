---
title: Inimigos e NPCs
aliases:
  - Antagonistas
  - NPCs
type: sistema
status: em desenvolvimento
tags:
  - ddw
  - regras
  - npc
---

# Inimigos e NPCs

> [!abstract] Por que um sistema próprio?
> Personagens jogadores administram recursos — Pontos de Ação, teto de regeneração, cooldowns, Consequências. Um Narrador conduzindo quatro bandidos não deveria carregar quatro economias inteiras. Este documento define como **inimigos e NPCs** funcionam: eles usam **números fixos, sem economia**.

O dano causado a um NPC **resolve exatamente como o de um PJ** (margem → caixas de Estresse → Consequência → Nocaute); o Narrador apenas pré-calcula as caixas. O que um NPC **não** tem:

- Não gasta nem regenera **PA**;
- Não tem **cooldowns** nem combinações de Talentos;
- Não tem **PA comprometido** nem ações seguradas;
- Não marca Estresse como custo de ação.

---

## O Bloco de Estatísticas

> **Nome** — *Tipo*
> **Causalidade:** X · **Ofensiva:** X · **Defesa:** X
> **Resistência:** caixas · **Ações:** X
> **Talentos:** *lista de balas, com "1×/cena" quando necessário*

- **Causalidade** — a mesma defesa passiva dos PJs (ver [[Iniciando Ações#Mitigando Obstáculos]]). Também concede caixas (abaixo).
- **Ofensiva** — valor fixo de ataque. Substitui `PA + Habilidade`.
- **Defesa** — valor fixo de defesa. Substitui a Guarda (`PA comprometido + Habilidade`).
- **Resistência** — as caixas de Estresse do NPC, derivadas do **Tipo** + **Causalidade**.
- **Ações** — quantas ações o NPC toma em seu turno (no seu próprio post).
- **Talentos** — efeitos especiais em texto, sem rastreamento de cooldown.

> [!info] Faixa de números
> A Ofensiva e a Defesa ficam na mesma faixa que os PJs alcançam com 0–8 PA somados a uma Habilidade: cerca de **3–4** (fraco), **6–7** (competente) e **8–10** (lendário).

---

## Causalidade

- **Pessoas comuns e capangas:** **−1**. Atacar quem não tem peso no mundo é **um passo mais fácil** (o Obstáculo cai em 1). Não concede caixa alguma — capangas são planos.
- **Genéricos:** **0**.
- **Antagonistas nomeados:** valores **positivos**, condizentes com seu peso na história.

> [!note] Peso no mundo
> Cada ponto de Causalidade concede **+1 caixa de Estresse `[1]`** à Resistência do NPC — além de já servir de defesa passiva. O mundo se dobra para manter de pé quem importa. Em contrapartida, valores negativos tornam o NPC mais frágil.

---

## Tipos e Equivalência de PC (EC)

A **Equivalência de PC (EC)** mede quanto de uma personagem jogadora um inimigo vale.

| Tipo | EC | Ações/turno | Resistência |
| --- | --- | --- | --- |
| **Capanga** | ¼ (4 ≈ 1 PJ) | 1 | 1 golpe (qualquer dano o derruba) |
| **Tropa** | 1 (como grupo) | 1 (grupo) | pool compartilhado |
| **Elite** | **1** | **2** | caixas `[1][2]` + Causalidade |
| **Chefe** | **1–3** (à escolha do Narrador) | **2 + (EC − 1)** | caixas `[2][2][4]` + Causalidade + Consequências + Fases |

- **Elite = 1 PC:** espelha um PJ — 2 ações, Defesa/Ofensiva na faixa competente, Causalidade 1–2 para igualar a durabilidade. Um duelo justo 1 contra 1.
- **Chefe = 1 a 3 PCs:** o Narrador escolhe a EC conforme o tamanho do grupo.

### Orçamento de Encontro

Some a EC de todos os inimigos e aproxime do **número de PJs**. Um Chefe EC 3 sozinho é o encontro inteiro para uma mesa de 3; uma mesa de 5 deve receber EC 5, espalhada entre um Chefe e capangas.

---

## Ações por Turno

> [!warning] Play-by-post não tem rodada justa
> A ordem é: **os jogadores postam**, depois o Narrador resolve e posta a fase dos inimigos. Não existe um intervalo entre os turnos dos jogadores para um Chefe "agir de novo". Por isso, um Chefe concentra **todas** as suas ações no próprio turno — nunca fora dele.

- **Capanga / Tropa:** 1 ação.
- **Elite:** 2 ações.
- **Chefe:** `2 + (EC − 1)` ações — EC 1 → 2, EC 2 → 3, EC 3 → 4, tudo no mesmo post.

---

## Chefes e o Peso dos PJs

Um Chefe sozinho é **focado** pela mesa inteira (os jogadores agem primeiro e somam 4–8 ações por rodada). Sem ações intercaladas, ele sobrevive **absorvendo** o ataque, com:

1. **Caixas de Causalidade** — a principal camada anti-foco: um Chefe Cau 3 é mais difícil de acertar *e* carrega 3 caixas extras.
2. **Fases** — ao esvaziar suas caixas, ele **transiciona** em vez de cair (ver abaixo).
3. **Alcance** — todo Chefe deve ter ao menos um Talento **multi-alvo**, para que um único turno pressione a mesa toda.
4. **Capangas** — a forma mais barata de absorver ações.
5. *(Opcional)* **Teto de dano** — ver a caixa abaixo.

> [!warning] Teto de dano (só para Chefes EC 3)
> Para um Chefe solo que não pode ser destruído por uma "nova" da mesa inteira, limite o dano que ele sofre por turno (ex: no máximo **1 caixa de Estresse** por turno, ignorando o excedente). Use com moderação — é uma rede de segurança, não uma regra padrão.

### Fases

Um Chefe tem **Fases** em vez de apenas cair. Ao chegar a 0 caixas, ele:

- Limpa parte de suas caixas de Causalidade;
- Troca Ofensiva e/ou Defesa por um novo perfil;
- Ganha um Talento novo.

Só na última Fase ele pode ser derrotado de fato.

---

## Mortalidade

Inimigos seguem a **mesma lógica dos PJs**:

- Dano resolve por caixas → Consequências → **Nocaute** (ver [[Combate#Estresse e Consequências]]).
- **Nocaute não é morte.** Um inimigo caído só morre por **Golpe de Misericórdia** ou por um efeito narrativo explícito (ver [[Combate#Morte e Golpe de Misericórdia]]).
- Vale o **Tom da Mesa**: no **Heroico** inimigos preferem capturar; no **Sombrio** (padrão) executam quando faz sentido; no **Brutal** tudo é possível — sempre **telegrafado**.

---

## Exemplos

> [!example] Bandido — *Capanga*
> **Causalidade −1** · **Ofensiva 4** · **Defesa 3** · **Resistência:** 1 golpe · **1 ação**
> *Sem Talentos — a força deles está no número.*

> [!example] Guarda de Elite — *Elite*
> **Causalidade 1** · **Ofensiva 6** · **Defesa 6** · **Resistência:** `[1][2]` +1 = `[1][1][2]` · **2 ações**
> *Formação: +1 de Defesa por aliado adjacente.*

> [!example] Líder da Guilda — *Chefe (EC 2)*
> **Causalidade 3** · **Ofensiva 8** · **Defesa 8** · **Resistência:** `[2][2][4]` +3 (Cau) · 3 Consequências · **3 ações**
> *Onda de Choque: Ofensiva contra todos no alcance.*
> *Fase 2: ao esgotar as caixas, limpa metade das caixas de Causalidade e troca a Ofensiva bruta por controle de área.*

## Notas relacionadas

- [[Combate]] — economia de ação, dano e Nocaute que os NPCs seguem.
- [[index|Mapa de Conteúdo]] — hub do vault.

---

> [!info] Navegação
> ← [[Categorias de Talentos]] · [[index|Mapa de Conteúdo]]
