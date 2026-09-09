# F0.6 — Exercícios de recuperação ativa e aplicação

**Assessment state:** `READY`

**Total:** 100 pontos

**Gate local de progressão:** `>=80/100` **e** nenhum critical fail.

Este instrumento mede desempenho observado. Produção da aula, leitura ou familiaridade com os termos não altera learner state.

## Regras

- Faça sem consultar `ANSWER_KEY.md`.
- Mostre raciocínio, não apenas respostas.
- Calculadora simples é permitida quando houver exponenciação.
- Quando a pergunta envolver um estudo concluído, privilegie estimate/CI sobre observed power.
- Não transforme `exploratory` em sinônimo de “inválido”.

---

# Parte A — Type I/II error, alpha, beta e power — 20 pontos

## A1 — Definições sem probability reversal — 8 pontos

Defina em suas próprias palavras:

1. Type I error;
2. alpha;
3. Type II error;
4. beta;
5. power.

Sua definição de power deve incluir explicitamente:

- efeito verdadeiro assumido/especificado;
- design/modelo;
- repeated sampling/replicações hipotéticas;
- rejeição de H0.

Depois repare estas frases:

- “alpha=0.05 significa 5% de chance de H0 ser verdadeira.”
- “80% power significa 80% de probabilidade de H1 ser verdadeira.”

## A2 — Power curve — 5 pontos

Mesmo desenho, alpha e variabilidade. Considere três efeitos verdadeiros hipotéticos:

- `delta = 0.2`;
- `delta = 1.0`;
- `delta = 2.0`.

Sem calcular power numericamente:

1. ordene os três cenários do menor para o maior power esperado;
2. explique por que dizer apenas “o estudo tem 80% power” é incompleto.

## A3 — Fatores que alteram power — 7 pontos

Para cada mudança abaixo, diga a direção **típica** do efeito sobre power, mantendo o restante comparável, e explique:

1. aumentar n;
2. tornar alpha mais estrito (`0.05 → 0.01`);
3. aumentar o verdadeiro effect size considerado;
4. aumentar a variabilidade residual.

---

# Parte B — Power, precision, sample-size justification e observed power — 20 pontos

## B1 — Power vs precision — 6 pontos

Dois estudos concluídos avaliam o mesmo outcome e usam o mesmo SESOI = `+2.0`.

### Study A

`estimate = +0.4`

`95% CI = −0.1 a +0.9`

### Study B

`estimate = +0.4`

`95% CI = −3.0 a +3.8`

1. Qual estudo é mais preciso?
2. Qual estudo é mais informativo sobre excluir benefício `>=+2.0`?
3. Por que não é suficiente perguntar qual estudo “teve mais power” depois de observar esses CIs?

## B2 — Observed power trap — 7 pontos

Um paper reporta:

`MD = +1.1; 95% CI = −1.5 a +3.7; p=0.40`.

Depois calcula observed power usando `+1.1` como efeito e obtém `27%`.

Os autores escrevem:

> “O resultado não foi significativo porque o estudo teve apenas 27% de power; portanto provavelmente ocorreu um false negative.”

Faça uma crítica em quatro etapas:

1. identifique o erro conceitual do observed power;
2. explique por que `27%` não é probabilidade posterior de false negative;
3. interprete o CI se SESOI=`+2.0`;
4. escreva uma conclusão melhor.

## B3 — Justificação de n — 7 pontos

Para cada cenário, escolha a estratégia de sample-size justification mais coerente e justifique:

### Cenário 1

O objetivo é estimar uma diferença média com CI suficientemente estreito para separar efeitos triviais de efeitos `>=2 unidades`.

### Cenário 2

O objetivo confirmatório é testar um efeito prespecified de `2 unidades` com alpha bilateral `0.05` e target power `90%`.

### Cenário 3

A população total acessível possui apenas 48 atletas elegíveis e todos serão convidados.

Use, quando pertinente:

- desired accuracy/precision;
- a-priori power;
- near-census/population;
- resource constraints;
- heuristic;
- no explicit justification.

---

# Parte C — Multiplicity e family-wise false-positive risk — 20 pontos

## C1 — Complement probability — 6 pontos

Sob a hipótese **ilustrativa** de testes independentes, todos os nulls verdadeiros e alpha=0.05 por teste:

1. calcule `P(>=1 false positive)` para `m=5`;
2. calcule para `m=20`;
3. explique por que essa fórmula não deve ser aplicada mecanicamente a outcomes correlacionados em qualquer paper.

Use:

`P(>=1 FP) = 1 − 0.95^m`.

## C2 — Defina a family — 7 pontos

Um trial tem:

- 1 primary outcome em week 12;
- 4 key secondary outcomes em week 12;
- 10 exploratory biomarkers em weeks 4, 8 e 12.

O paper declara que qualquer secondary com `p<0.05` comprova um benefício adicional e não descreve hierarchy ou adjustment.

Responda:

1. qual conjunto claramente exige uma multiplicity strategy para claims confirmatórios adicionais?
2. os 30 biomarker-time analyses precisam necessariamente pertencer à mesma confirmatory family? Explique.
3. por que “cada teste tem alpha=0.05” não resolve o problema conjunto?

