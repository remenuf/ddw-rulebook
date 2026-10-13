---
title: Combate
type: sistema
status: ativo
tags:
  - ddw
  - regras
---

# Combate


![[95780bd2-c0cb-41d3-aef3-f5af52f52eae.png]]

O combate é regido pela gestão de Pontos de Ação (PA) e pela integridade física da personagem, medida através de Estresse e Consequências. Para conduzir os antagonistas, veja [[Inimigos e NPCs|Inimigos e NPCs]].

### Economia de Ação

Cada personagem possui **2 ações por turno**. Uma "ação" é um esforço deliberado: **atacar, aplicar buff, aplicar debuff, curar, conjurar uma invocação** (ou iniciar qualquer ação segurada).

- Cada ação é paga com **PA**: a magnitude de uma ação é `(PA ou Equipamento) + Habilidade ou Talento`.
- Ações de **0 PA** continuam consumindo uma caixa de **Estresse**.
- Sua proteção não é uma ação: ela vem da **Guarda** (ver *Defesa*).

### Turnos e Iniciativa

- **O lado dos jogadores age primeiro**, na ordem que o grupo desejar (livre acordo). Em seguida, o Narrador resolve as ações dos inimigos.
- **Ordem entre inimigos** (prioridade decrescente): possuir um **Talento** relevante → possuir a **Habilidade** relevante → maior **Causalidade** → maior **valor da Habilidade** → **dado**. O dado pode servir como desempate — ou, se o grupo preferir, como primeiro critério. O Narrador também pode simplesmente definir a ordem.
- **Emboscada:** quem surpreende tende a agir primeiro; a ordem final é decidida pela narrativa.

### Ofensiva

Para atacar, o jogador deve somar o **PA investido** ao bónus de uma **Habilidade** ou de um **Talento**.

- **Cálculo de Ataque:** `(PA ou Equipamento) + (Habilidade ou Talento)`.

> [!warning]
> Ações de ataque não podem ser seguradas por meios normais.

### Defesa

A proteção de uma personagem divide-se em duas camadas:

