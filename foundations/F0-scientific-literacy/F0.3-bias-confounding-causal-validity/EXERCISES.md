# F0.3 — Exercícios de recuperação ativa e aplicação

**Use depois de estudar `LESSON.md`.**

Não consulte `ANSWER_KEY.md` na primeira tentativa. O objetivo é raciocinar sobre **mecanismos de distortion causal**, não apenas reconhecer nomes de bias.

## Estrutura e pontuação

- Parte A — recuperação ativa: 20 pontos
- Parte B — DAGs, causal roles e adjustment: 30 pontos
- Parte C — mecanismos de bias e repairability: 25 pontos
- Parte D — randomization + target-trial thinking: 15 pontos
- Parte E — integração completa em sports nutrition: 10 pontos

**Total:** 100 pontos.

### Gate local de competência

- `>= 80/100`: desempenho suficiente para seguir, desde que nenhuma falha crítica ocorra;
- `70–79`: corrigir as partes frágeis e refazer itens equivalentes;
- `< 70`: revisar F0.3 e repetir avaliação equivalente.

### Falha crítica, independentemente da nota

- tratar DAG como prova empírica de causalidade;
- afirmar que “ajustar muitas covariáveis” elimina confounding sem justificar causal roles;
- ajustar deliberadamente um collider como se isso sempre reduzisse bias;
- ajustar mediator ao estimar total effect sem reconhecer que o estimand muda;
- afirmar que randomization elimina selection, missingness, measurement e todos os problemas pós-randomização;
- afirmar que target-trial emulation transforma observational data em randomized data;
- declarar causalidade em cenário com reverse-causation plausível sem enfrentar temporal ordering;
- tratar percentual de missing data, isoladamente, como medida suficiente de bias;
- afirmar que unmeasured confounding foi “corrigido” por um método que não possui informação sobre ele, sem assumptions adicionais.

Esta avaliação pode sustentar `RECALLED`/`APPLIED` quando efetivamente realizada e corrigida. Produção do material não altera estado de aprendizagem.

---

# Parte A — Recuperação ativa — 20 pontos

Cada questão vale 2 pontos.

1. Diferencie random error de systematic error/bias.
2. Explique confounding usando a ideia de common cause.
3. O que é residual confounding? Dê duas causas possíveis.
4. Diferencie confounder, mediator e collider para uma pergunta de total causal effect.
5. Por que “ajuste tudo que estiver associado ao outcome” pode aumentar bias?
6. O que um DAG representa e o que ele **não** prova?
7. Por que complete-case analysis pode produzir selection bias?
8. Explique por que 10% de missing outcomes em cada braço não garante ausência de attrition bias.
9. O que randomization oferece para causal identification e quais dois problemas ela não resolve automaticamente?
10. Diferencie internal validity de external validity/applicability.

---

# Parte B — DAGs, causal roles e adjustment — 30 pontos

Cada questão vale 10 pontos.

Em cada item:

1. identifique o target causal effect;
2. classifique os nós relevantes como confounder, mediator, collider ou outro papel;
3. diga o que você ajustaria/não ajustaria para o **total effect**;
4. explique o mecanismo de bias que surgiria com uma estratégia incorreta.

## B1 — Training load, suplemento e desempenho

Pergunta: efeito total de iniciar suplemento `A` sobre performance `Y` em 12 semanas.

Assuma a estrutura:

```text
T ──► A ──► Y
└─────────► Y
```

`T` = training load pré-exposição.

1. Qual é o papel de T?
2. O que acontece se T não for adequadamente controlado em observational data?
3. Se T foi medido apenas por uma pergunta muito grosseira, qual problema pode permanecer mesmo após ajuste?
4. O que randomization de A mudaria nessa estrutura baseline?

## B2 — Mecanismo intermediário

Pergunta: efeito **total** de estratégia de carboidrato `A` sobre performance `Y`.

Assuma:

```text
A ──► M ──► Y
└─────────► Y
```

`M` = disponibilidade fisiológica de substrato após a estratégia.

1. Qual é o papel de M?
2. Ajustar M responde ao total effect? Explique.
3. Em que tipo de pergunta M poderia se tornar relevante para um estimand diferente?
4. Por que não basta dizer “M está associado a Y, então deve entrar no modelo”?

## B3 — Seleção para grupo elite

Pergunta: efeito de suplemento `A` sobre performance `Y`.

Assuma:

```text
A ──► S ◄── U ──► Y
```

`S` = ser selecionado para uma equipe de elite.
`U` = talento/potencial não medido.

O banco usado para análise contém **apenas S=1**.

1. Qual é o papel de S nesse caminho?
2. Por que restringir a S=1 pode criar associação entre A e U?
3. Por que ajustar estatisticamente por S dentro dessa amostra não “desfaz” automaticamente o problema?
4. Qual decisão de design seria preferível se a pergunta-alvo é sobre a população de atletas elegíveis antes da seleção elite?

---

# Parte C — Mecanismos de bias e repairability — 25 pontos

Cada cenário vale 5 pontos. Para cada um, responda obrigatoriamente em cinco linhas/blocos:

