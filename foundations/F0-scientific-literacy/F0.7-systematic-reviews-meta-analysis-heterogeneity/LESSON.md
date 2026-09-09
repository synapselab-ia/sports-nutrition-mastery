# F0.7 — Revisões sistemáticas, meta-análises e heterogeneidade

**Production state:** `APPROVED`

**Prerequisites P2:** F0.2 — desenhos de estudo e limites de inferência; F0.5 — estimativas, intervalos de confiança, effect measures e relevância prática; F0.6 — multiplicidade, prespecification e flexibilidade analítica. F0.3 é fortemente recomendado antes de interpretar formalmente risk of bias dentro de uma síntese.

**P0 ensinados localmente:** systematic review, meta-analysis, eligibility criteria, study selection, data extraction, synthesis, effect-measure compatibility, study weight, pooled estimate, fixed-effect meta-analysis, random-effects meta-analysis, heterogeneity, clinical diversity, methodological diversity, statistical heterogeneity, I², sensitivity analysis, subgroup analysis, meta-regression, small-study effects, non-reporting/publication bias.

**P1 ensinados localmente:** inverse-variance weighting intuition; log-scale reminder for ratio measures; forest-plot anatomy; prediction-interval intuition; direct interaction reasoning for subgroup differences.

**Core/method sources:** `F0-S03`, `F0-S04`, `F0-S05`, `F0-S06`.

## 1. Competência-alvo

Ao terminar esta unidade, você deve conseguir auditar uma revisão/meta-análise perguntando:

1. qual pergunta e eligibility criteria definem o evidence body?
2. como estudos foram procurados, selecionados e extraídos?
3. quais studies/results alimentam cada synthesis?
4. os effect measures/outcomes são compatíveis para pooling?
5. o que estimates, CIs, weights e diamond representam no forest plot?
6. qual quantity o fixed-effect ou random-effects model resume?
7. qual clinical, methodological e statistical heterogeneity existe?
8. o que I² informa e o que não prova?
9. a pooled quantity permanece cientificamente útil diante da diversidade?
10. sensitivity/subgroup/meta-regression foram prespecified ou result-driven?
11. existem small-study/missing-evidence signals e quais alternative explanations permanecem?
12. PRISMA torna o processo visível, mas o que ainda exige appraisal separado?

Regra central:

> **Uma meta-análise é uma síntese model-dependent de estimates selecionados por um processo de revisão. Ela não transforma estudos incompatíveis ou enviesados em verdade por média. Antes do pooled effect, pergunte o que está sendo combinado, por que é comparável e que diversidade a média pode esconder.**

---

# 2. Systematic review ≠ meta-analysis

Uma **systematic review** usa métodos explícitos para question/protocol, eligibility, search, selection, extraction, appraisal, synthesis e interpretation.

Uma **meta-analysis** é a combinação estatística de resultados de dois ou mais estudos.

Portanto:

- uma systematic review pode legitimamente não fazer pooling;
- uma numerical meta-analysis pode ser fraca se os studies foram selecionados de forma não sistemática.

`review process` e `combination mathematics` são problemas diferentes.

---

# 3. Workflow da systematic review

Use:

`Protocol/question → Eligibility → Search → Screening → Extraction → Study/result appraisal → Effect measure → Synthesis plan → Heterogeneity → Missing evidence → Interpretation`

## Protocol/question

Defina antes de examinar resultados favoráveis:

- population/context;
- intervention/exposure e comparator;
- outcomes/time windows;
- eligible designs;
- primary syntheses;
- important moderators/subgroups quando possível.

## Eligibility

Eligibility criteria delimitam qual evidence universe a review representa.

Mudanças pós-resultados podem alterar materialmente o body of evidence.

## Search

Audite:

- databases/information sources;
- registries quando pertinentes;
- search date;
- reproducible strategy;
- language/publication-status restrictions;
- additional search methods quando justificadas.

## Screening

Um **study** pode gerar vários **reports**. Não conte relatórios duplicados como studies independentes.