## C3 — Estratégias conceituais — 7 pontos

Para uma família de cinco confirmatory endpoints, explique a função e uma limitação de cada estratégia:

1. único primary endpoint;
2. hierarchy/gatekeeping;
3. Bonferroni simples;
4. classificar analyses restantes como exploratory.

Não é necessário memorizar algoritmos avançados.

---

# Parte D — Analytical flexibility, subgroups e prespecification — 15 pontos

## D1 — Hypothesis multiplicity vs analytical-path multiplicity — 5 pontos

Um pesquisador testa o mesmo outcome/week 12 com:

- raw outcome;
- change score;
- ANCOVA ajustada por baseline;
- ANCOVA baseline + sex;
- com e sem dois outliers.

Ele escolhe o modelo de menor p-value.

1. Isso representa necessariamente 6 hipóteses científicas independentes?
2. Qual é o problema metodológico principal?
3. Que informação de protocol/SAP ajudaria a auditar o processo?

## D2 — Subgroup trap — 4 pontos

Resultado:

- homens: p=0.03;
- mulheres: p=0.21.

Autores concluem:

> “A intervenção funciona apenas em homens.”

Explique por que a conclusão não decorre desses dois p-values e o que deveria ser avaliado.

## D3 — Transparência — 6 pontos

Diferencie:

1. trial registration;
2. protocol;
3. SAP.

Depois explique por que:

- timing/versioning importam;
- uma alteração documentada após início do trial não é automaticamente fraude;
- preregistration não garante low risk of bias.

---

# Parte E — Performance task integrado — 25 pontos

Audite o estudo sintético abaixo.

## Planejamento disponível antes do recrutamento

120 atletas randomizados para A ou B.

Registro declara:

- primary outcome: time-trial performance em week 12;
- three secondary outcomes em week 12;
- alpha bilateral `0.05`;
- effect usado no sample-size planning: `+2.0%`;
- target power: `80%` para esse efeito;
- não há multiplicity strategy explícita para secondary claims.

O artigo não fornece link para SAP.

## Resultados reportados

Primary:

`effect = +0.6%`

`95% CI = −0.5% a +1.7%`

`p = 0.28`

Além disso, os autores:

- analisaram 20 outcomes em 4 time points = 80 outcome-time comparisons;
- testaram 6 definições de subgroup nos 20 outcomes em week 12 = até 120 interaction analyses;
- testaram até 3 covariate models para vários outcomes;
- destacaram mood/week 8, `p=0.008`;
- destacaram recovery no subgroup “high baseline fitness”, `p=0.03`;
- chamaram os dois achados de “confirmatory evidence”;
- não forneceram tabela completa dos resultados testados;
- calcularam observed power do primary usando effect observado de `+0.6%` e argumentaram que “low observed power explains the nonsignificant primary”.

## Sua resposta deve conter estes 10 blocos

1. **Target confirmatory claims:** identifique o claim primário documentado e o status dos secondaries.
2. **Decision rule:** interprete alpha=0.05 sem probability reversal.
3. **Planning power:** explique o que “80% power para +2.0%” significa e não significa.
4. **Primary estimate/CI:** interprete `+0.6% [−0.5,+1.7]` usando F0.5; não use observed power.
5. **Effective family:** descreva quais analyses criam multiplicity e diferencie hypothesis family de model-path multiplicity.
6. **Subgroups:** critique o highlighted subgroup p=0.03.
7. **Prespecification evidence:** o que o registry sustenta e o que a falta de SAP deixa não resolvido?
8. **Confirmatory vs exploratory:** classifique mood/week8 e subgroup finding com base apenas nas informações dadas.
9. **Transparent reporting plan:** proponha pelo menos seis elementos que deveriam ser reportados/prespecified.
10. **Calibrated conclusion:** escreva um parágrafo final sem `p<0.05=truth`, sem observed-power rescue e sem declarar que preregistration garante validade.

---

# Critical fails

Qualquer um destes padrões bloqueia o gate mesmo com `>=80/100`:

- `power = P(H1 verdadeira)`;
- `1−power = P(este resultado não significativo ser false negative)`;
- observed/post hoc power calculado do effect observado usado como evidência de ausência/presença de efeito;
- tratar muitos testes unadjusted como provas confirmatórias independentes só porque cada um usa alpha=0.05;
- `preregistered = low risk of bias / correct design`;
- usar `p>0.05` para provar ausência do efeito no performance task;
- usar `p<0.05` de subgroup sem interaction para provar diferença entre subgroups;
- ignorar completamente estimate/CI na interpretação do estudo concluído.

---

# Competências avaliadas

- `K1` — definir alpha/beta/power/family;
- `K3` — diferenciar power/precision, hypothesis/path multiplicity, confirmatory/exploratory;
- `K4` — interpretar planning e observed results;
- `K5` — prever consequências de n, alpha, effect e multiplicity;
- `K6` — calcular FWER ilustrativa e aplicar sample-size logic;
- `K7` — integrar F0.4/F0.5 com prespecification e multiplicity;
- `K8` — reconhecer probability reversals, post hoc power misuse e selective analysis.