1. **Target causal question** — qual pergunta causal está sendo sugerida?
2. **Causal structure** — descreva o caminho relevante em palavras ou setas.
3. **Distortion mechanism** — por que a estimate pode se afastar do causal effect?
4. **Repairability** — o que pode ser prevenido/mitigado por design, measurement ou analysis e o que pode não ser recuperável dos dados disponíveis?
5. **Calibrated conclusion** — escreva uma conclusão proporcional às assumptions.

## C1 — Reverse causation

Um cross-sectional survey encontra que atletas com menor energy intake relatam mais fadiga na mesma semana. Os autores escrevem: “low energy intake causes fatigue”.

## C2 — Differential measurement

Em um randomized trial de um suplemento, participantes sabem o grupo. O primary outcome é uma escala subjetiva de recuperação. O grupo ativo foi informado de que o suplemento “pode acelerar recovery”, e avaliadores também conhecem assignment.

## C3 — Attrition por tolerabilidade

Um trial randomiza atletas para suplemento A ou placebo. No grupo A, participantes com fortes GI symptoms abandonam mais frequentemente. GI symptoms também prejudicam training e performance. O artigo publica apenas completer analysis.

## C4 — Exposure misclassification

Um cohort classifica atletas como “high” ou “low” habitual protein intake usando uma única pergunta de memória sobre “um dia típico” feita no baseline. O estudo acompanha performance por dois anos.

## C5 — Residual confounding

Em observational data, usuários de suplemento X têm melhor performance. O modelo “ajusta para training” usando apenas “dias por semana”, mas não mede volume, intensidade, coaching quality ou baseline commitment.

---

# Parte D — Randomization + target-trial thinking — 15 pontos

## D1 — “É RCT, então acabou” — 7 pontos

Um trial randomiza 300 atletas para A ou B. A randomization e allocation process parecem adequados. Depois:

- 30% de A e 8% de B ficam sem primary outcome;
- o avaliador conhece o grupo;
- análise final usa somente participantes com adherence >90%;
- adherence é maior entre participantes com maior baseline motivation.

Responda:

1. Qual problema causal baseline a randomization reduz? — 1 ponto
2. Identifique três ameaças pós-randomização presentes. — 3 pontos
3. Explique por que analisar apenas >90% adherent pode perder a comparabilidade criada no baseline. — 2 pontos
4. Escreva uma frase de conclusão que não trate “randomized” como sinônimo de “unbiased”. — 1 ponto

## D2 — Target trial observational — 8 pontos

Pergunta vaga:

> “Tomar café antes do treino melhora performance no longo prazo?”

Existe um grande banco observacional com hábitos de consumo e testes de performance.

Faça:

1. **Pergunta causal precisa** com population, strategies, outcome e time horizon. — 2 pontos
2. Especifique o target trial hipotético com eligibility, strategies, time zero, outcome/follow-up e causal contrast. — 3 pontos
3. Liste duas divergências de observational data que poderiam impedir boa emulation. — 2 pontos
4. Explique por que o framework não cria randomization nem measured confounders que o banco não possui. — 1 ponto

---

# Parte E — Caso integrativo de sports nutrition — 10 pontos

Leia o cenário:

> Pesquisadores usam dados de 2.000 corredores recreacionais. Pessoas que espontaneamente usam suplemento Z têm, em média, melhor time em 10 km após seis meses. Usuários de Z treinavam mais no baseline e eram mais propensos a contratar coach. O artigo ajusta para idade, sexo, BMI e “número de dias de treino por semana”, mas não mede volume/intensity nem coaching quality. Durante o follow-up, corredores com lesão abandonam com maior frequência; lesão é mais comum entre atletas de training load alto. O outcome final existe apenas para quem realizou novo 10 km. Entre completers, o modelo também ajusta para mudança de body mass durante o follow-up, embora Z possa afetar body mass e body mass possa afetar performance. Os autores concluem que Z “causes faster running”.

Produza uma mini crítica causal contendo obrigatoriamente:

1. **Target question/estimand** — 2 pontos
2. **DAG verbal ou em setas** com pelo menos um confounder, um possível mediator e um selection node — 2 pontos
3. **Dois invalid/inadequate adjustment decisions** e o mecanismo de distortion — 2 pontos
4. **Um problema que analysis talvez consiga mitigar sob assumptions e um problema que não pode ser garantidamente recuperado porque faltou measurement/data** — 2 pontos
5. **Calibrated conclusion** que preserve associação versus causal effect e explicite assumptions — 2 pontos

---

# Autoauditoria antes do gabarito

Antes de abrir `ANSWER_KEY.md`, confira se você:

- definiu a causal question antes de escolher covariáveis;
- separou random error de systematic bias;
- identificou common causes em vez de usar apenas associações estatísticas;
- distinguiu confounder, mediator e collider pelo DAG/temporal ordering;
- evitou “adjust all variables”;
- perguntou quem entrou, permaneceu e teve outcome observado;
- tratou missingness como mecanismo, não apenas percentual;
- auditou exposure/outcome/confounder measurement;
- testou reverse causation;
- separou o benefício baseline da randomization dos problemas pós-randomização;
- usou target-trial thinking como benchmark, não como retroactive RCT;
- separou internal validity de applicability;
- declarou quando informação ausente impede reparo garantido;
- escreveu conclusão cujo grau de certeza corresponde às assumptions restantes.