## Extraction

Preserve:

- design/sample;
- intervention/comparator;
- outcome/timepoint;
- effect measure;
- estimate + SE/CI;
- analysis population;
- unit-of-analysis structure;
- transformations/conversions.

Extraction errors podem criar weights errados e heterogeneity artificial.

---

# 4. PRISMA: reporting, não quality certificate

`F0-S03` — PRISMA 2020 — é a reporting guideline vigente para systematic reviews.

Ela expõe objective, eligibility, information sources/search, selection, synthesis, heterogeneity investigations, sensitivity analyses, protocol/registration e related reporting.

PRISMA 2020 contém 27 itens, expanded checklist, abstract checklist e flow diagrams.

Critical distinction:

`PRISMA-complete ≠ low risk of bias ≠ high certainty`

PRISMA responde principalmente:

> “consigo ver o que os autores fizeram?”

Não:

> “o que fizeram foi necessariamente correto?”

Formal risk of bias/certainty permanece F0.8.

---

# 5. Antes de pooling: effect-measure compatibility

F0.5 permanece obrigatório.

Não faça:

`MD + SMD + RR` como se fossem números da mesma scale.

Pergunte:

1. same construct?
2. same outcome direction?
3. comparable timepoint?
4. same target contrast?
5. valid conversion/transformation?
6. unit-of-analysis preserved?

## MD versus SMD

- MD combina original units quando scales são comparáveis;
- SMD pode harmonizar different instruments de um similar construct, mas não transforma different constructs em equivalentes.

## Ratio measures

RR e OR continuam distintos e ratio measures são normalmente analisadas em log scale em meta-analysis.

Directional agreement não é numerical compatibility.

---

# 6. Meta-analysis como weighted average

Em forma simplificada:

`pooled estimate ≈ Σ(w_i × theta_i) / Σw_i`

É uma média de **study estimates**, não “média das pessoas”.

---

# 7. P1 — inverse-variance weighting

Em um simple inverse-variance framework:

`weight ≈ 1 / SE²`

Menor SE → maior statistical weight.

Exemplo:

- `SE=0.20 → 1/0.20² = 25`;
- `SE=0.40 → 1/0.40² = 6.25`.

O primeiro recebe cerca de quatro vezes o inverse-variance weight.

Mas:

`weight ≠ study quality ≠ certainty`

Um estimate muito preciso ainda pode ser biased.

---

# 8. Fixed-effect meta-analysis

Em uma common interpretation, fixed-effect assume que os studies estimam o mesmo underlying effect e que observed differences decorrem de sampling variation.

A pooled quantity é uma common/typical-effect estimate sob esse model.

Não escolha fixed-effect apenas porque um heterogeneity test não foi statistically significant: com poucos studies, a capacidade de detectar heterogeneity pode ser baixa.

---

# 9. Random-effects meta-analysis

Random effects permite **different but related effects** representáveis por uma distribution.

O pooled estimate representa a **average effect** dessa assumed distribution.

A weight intuition inclui between-study variance `tau²`:

`weight_i ≈ 1 / (SE_i² + tau²)`

Quando tau² aumenta, weights tendem a ficar mais semelhantes e small studies recebem relativamente mais weight que em fixed effect.

Critical rule:

> **Random effects modela heterogeneity; não a elimina, não explica suas causas e não corrige bias.**

A escolha fixed/random deve seguir target quantity e model plausibility, não apenas um heterogeneity-test p-value.

---

# 10. CI do pooled mean versus prediction interval

Em random effects:

- pooled CI = uncertainty sobre a **mean effect**;
- prediction interval = tentativa de representar onde um effect de um comparable new study/context pode cair sob o model.

Uma narrow pooled CI pode coexistir com ampla between-study variation.

F0.7 exige a distinção conceitual, não derivação matemática.

---

# 11. Forest plot: anatomia

Identifique:

