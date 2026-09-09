# F0.7 — Exercícios de recuperação ativa e aplicação

**Assessment state:** `READY`

**Total:** 100 pontos

**Gate local de progressão:** `>=80/100` **e** nenhum critical fail.

Este instrumento mede desempenho observado. Produção da aula, leitura ou familiaridade com os termos não altera learner state.

## Regras

- Faça sem consultar `ANSWER_KEY.md`.
- Mostre raciocínio, não apenas labels.
- Calculadora simples é permitida para inverse-variance arithmetic.
- Não use I² como decisão binária de pooling.
- Preserve effect measure, null value, magnitude e CI antes de discutir heterogeneity.
- Não transforme PRISMA em quality/risk-of-bias score.
- Em subgroup/meta-regression, aplique as proteções de F0.6 contra multiplicity e post hoc storytelling.

---

# Parte A — Systematic review workflow e reporting — 15 pontos

## A1 — Systematic review versus meta-analysis — 5 pontos

Explique em suas próprias palavras:

1. o que é uma systematic review;
2. o que é uma meta-analysis;
3. por que uma systematic review pode ser válida sem meta-analysis;
4. por que uma meta-analysis numérica pode ser pouco confiável se os estudos foram selecionados de forma não sistemática.

## A2 — Reconstrua o workflow — 6 pontos

Coloque em ordem lógica e explique a função de cada etapa:

- extraction;
- protocol/question;
- synthesis;
- screening/selection;
- eligibility criteria;
- search;
- effect-measure choice/compatibility;
- heterogeneity/missing-evidence interpretation.

## A3 — PRISMA trap — 4 pontos

Autores escrevem:

> “A review seguiu todos os 27 itens do PRISMA 2020, portanto é uma revisão de alta qualidade metodológica e baixo risco de bias.”

Faça uma correção em duas partes:

1. o que PRISMA realmente ajuda a garantir/expor;
2. o que PRISMA não certifica.

---

# Parte B — Effect compatibility, weighting e models — 20 pontos

## B1 — Pooling compatibility — 6 pontos

Considere quatro reports:

- Study A: `MD=+2.0 unidades` no mesmo performance score;
- Study B: `MD=+1.5 unidades` no mesmo score;
- Study C: `SMD=+0.40` em outro instrumento que tenta medir construct semelhante;
- Study D: `RR=0.80` para um binary outcome.

Responda:

1. quais estimates podem ser pooled diretamente como MD?
2. por que C não entra simplesmente como `0.40` no mesmo MD?
3. por que D não pertence à mesma numerical synthesis só porque “favorece a intervenção”?
4. que perguntas sobre construct/time point/unit structure ainda precisam ser feitas antes de qualquer pooling?

## B2 — Inverse-variance intuition — 6 pontos

Dois studies estimam a mesma MD:

- Study A: `SE=0.20`;
- Study B: `SE=0.40`.

Use `weight ∝ 1/SE²`.

1. calcule o inverse-variance quantity de cada study;
2. qual recebe mais weight em um simple fixed-effect inverse-variance model?
3. aproximadamente quantas vezes mais?
4. por que isso **não** significa que o study com maior weight é metodologicamente melhor?

## B3 — Fixed versus random effects — 8 pontos

Para cada frase, marque `CORRETA` ou `INCORRETA` e repare as incorretas:

1. “Fixed-effect e random-effects são dois modos de corrigir bias dos estudos.”
2. “Em fixed-effect, uma interpretação comum assume um common underlying effect e diferenças observadas por sampling variation.”
3. “Random-effects permite effects diferentes relacionados e o pooled estimate representa uma average sob uma assumed distribution.”
4. “Se I² for alto, random-effects resolve o problema automaticamente.”
5. “A escolha fixed/random deve ser feita apenas pelo p-value do heterogeneity test.”
6. “Em random effects, entre-study variance pode reduzir a diferença relativa de weights entre estudos grandes e pequenos.”

---

