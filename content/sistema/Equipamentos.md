---
title: Equipamentos
type: sistema
status: ativo
tags:
  - ddw
  - regras
---

# Equipamentos


![[f32cf264-1555-4097-bfc8-a71b5fd698c0.png]]

Os equipamentos — sejam lâminas de aço, cajados rúnicos ou artefatos — funcionam como extensões da capacidade da personagem, permitindo que ela execute ações sem consumir sua própria energia/mana (PA).

Equipamentos relevantes possuem um **Nível (1 a 5)** que determina sua potência base.

- **Nível 1-2:** Itens Mundanos ou de boa fatura.
- **Nível 3-4:** Itens Mágicos ou de mestre.
- **Nível 5:** Relíquias Únicas ou Artefatos.

### Utilizando Equipamentos

Ao realizar uma ação (ataque, defesa ou utilitária), o jogador pode optar por utilizar o Nível do Equipamento no lugar do gasto de PA.

**Fórmula da Ação:** `Nível do Equipamento + (Habilidade ou Talento)`

### Durabilidade e Desgaste

Todo equipamento possui uma integridade limitada. A **Durabilidade** máxima é proporcional à qualidade do item:

**Durabilidade Máxima:** `Nível do Equipamento x 2`

(Ex: Um equipamento de nível 5 tem 10 de Durabilidade).

Sempre que um equipamento substitui o PA em uma ação, sua durabilidade é reduzida. O valor perdido é igual à **Dificuldade Final** da ação (após todas as mitigações por Sinergia).

*Exemplo:* Um guerreiro ataca com uma espada Nível 3. A dificuldade (Defesa do alvo) é 5. Ele usa Sinergia para mitigar a dificuldade para 2. Ao final do ataque, a espada perde 2 de Durabilidade.

### Uso Consecutivo e Sobrecarga

Equipamentos não possuem Cooldown, mas desgastam facilmente se usados sem consideração. Se o mesmo equipamento for usado sem que haja um turno de intervalo com gasto de **PA** (Pontos de Ação) entre os usos, o dano na durabilidade dobra exponencialmente:

- **1º Uso:** Dano normal (Dificuldade).
- **2º Uso sem intervalo de PA:** Dano Dobrado (Dificuldade×2).
- **3º Uso sem intervalo de PA:** Dano Quadruplicado (Dificuldade×4).

Ações seguradas não entram nessa multiplicação — veja [[Equipamentos#Equipamentos em Ações Seguradas|Equipamentos em Ações Seguradas]].

> [!warning]
> Itens mágicos recebem um escudo de durabilidade temporário no início de cada cena igual ao valor do atributo **Arcanismo** do usuário. Este escudo é consumido antes da durabilidade real do item.

### Equipamentos em Ações Seguradas

Uma ação segurada também pode ser sustentada por um equipamento em vez de PA — mas **nunca de graça**. Enquanto a ação permanecer ativa, o item continua em uso e sofre desgaste a cada turno:

- **Ações seguradas comuns** (buffs, invocações, transformações): o item perde, por turno, durabilidade igual à **Dificuldade Final da ação**.
- **Guarda sustentada por equipamento** (ex: escudo): o desgaste é **por impacto** — cada ataque que a Guarda efetivamente bloqueia custa durabilidade igual à **dificuldade daquele ataque**. Turnos sem bloqueio não desgastam o item.

Nos dois casos o desgaste é **linear**: segurar é um uso contínuo e **não** entra na multiplicação do *Uso Consecutivo*.

> [!note]
> Sustentar com **PA** apenas mantém os pontos comprometidos; sustentar com **equipamento** consome o item. Guardar-se com PA é o caminho sustentável; guardar-se com escudo é para picos.

### Manutenção e Quebra

A durabilidade de um item pode ser restaurada através de Habilidades de criação. A dificuldade da para reparar é equivalente a durabilidade que se almeja recuperar. Falhar em um teste de reparo irá quebrar o item.

Se a Durabilidade de um equipamento chegar a **0**, o equipamento torna-se inutilizável e perde seus bônus até ser totalmente restaurado. Se sofrer dano enquanto estiver com 0, o item é destruído permanentemente.

> [!warning]
> Equipamentos de nível 1 e 2 podem ser raparados por NPCs em troca de dinheiro.

### Aquisição e Forja

O acesso a equipamentos de qualidade superior é limitado pelo prestígio e pelos recursos da personagem. No mundo de **Erwood**, a economia divide-se entre o comércio mundano e as conquistas lendárias.

| **Nível** | **Categoria** | **Forma de Obtenção** |
| --- | --- | --- |
| **1** | Mundano | Comércio Comum |
| **2** | Boa Fatura | Comércio Especializado / Encomenda |
| **3** | Mestre | Missões / Forja com Materiais Raros |
| **4** | Mágico / Épico | Dungeons Perigosas / Grandes Feitos |
| **5** | Relíquia | Clímax Narrativo / Durante uma aventura que resulte em Convergência |

> [!warning]
> Para mais informações de como forjar equipamentos, visite [[Talentos|Talentos de Fabricação]].

---

> [!info] Navegação
> ← [[Sistema de Títulos]] · [[index|Mapa de Conteúdo]] · [[Consumíveis]] →