1. study label;
2. study effect estimate;
3. study CI;
4. marker size/weight quando mostrado;
5. null/reference line;
6. effect scale;
7. pooled diamond;
8. pooled CI;
9. subgroup labels;
10. heterogeneity statistics.

Null:

- MD/SMD/RD → normalmente `0`;
- RR/OR → `1`.

Diamond centre = pooled point estimate.
Diamond width = pooled CI.

`diamond ≠ truth`.

---

# 12. Leitura correta de forest plot

F0.5 sequence continua:

`Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`

F0.7 adiciona:

`Compatibility → Weight/model → Heterogeneity → Synthesis defensibility`

Não reduza a leitura a “cruza ou não cruza o null”.

---

# 13. Heterogeneity em três camadas

## Clinical diversity

Diferenças em participants, intervention dose/duration, comparator, outcome, follow-up, baseline context e setting.

## Methodological diversity

Diferenças em design, measurement, analysis population, missing-data handling, unit-of-analysis treatment e bias mechanisms.

## Statistical heterogeneity

Observed effect estimates variam mais do que seria esperado apenas por sampling error sob o model.

Statistical heterogeneity pode refletir real effect modification, methodological differences, measurement variation, extraction problems ou combinações.

`heterogeneity ≠ automaticamente biological variability`.

---

# 14. I²: informação sem threshold worship

I² descreve aproximadamente a proportion da observed variability entre study effects atribuível a heterogeneity em vez de sampling error no framework usado.

I² NÃO é:

- percent of studies “heterogeneous”;
- percent effect “explained”;
- quality score;
- probability meta-analysis is wrong;
- proof of study equivalence when low;
- automatic pooling ban when high.

Cochrane oferece rough ranges, mas alerta que thresholds podem mislead. Interprete junto com:

- magnitude/direction dos effects;
- number of studies;
- uncertainty of heterogeneity estimates;
- clinical/methodological diversity.

Com poucos studies, I² pode ser impreciso.

---

# 15. Quando pooling pode ser inadequado

Sinais contra pooling:

- materially different questions/estimands;
- incompatible outcome constructs;
- incompatible effect scales sem defensible conversion;
- reversed/mis-harmonized directions;
- excessive clinical diversity que torna average pouco útil;
- methodological diversity dominada por different biases;
- unresolved extraction/unit-of-analysis problems;
- incompatible time horizons;
- insufficient information para useful model;
- opposing effects onde uma average esconderia decisões diferentes.

`não poolar ≠ não sintetizar`.

Narrative/tabular synthesis continua possível.

---

# 16. Sensitivity analysis

Sensitivity analysis pergunta:

> “a conclusion muda sob outra reasonable methodological assumption/decision?”

Exemplos:

- excluir unit-of-analysis error;
- fixed vs random;
- alternative defensible conversions;
- remove influential study;
- alternative missing-data assumptions.

Não é sensitivity analysis defensável:

> testar versões até encontrar a mais favorável e reportar só aquela.

Aplique F0.6 prespecification/transparency.

---

# 17. Subgroup analyses

Subgroups podem investigar effect modification por population, dose/duration, setting, study design e outras characteristics.

Proibido:

`subgroup A significant + subgroup B nonsignificant = interaction`

É necessária direct interaction reasoning.

Post hoc subgroup patterns são normalmente hypothesis-generating, especialmente com poucos studies e múltiplas moderators testadas.

---

# 18. Meta-regression

Meta-regression relaciona study-level effect estimates a study-level characteristics.

Exemplo:

`effect estimate ~ intervention duration`

Limitações:

- poucos studies;
- multiplicity de candidate moderators;
- study-level confounding;
- collinearity;
- post hoc selection;
- ecological interpretation limits.

`meta-regression association ≠ proven cause of heterogeneity`.

---

# 19. Small-study effects e missing evidence

Small-study effect = smaller/less precise studies mostram systematically different effects dos larger/more precise studies.

Possible causes:

- non-reporting/publication bias;
- higher bias in small studies;
- real clinical differences;
- effect-measure artefacts;
- chance.