# Parte C — Forest plot e heterogeneity — 25 pontos

## C1 — Forest-plot anatomy — 7 pontos

Sem consultar a aula, liste e explique pelo menos sete elementos de um forest plot, incluindo obrigatoriamente:

- study estimate;
- CI;
- null line;
- weight;
- pooled diamond;
- effect scale;
- heterogeneity information.

Depois explique por que o diamond não deve ser chamado de “true effect”.

## C2 — Heterogeneity layers — 8 pontos

Classifique cada diferença principalmente como `clinical diversity`, `methodological diversity`, ou `statistical heterogeneity signal`. Pode haver overlap; justifique.

1. um trial recruta elite athletes e outro recreational;
2. um usa blinded outcome assessment e outro não;
3. effects observados variam muito mais do que os CIs/sampling error sugerem;
4. intervenção dura 2 semanas em um study e 12 em outro;
5. um study analisa crossover como se groups fossem independentes;
6. outcome é medido em laboratory time-trial versus field performance test.

## C3 — I² traps — 10 pontos

Repare estas frases:

1. `I²=0%` prova que todos os studies são clinicamente idênticos.
2. `I²=20%` significa que 20% dos studies são heterogêneos.
3. `I²=85%` prova que meta-analysis é inválida e deve ser deletada.
4. I² é um quality score do evidence body.
5. Com poucos studies, I² pode ser incerto e deve ser interpretado junto com magnitude/direction, clinical/methodological diversity e outros heterogeneity information.

Para cada uma, explique o raciocínio, não apenas o label.

---

# Parte D — Sensitivity, subgroups, meta-regression e missing evidence — 15 pontos

## D1 — Sensitivity analysis — 4 pontos

Uma review apresenta:

- primary synthesis com todos os studies;
- sensitivity analysis excluindo um study com unit-of-analysis error;
- outra analysis criada após ver o resultado, excluindo os três studies com effects menores.

Explique:

1. qual sensitivity analysis tem rationale metodológico plausível;
2. por que a segunda parece outcome-driven;
3. como F0.6 prespecification/transparency deve ser aplicada.

## D2 — Subgroup/meta-regression trap — 5 pontos

Uma meta-analysis com 8 studies testa 12 moderators após observar high heterogeneity. Apenas “training status” produz interaction p=0.04.

Autores concluem:

> “Training status é a causa comprovada da heterogeneity.”

Critique usando:

- multiplicity;
- prespecification;
- small number of studies;
- study-level confounding/collinearity;
- difference between association and causal explanation.

## D3 — Funnel plot / small-study effects — 6 pontos

Responda:

1. o que é small-study effect?
2. cite quatro explicações possíveis para funnel-plot asymmetry;
3. por que asymmetry não prova publication bias?
4. por que symmetry não prova ausência de missing evidence?
5. por que um funnel plot com apenas cinco studies não autoriza uma conclusão forte de “no publication bias”?

---

# Parte E — Performance task integrado — 25 pontos

Audite a synthetic review abaixo.

## Protocol antes da busca

Review question:

`Intervention X versus control` sobre synthetic performance score; maior valor = melhor.

Prespecified:

- adult trained/recreational athletes;
- randomized parallel trials;
- primary outcome: performance score at 8–12 weeks;
- MD quando a mesma scale estiver disponível;
- random-effects synthesis devido a expected clinical diversity;
- subgroup trained versus recreational;
- sensitivity analysis excluindo high attrition.

## Search/reporting

Autores reportam:

- quatro bibliographic databases;
- trial registry;
- sem language restriction;
- data da última busca;
- PRISMA 2020 completo.

## Five compatible studies

| Study | Population/context | MD | 95% CI | SE |
|---|---|---:|---:|---:|
| A | recreational; short duration | +0.2 | −0.5 to +0.9 | 0.35 |
| B | recreational | +0.5 | −0.3 to +1.3 | 0.40 |
| C | trained | +1.1 | +0.5 to +1.7 | 0.30 |
| D | elite; different measurement setting | +2.4 | +1.5 to +3.3 | 0.45 |
| E | elite; different measurement setting | +3.0 | +2.0 to +4.0 | 0.50 |