1. **Defesa Passiva (Causalidade):** sempre ativa. Ataques que não superarem a Causalidade são ignorados.
2. **Defesa Ativa (Guarda):** uma postura que você **mantém**. Ao erguer a Guarda, gaste **1 ação** e **comprometa PA**: o valor dela é `PA comprometido + Habilidade ou Talento` e defende contra **todos** os ataques enquanto mantida. Enquanto comprometido, esse PA reduz seu teto de regeneração e não regenera (ver [[Iniciando Ações#Ações podem ser duradouras|Ações podem ser duradouras]]). Ao baixar a Guarda, o teto volta e o PA comprometido volta a regenerar.

Sustentar a Guarda com um **equipamento** (ex: escudo) troca o PA comprometido pelo desgaste do item — ver [[Equipamentos#Equipamentos em Ações Seguradas|Equipamentos em Ações Seguradas]].

> Baixar a Guarda libera o PA para o ataque — esse é o preço de “ir para cima”. Sem Guarda, você fica exposto e conta apenas com a Defesa Passiva.

### Defender um Aliado (Guarda Compartilhada)

Sua Guarda protege **você** por padrão. Você pode estendê-la para cobrir **um aliado** ao seu alcance.

- Estender a Guarda a um aliado gasta **1 ação**; o valor da Guarda e o PA comprometido continuam os mesmos.
- O aliado protegido usa a **sua Guarda** no lugar da defesa dele contra os ataques que receber.
- O dano que passar pela Guarda cai sobre o **alvo do ataque** (o aliado).
- Cobrir **mais de um aliado**, ou protegê-los à distância, exige **Talentos** (ex: *Guarda-Costas*, *Muralha*).

### Ataque Vs Defesa

Ao se comparar com o ataque, a defesa do jogador é considerada como o **Nível de Dificuldade** da ação do oponente. Portanto, o atacante pode diminuir essa dificuldade através do uso conjunto de Habilidades e Talentos (Sinergia). O defensor, por ser o "obstáculo" da cena, não se beneficia de Talentos Auxiliares para mitigar o ataque recebido, focando-se apenas em aumentar seu valor bruto de Guarda.

### Dano e Complicação

O dano é a diferença bruta entre a Ofensiva e a Defesa (`Ataque - Defesa`). No entanto, caso o dano final for **exatamente 1**, o atacante também sofre 1 de Estresse, por ter tido um “êxito com complicações”.

### Estresse e Consequências

O dano é alocado em caixas de **Estresse** com os valores: [1], [2] e [3]. Estes valores correspondem ao quanto de dano cada caixa pode absorver em um único ataque.

Quando uma personagem sofre dano, seu jogador escolhe qual e quantas caixas de **Estresse** irá consumir para receber aquele dano. Caso ainda sobre algum dano, ele será aplicado como uma **Consequência**.

> [!warning] Regra Global de Custos
> Sempre que uma ação exigir a marcação de uma caixa de Estresse (como em Ataques em Área ou ações de 0 PA) e o jogador não possuir caixas disponíveis, ele deve obrigatoriamente receber uma **Consequência**. Caso todos os slots de consequência também estejam ocupados, a personagem entra em **Nocaute** imediatamente.

> [!warning]
> Por mais que uma caixa de Estresse abrigue um dano menor que o seu limite, ela ainda será totalmente utilizada. Ex: Ao receber 1 de dano, o jogador que já tem a caixa de Estresse [1] marcada decide colocar o dano na caixa [2], essa caixa então é totalmente utilizada como se tivesse recebido dois de dano.

![[98bae456-c294-4f1d-bfea-e1b28a76050c.png]]

Enquanto o Estresse é o cansaço do combate, as Consequências são ferimentos reais com penalidades. E diferente do Estresse, que é totalmente limpo após um descanso, as Consequências são persistentes até serem curadas narrativamente.

> [!warning]
> Cada personagem possui inicialmente 3 espaços de C**onsequências**.

A gravidade de uma consequência é determinada pelo **dano excedente** — o que sobra após consumir as caixas de Estresse. Segue a tabela abaixo como referência:

| Tipo | Dano | Penalidade Mecânica | Recuperação |
| --- | --- | --- | --- |
| **Leve** | Até 2 | -1 em ações relacionadas ao Atributo afetado. | **Descanso Curto** (fim de cena com pausa). |
| **Média** | Até 4 | +2 turnos de Cooldown no Atributo afetado. | **Descanso Longo** (entre aventuras). |
| **Grave** | Até 6 | Bloqueio de Sinergia (não pode usar os Talentos do atributo afetado de forma auxiliar). | Uma **aventura dedicada à cura**. |

> [!info] Excedente acima de Grave
> Se o dano excedente passar de 6, aplique a tabela repetidamente: cada 6 pontos preenchem uma Consequência **Grave**, e o restante determina a faixa seguinte. Assim, 7–8 → **Grave + Leve**; 9–10 → **Grave + Média**; 11–12 → **Grave + Grave**; e **13+** preenche os três espaços — levando a personagem direto ao **Nocaute**.

Referente ao “Atributo Afetado” citadas na tabela: Quando uma Consequência é **atribuída**, a depender do cunho narrativo do dano, ela afetará um de seus atributos, aplicando a penalidade a todas as Habilidades vinculadas e, por consequência, aos seus Talentos.

Ex: Um guerreiro sofre um ataque que resulta em uma consequência física, logo sua Proeza Marcial e todas as Habilidades relacionadas receberão a penalidade dessa consequência. Da mesma forma um arcanista que receba dano em sua capacidade de lançar magia ou um devoto tenha sua fé abalada.

Note que a categoria da penalidade não é exclusiva por profissões. Um mago ainda pode receber uma penalidade física, apenas não seria tão punitivo quanto em um guerreiro.

### Nocaute

Uma personagem entra em **Nocaute** quando o dano excede todos os seus recursos de absorção — não há caixas de Estresse disponíveis e todos os slots de Consequência já estão ocupados por custos — ou quando uma regra específica o determina (Overdose, Maldições, etc.).

- Um alvo nocauteado está **indefeso**: não age, não defende, e qualquer ataque contra ele ignora sua Defesa.
- A personagem permanece nocauteada até ser **socorrida** (Talento de Cura ou Consumível) **ou** até conseguir um **Descanso Curto** (ver *Descanso e Recuperação*) — normalmente ao fim de uma cena com pausa. Se as cenas seguirem emendadas sem descanso, ela continua inconsciente.
- Ao despertar, todo o **Estresse** é limpo, mas as **Consequências** permanecem.

### Morte e Golpe de Misericórdia

Em Erwood a morte é um risco constante — mas nunca um acidente. **Nocaute não é morte**: é a derrota. A morte exige uma escolha deliberada.

- **Golpe de Misericórdia:** qualquer ataque declarado contra um alvo **indefeso** o mata (sem rolagem).
- **Sem morte por azar:** ninguém morre de um único golpe estando de pé. Só se morre **depois de já estar caído**, por execução deliberada ou por um efeito narrativo explícito.

**A Última Resistência (válvula de justiça):** quando um Golpe de Misericórdia é declarado contra um **PJ**, o jogador tem direito a uma **última ação desesperada** antes do golpe se resolver — fugir, ativar um último Talento, implorar, salvar um aliado. O mestre narra se o gesto muda o desfecho. Ele ainda pode terminar em morte, mas ela **nunca será apenas “o mestre decidiu”**: o jogador teve sua última escolha.

> [!info] Tom da Mesa
> O grupo define o tom da campanha no início:
> - **Heroico:** PJs só morrem com o consentimento do jogador (ou por uma morte heroica buscada); inimigos preferem capturar.
> - **Sombrio (padrão):** inimigos letais executam caídos quando isso faz sentido — o perigo é constante, mas sempre **telegrafado**.
> - **Brutal:** qualquer inimigo pode dar o golpe; sobreviver é a exceção.

> [!warning] Justiça antes da morte
> Telegrafe a letalidade. Um inimigo capaz de matar deve se revelar (reputação, postura, avisos) **antes** de estar sobre um caído. A morte deve parecer consequência, nunca pegadinha.

A morte é permanente. Um novo personagem entra na história em um momento narrativamente apropriado.

### Descanso e Recuperação

- **Descanso Curto:** um momento de pausa ao fim de uma cena. Limpa **todo o Estresse**, desperta personagens **nocauteadas** e cura Consequências **Leves**.
- **Sem descanso, sem alívio:** cenas emendadas sem pausa (por exemplo, combate → perseguição → combate) **não** limpam o Estresse — ele atravessa as cenas.
- **Descanso Longo:** o intervalo entre aventuras. Além de tudo do Descanso Curto, cura Consequências **Médias**.
- **Consequências Graves:** só desaparecem com uma **aventura dedicada à cura**.

### Ataques em Área

Ataques de grande escala permitem atingir múltiplos alvos simultaneamente. Atingir vários alvos de uma só vez é exaustivo: o autor deve **marcar uma caixa de Estresse** — esse é o custo do ataque em área, pago mesmo que ele erre ou não haja alvos válidos. Além disso, some o valor de seu **Atributo** utilizado à jogada de ataque.

O bônus do Atributo é dividido igualmente entre o número de alvos que possuam **Causalidade igual ou superior** à do autor.

Se o autor não tiver caixas de Estresse disponíveis, vale a **Regra Global de Custos** (recebe uma Consequência; em último caso, **Nocaute**).

- **Alvos com Causalidade Inferior:** Não contam para a divisão do bônus, mas sofrem o ataque com o bônus total resultante da divisão dos outros alvos.
- **Arredondamento:** O resultado da divisão é sempre arredondado para baixo. Se o número de alvos "pesados" for maior que o bônus, o bônus torna-se 0.

**Exemplo:**

> [!example]
> Um mago com 3 de Arcanismo e 1 de Causalidade decide lançar uma grande explosão em área, ele consome uma caixa de Estresse e faz a jogada com 2 PA + 3 (nível de seu talento). Agora vamos considerar os seguintes cenários baseados em seus alvos:
> 
> 1. **Três alvos de Causalidade 1:** O bônus de Arcanismo é dividido por três, aumentando em +1 na jogada de ataque contra cada alvo.
> 2. **Dois alvos de Causalidade 1:** O bônus é dividido por dois, mas como não é possível ter o bônus de 1.5, ele é arredondado para baixo, aumentando em +1 na jogada de ataque contra cada alvo.
> 3. **Quatro alvos de Causalidade 1:** Como o número de alvos é maior que o bônus, ele é zerado, porém o ataque em área ainda é efetuado.
> 4. **Três alvos de Causalidade 1 e Um de Causalidade 0:** Como o alvo de Causalidade inferior não conta para a divisão, o bônus dividido por três fica sendo +1 contra todos, incluindo contra o alvo de Causalidade 0.
> 5. **Cem alvos de Causalidade 0:** Por todos serem de Causalidade inferior ao atacante, o bônus não é dividido, aumentando em +3 na jogada de ataque contra todos os alvos.

---

> [!info] Navegação
> ← [[Talentos]] · [[index|Mapa de Conteúdo]] · [[Progressão de Personagem]] →