Therefore:

`small-study effect ≠ publication bias proven`.

---

# 20. Funnel plots

Funnel plot = effect estimates versus study size/precision measure.

Asymmetry pode levantar suspeita, mas não diagnostica publication/non-reporting bias.

Symmetry também não prova ausência de missing evidence.

Current Cochrane guidance continua alertando que formal funnel-asymmetry tests têm low power e, como common rule of thumb, muitos são considerados apenas com ~10 ou mais studies.

Mesmo com número suficiente, asymmetry exige alternative explanations.

Formal ROB-ME permanece F0.8.

---

# 21. Worked example — heterogeneous synthesis

Cinco studies usam o mesmo MD scale:

| Study | MD | SE |
|---|---:|---:|
| A | +0.2 | 0.35 |
| B | +0.5 | 0.40 |
| C | +1.1 | 0.30 |
| D | +2.4 | 0.45 |
| E | +3.0 | 0.50 |

Approximate fixed-effect inverse-variance weights:

- A ≈ 23.7%;
- B ≈ 18.1%;
- C ≈ 32.2%;
- D ≈ 14.3%;
- E ≈ 11.6%.

Synthetic outputs:

- fixed-effect pooled MD ≈ `+1.18`;
- `I² ≈ 87%`;
- illustrative random-effects pooled MD ≈ `+1.40`;
- random-effects 95% CI ≈ `+0.44 a +2.36`.

Interpretation:

- study effects vary strongly;
- pooled random-effects value summarizes an average, not universal effect;
- pooled CI is uncertainty around the mean, not full effect distribution;
- clinical/methodological explanations must be examined.

---

# 22. Antes de aceitar uma subgroup story

Imagine larger effects nos elite studies, mas esses studies também têm longer duration e different measurement setting.

Possible stories:

- training status effect modification;
- duration effect modification;
- measurement/methodological differences;
- combination.

Não selecione uma story apenas porque combina com o observed pattern.

Verifique:

- prespecified moderator;
- direct interaction/meta-regression estimate + CI;
- multiplicity;
- collinearity;
- number of studies;
- alternative explanations.

---

# 23. Integrated 12-field review audit

Use:

`1. Review question → 2. Eligibility → 3. Search/selection → 4. Extraction/unit structure → 5. Effect compatibility → 6. Study estimates/precision → 7. Weight/model → 8. Clinical/methodological heterogeneity → 9. Statistical heterogeneity → 10. Sensitivity/subgroup/meta-regression prespecification → 11. Missing-evidence/small-study signals → 12. Pooling/conclusion defensibility`

Esse é o framework obrigatório do módulo.

---

# 24. Integrated synthetic scenario

Review de `Intervention X versus control` em synthetic performance score; higher = better.

Protocol anterior à busca:

- trained/recreational adults;
- randomized parallel trials;
- primary outcome at 8–12 weeks;
- MD quando same scale;
- random-effects devido a expected clinical diversity;
- prespecified subgroup trained vs recreational;
- sensitivity analysis excluindo high attrition.

Search reporta four databases + trial registry + no language restriction + search date.

Five compatible studies:

| Study | Population/context | MD | 95% CI | SE |
|---|---|---:|---:|---:|
| A | recreational; shorter duration | +0.2 | −0.5 to +0.9 | 0.35 |
| B | recreational | +0.5 | −0.3 to +1.3 | 0.40 |
| C | trained | +1.1 | +0.5 to +1.7 | 0.30 |
| D | elite; different measurement setting | +2.4 | +1.5 to +3.3 | 0.45 |
| E | elite; different measurement setting | +3.0 | +2.0 to +4.0 | 0.50 |

Software:

- random-effects pooled MD `+1.4 [0.4,+2.4]`;
- `I²=87%`;
- fixed-effect `+1.18`.

Study F usa different questionnaire/construct e reports `SMD=+0.60 [0.10,+1.10]`.

Não adicione `0.60` diretamente ao MD pool.