Software reports:

- random-effects pooled MD `+1.4 [0.4,+2.4]`;
- `I²=87%`;
- fixed-effect pooled MD `+1.18`.

## Sixth incompatible study

Study F usa outro questionnaire/construct e reporta:

`SMD=+0.60 [0.10,+1.10]`.

Autores querem adicionar `0.60` diretamente ao MD pooling “porque aponta na mesma direção”.

## Post hoc exploration

Depois de ver `I²=87%`, testam:

- duration `<8 vs >=8 weeks`;
- elite vs non-elite;
- indoor vs outdoor;
- high vs low baseline score;
- leave-one-out analyses.

Destacam elite status porque interaction `p=0.04`. Elite status é quase collinear com measurement setting e não foi prespecified.

## Missing-evidence claim

Há apenas cinco compatible studies. Autores desenham funnel plot e dizem:

> “O plot parece symmetric, provando ausência de publication bias.”

## Authors’ conclusion

> “PRISMA compliance confirma high-quality evidence. Meta-analysis proves Intervention X improves performance by ~1.4 units. High I² merely justifies random effects and no longer matters. Elite athletes respond more because subgroup interaction p=0.04.”

## Sua resposta deve conter estes 10 blocos

1. **Review process:** identifique strengths e o que reporting não prova.
2. **Compatibility:** explique por que A–E podem ser considered together provisionally e por que F não entra como `0.60 MD`.
3. **Weights:** explique inverse-variance weight e por que weight ≠ quality.
4. **Pooled result:** interprete `+1.4 [0.4,+2.4]` pela lógica F0.5, sem chamar de universal truth.
5. **Heterogeneity:** interprete `I²=87%` sem automatic pooling ban nem dismissal.
6. **Clinical/methodological alternatives:** dê pelo menos duas explanations antes de aceitar elite-status story.
7. **Subgroup/meta-regression:** critique post hoc moderator testing e p=0.04.
8. **Missing evidence:** critique o funnel-plot claim com apenas cinco studies.
9. **PRISMA:** explique por que complete reporting não certifica low risk of bias/high certainty.
10. **Pooling decision + calibrated conclusion:** diga se/como mostraria a pooled MD e quais caveats ou alternative synthesis são necessários.

---

# Critical fails

Qualquer um destes padrões bloqueia o gate mesmo com `>=80/100`:

- `pooled estimate = automaticamente true/superior evidence`;
- `low I² = studies clinically/methodologically identical`;
- `high I² = meta-analysis automatically invalid`;
- `PRISMA-complete = low risk of bias/high quality`;
- pooling direto de incompatible effect measures/scales só porque apontam para mesma direction;
- `random effects resolves heterogeneity`;
- `weight = study quality`;
- comparar subgroup significance labels em vez de interaction;
- tratar post hoc subgroup/meta-regression pattern como proven cause;
- funnel symmetry como proof of no publication bias;
- funnel asymmetry como proof of publication bias;
- ignorar magnitude/CI do pooled result;
- selecionar sensitivity analysis apenas para obter conclusion favorável e apresentá-la como prespecified.

---

# Competências avaliadas

- `K1` — systematic review/meta-analysis/heterogeneity/weight definitions;
- `K2` — review workflow e forest-plot structure;
- `K3` — systematic review vs meta-analysis, fixed vs random, clinical/methodological/statistical heterogeneity;
- `K4` — interpret pooled estimate/CI/I²/funnel patterns;
- `K5` — prever consequências de incompatible pooling, weights, heterogeneity e missing evidence;
- `K6` — inverse-variance arithmetic e forest-plot application;
- `K7` — integrar F0.2/F0.5/F0.6 em evidence synthesis;
- `K8` — reconhecer limites de pooling, I², subgroup stories, PRISMA e small-study diagnostics.