Post hoc, autores testam duration, elite status, indoor/outdoor, baseline score e leave-one-out variants. Destacam elite status com interaction `p=0.04`, embora elite status seja collinear com measurement setting e não prespecified.

Com apenas five compatible studies, funnel plot parece symmetric e autores claim “no publication bias”. Isso não é defensável.

Complete PRISMA reporting também não transforma essa synthesis em high-certainty evidence.

---

# 25. Critical fails

Rejeite:

1. `pooled estimate = automatically true/superior`;
2. `low I² = studies clinically/methodologically identical`;
3. `high I² = meta-analysis automatically invalid`;
4. `PRISMA-complete = low risk/high quality`;
5. direct pooling of incompatible effect measures/scales by sign;
6. `random effects resolves heterogeneity`;
7. `weight = quality`;
8. significant/non-significant subgroup comparison as interaction;
9. post hoc subgroup/meta-regression as proven explanation;
10. funnel symmetry as proof of no publication bias;
11. funnel asymmetry as proof of publication bias;
12. pooled p-value replacing magnitude/CI/context;
13. fixed/random choice made only from heterogeneity-test p-value;
14. outcome-driven sensitivity analysis relabeled prespecified;
15. meta-analysis used to hide materially different questions.

---

# 26. Active recall

Sem consultar:

1. systematic review vs meta-analysis;
2. review workflow;
3. study vs report;
4. effect-measure compatibility;
5. inverse-variance weighting;
6. weight vs quality;
7. fixed-effect target;
8. random-effects target;
9. tau² intuition;
10. pooled CI vs prediction interval;
11. forest-plot anatomy;
12. clinical/methodological/statistical heterogeneity;
13. what I² says;
14. what I² does not say;
15. when not to pool;
16. sensitivity analysis;
17. subgroup interaction trap;
18. meta-regression limits;
19. small-study effects;
20. funnel asymmetry limits;
21. PRISMA function/limit;
22. execute the 12-field audit from memory.

---

# 27. Integração com anteriores

F0.2: design/unit/inference boundaries.

F0.5: effect measures + estimate/CI/magnitude.

F0.6: prespecification + multiplicity + analytical flexibility.

F0.7: evidence-body assembly + weighted synthesis + heterogeneity + missing-evidence reasoning.

Nenhuma camada substitui a anterior.

---

# 28. Limites deliberados

Não entram em profundidade:

- derivation of Q/I²/tau² estimators;
- exhaustive random-effects estimator catalogs;
- network meta-analysis;
- IPD meta-analysis;
- advanced multivariate synthesis;
- formal ROB-ME;
- publication-bias correction models;
- formal GRADE certainty judgments.

RoB/certainty/applicability entram em F0.8.

---

# 29. Fontes e versão

## `F0-S03` — PRISMA 2020

Current reporting guideline; 27 items + expanded/abstract checklists and flow diagrams. Reporting transparency only; no low-bias certification.

## `F0-S04` — Cochrane Chapter 10

Current chapter page remains *Analysing data and undertaking meta-analyses*, citing Handbook v6.5 and chapter last updated November 2024. Provides weighting, fixed/random effects, heterogeneity, I², subgroup/meta-regression, sensitivity and pooling cautions.

Cochrane’s versions page records patch-level `6.5.1` changes through 2026; none replaces the Chapter-10 methods used here.

## `F0-S05` — Cochrane Handbook current methods

Review workflow plus current Chapter 13 missing-evidence/small-study cautions. Funnel asymmetry is non-diagnostic.

## `F0-S06` — Cochrane Chapter 6

Effect-measure/data compatibility, unit structure and log-scale ratio logic.

---

# 30. Regra final

Ao encontrar uma meta-analysis, não pergunte primeiro “qual o pooled effect?”. Pergunte:

> **qual evidence universe foi construído, que quantities entram na synthesis, como studies foram weighted, que diversity existe, quais analytical choices foram prespecified, o que pode estar missing e se uma pooled average ainda responde uma scientific question útil?**
