# F0.9 — Leitura crítica de um artigo completo

**Production state:** `APPROVED`

**Prerequisites P2:** F0.1–F0.8.

**P0 ensinados localmente:** article anatomy, main text, supplement, appendix, registry, protocol, statistical analysis plan (SAP), data repository, provenance, publication timeline, extraction table, result table.

**P1 ensinados localmente:** navegação entre artigo/suplemento/registro/protocolo/SAP; extração compacta de PICO/estimand; construção de uma tabela de resultados antes da interpretação; auditoria temporal de prespecificação.

**Core/method sources:** `F0-S01`, `F0-S07`, `F0-S18`, `F0-S19`, além das unidades canônicas F0.1–F0.8.

**Full-paper performance source:** `F0-S30`, acompanhado pelo registro `F0-S31`.

## 1. Competência-alvo

Ao terminar esta unidade, você deve conseguir ler um artigo completo de nutrição/exercício e produzir um appraisal em que a conclusão seja reconstruída a partir da pergunta, métodos e resultados — não copiada do abstract ou da discussão.

A sequência obrigatória é:

`1. question/estimand → 2. design/sampling → 3. intervention/exposure/comparator → 4. outcome measurement → 5. bias/confounding/missingness → 6. sample size/analysis plan → 7. effect estimate/uncertainty → 8. multiplicity/exploration → 9. result robustness → 10. applicability → 11. consistency with authors’ conclusion → 12. what the paper does not establish`

Regra central:

> **O artigo é um argumento empírico auditável. O título, o abstract e a discussão são alegações dos autores; a sua tarefa é reconstruir independentemente qual estimand foi realmente abordado, quais dados o informam, quão vulnerável é o resultado e até onde a conclusão pode ir.**

F0.9 não introduz uma nova “checklist mágica”. Ele integra F0.1–F0.8 em uma rotina única de leitura.

---

# 2. Por que o abstract não basta

O abstract é uma compressão editorial. Ele pode omitir:

- detalhes de randomização e amostragem;
- intervenções concomitantes;
- análise population;
- missing data;
- mudanças de outcome/timepoint;
- multiplicidade;
- estimativas não destacadas;
- intervalos de confiança relevantes;
- divergências entre registro e publicação;
- limitações de aplicabilidade.

Portanto:

`abstract = mapa inicial`

não:

`abstract = appraisal`.

Uma leitura crítica que não alcança Methods, Results e materiais externos disponíveis é incompleta por definição.

---

# 3. Anatomia operacional de um paper

## 3.1 Title

Serve para identificar a claim principal declarada. Não aceite o verbo causal ou a generalização do título antes de verificar desenho, estimand e população.

## 3.2 Abstract

Use para localizar:

- pergunta declarada;
- design declarado;
- amostra;
- outcomes destacados;
- números principais;
- conclusão dos autores.

Depois trate esses itens como hipóteses de navegação a serem auditadas no texto completo.

## 3.3 Introduction

Pergunte:

- qual lacuna os autores afirmam existir?
- qual pergunta/hipótese explicitam?
- a justificativa mecanística está sendo confundida com prova de desfecho?

## 3.4 Methods

É onde a pergunta deve ganhar forma executável:

- eligibility;
- recruitment/sampling;
- allocation/exposure definition;
- intervention/comparator;
- outcomes/timepoints;
- sample-size justification;
- analysis population;
- statistical model;
- missing-data approach;
- planned subgroup/sensitivity analyses;
- registration/protocol/SAP.

## 3.5 Results

É onde você extrai os objetos quantitativos sem depender do framing da discussão:

- participant flow;
- baseline/descriptive information;
- estimate;
- effect measure;
- CI/SE;
- p-value quando pertinente;
- timepoint;
- analysis population;
- adverse events/missingness;
- sensitivity/subgroup outputs.

## 3.6 Discussion/Conclusion

Somente agora compare:

`authors' claim ↔ measured estimand ↔ observed estimates/uncertainty ↔ design/bias ↔ applicability`.

A discussão pode oferecer explicações plausíveis e literatura contextual. Não transforma uma hipótese pós-resultado em achado causal estabelecido.

## 3.7 Supplement / appendix

Pode conter:

- análise detalhada;
- tabelas completas;
- outcome definitions;
- sensitivity analyses;
- harms;
- model diagnostics;
- mudanças de protocolo.

“Não está no main paper” não significa “não existe”.

## 3.8 Registry, protocol e SAP

Esses materiais têm valor especial porque podem mostrar o que existia **antes** de resultados relevantes estarem disponíveis.

Mas presença não basta. O timestamp importa.

`document exists ≠ prospectively prespecified`

## 3.9 Data/code repository

Dados e código aumentam auditabilidade/reprodutibilidade potencial. Eles não corrigem automaticamente bias, confounding, measurement error ou prespecificação ausente.

---

# 4. Passo zero — provenance e versão

Antes da leitura substantiva, registre:

| Campo | Pergunta |
|---|---|
| Identidade | DOI/PMID/registro correspondem ao paper correto? |
| Versão | versão publicada, preprint, accepted manuscript ou correção? |
| Acesso | full text legal está disponível? |
| Materiais | há supplement, registry, protocol, SAP, data/code? |
| Timeline | quando estudo, registro, protocolo, análise e publicação ocorreram? |
| Correções | existe corrigendum/retraction/expression of concern relevante? |

Isso evita analisar uma versão errada ou atribuir valor prospectivo a um documento criado depois do estudo.

---

# 5. P1 — extraia antes de interpretar

A primeira proteção contra framing é transformar o paper em duas tabelas pequenas.

## 5.1 Tabela PICO/estimand

Preencha antes da discussão:

| Campo | Extração |
|---|---|
| Population | quem é elegível e quem realmente foi analisado? |
| Intervention/exposure | qual estratégia/exposição foi operacionalizada? |
| Comparator | contra o quê? |
| Outcome | qual construct e qual medida? |
| Time | em que janela? |
| Estimand/contrast | qual comparação/efeito o modelo tenta estimar? |
| Analysis population | randomized, ITT, modified ITT, completers, per-protocol etc.? |
| Target context | para quem você pretende usar a conclusão? |

Se você não consegue preencher uma linha, marque `NOT REPORTED / UNCLEAR`. Não invente.

## 5.2 Tabela de resultado

Para cada resultado material:

| Campo | Extração |
|---|---|
| Outcome/timepoint | o que e quando? |
| Contrast | qual grupo/condição versus qual? |
| Effect measure | MD, RR, OR, slope, interaction etc. |
| Point estimate | magnitude observada |
| CI/SE | precisão/valores compatíveis |
| p-value | saída estatística, não verdade binária |
| Analysis population | quem entrou nesse resultado? |
| Prespecification | primary/secondary/exploratory/post hoc/unclear |
| Practical threshold | definido? defensável? ausente? |
| Caveat | principal limitação desse resultado |

Uma frase como “houve melhora” não substitui esta tabela.

---

# 6. Etapa 1 — question/estimand | F0.1

Reconstrua:

`population → intervention/exposure → comparator → outcome → time → estimand`

Compare três perguntas:

1. o que o título parece perguntar?
2. o que os autores dizem perguntar?
3. o que o desenho/modelo realmente estimam?

Elas podem divergir.

Exemplo sintético:

> “Suplemento X melhora recuperação.”

O paper mede apenas soreness 24 h após uma sessão aguda em homens jovens não treinados.

O estimand observado não autoriza automaticamente claims sobre recuperação funcional, adaptação crônica ou atletas treinados.

`construct breadth > measured outcome` é um detector de extrapolação.

---

# 7. Etapa 2 — design/sampling | F0.2

Classifique a arquitetura sem transformar o nome do design em veredito.

Pergunte:

- randomized ou observational?
- parallel, crossover, cluster, factorial?
- prospective/retrospective?
- unidade de allocation = unidade de analysis?
- como participantes chegaram ao estudo?
- qual comparação é within- ou between-subject?
- houve follow-up suficiente para o outcome?

Depois escreva:

> **O design permite, em princípio, qual classe de inferência?**

E separadamente:

> **Que problemas de execução/análise ainda podem impedir essa inferência?**

`RCT ≠ automatically valid result`.

`observational ≠ automatically useless`.

---

# 8. Etapa 3 — intervention/exposure/comparator

Não aceite rótulos curtos como “high protein”, “timing”, “placebo” ou “usual diet”. Extraia operacionalmente:

- dose;
- composição;
- frequência;
- timing;
- duração;
- co-interventions;
- adherence/fidelity;
- diferenças calóricas/macronutricionais relevantes;
- washout/carryover quando aplicável;
- comparator real recebido.

Se dois braços diferem em mais de uma dimensão, o contraste causal também difere em mais de uma dimensão.

Exemplo:

> grupo A recebe 40 g de proteína + 250 kcal; grupo B recebe nada.

Uma diferença futura entre grupos não isolaria necessariamente “proteína” de energia/composição adicional sem assumptions adicionais.

---

# 9. Etapa 4 — outcome measurement | F0.1 + F0.3

Pergunte:

- qual construct deveria ser medido?
- qual variável operacional foi usada?
- instrumento válido/reprodutível para esse uso?
- assessor blinded quando isso importa?
- mesma intensidade de mensuração entre grupos?
- outcome surrogate ou diretamente decision-relevant?
- um ponto de medida representa o construct inteiro?
- learning/familiarization influencia performance test?

Measurement precision não é measurement validity.

Um instrumento pode produzir números altamente repetíveis e medir apenas uma fração do construct que a conclusão reivindica.

---

# 10. Etapa 5 — bias/confounding/missingness | F0.3 + F0.8

Não escreva apenas “há risco de viés”. Especifique:

`mecanismo → resultado afetado → direção plausível/indeterminada → impacto potencial`.

Para randomized trials, use RoB 2 como estrutura de raciocínio result-specific quando apropriado:

- randomization process;
- deviations from intended interventions;
- missing outcome data;
- measurement of outcome;
- selection of reported result.

Não some domínios em quality score.

Para observational intervention-effect questions, recupere F0.3/ROBINS-I/target-trial reasoning:

- confounding;
- selection;
- classification;
- missingness;
- measurement;
- selective reporting.

## Missing data

Percentual sozinho não decide bias.

Pergunte:

- quem ficou sem outcome?
- por quê?
- razões diferem entre grupos?
- missingness pode depender do true outcome?
- análise excluiu participantes pós-allocation?
- sensitivity analyses cobrem assumptions plausíveis?

---

# 11. Etapa 6 — sample size e analysis plan | F0.4 + F0.6

Separe quatro objetos:

1. sample-size justification prospectiva;
2. analysis plan prospectivo;
3. precisão observada;
4. análise de poder feita após os dados.

## 11.1 Sample-size justification

Pergunte:

- qual effect/precision target justificou N?
- alpha/power/variance assumptions estavam especificados?
- o target era clinically/practically defensável?
- attrition foi considerada?

## 11.2 Analysis model

Extraia:

- outcome/model;
- repeated-measures structure;
- covariates;
- transformations;
- interaction terms;
- multiplicity adjustment;
- missing-data handling;
- analysis population.

## 11.3 Completed study

Depois do estudo, não use observed/post hoc power para explicar um resultado.

Use:

`estimate + CI + practical threshold + model/design/bias`.

Uma “sensitivity power analysis” pós-estudo pode informar aproximadamente que tamanho de efeito o design teria detectado sob assumptions escolhidas. Ela não transforma `p>0.05` em prova de ausência e não substitui CIs do contraste de interesse.

---

# 12. Etapa 7 — effect estimate/uncertainty | F0.5

A ordem permanece:

`Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning → unsupported claims`

## 12.1 Não confunda mudança no grupo com efeito entre grupos

Em um trial paralelo, isto:

> A melhorou significativamente do baseline.

não demonstra:

> A melhorou mais que B.

O contrast causal normalmente exige a **diferença entre grupos** ou interaction apropriada.

## 12.2 Não confunda “no significant difference” com equivalência

`p > 0.05` para group×time não prova que duas estratégias são equivalentes.

Para uma afirmação de ausência prática, você quer saber se a incerteza exclui efeitos maiores que um threshold relevante — e, para equivalence/non-inferiority claims formais, precisa de desenho/margem apropriados.

## 12.3 Ausência de CI é informação

Se o paper reporta p-value de interação, mas não um estimate + CI facilmente interpretável para o contraste principal, escreva:

> **a precisão do contraste principal não é completamente visível no relatório recuperado.**

Não preencha o CI ausente com imaginação.

---

# 13. Etapa 8 — multiplicity/exploration | F0.6

Construa a **claim family**, não apenas conte p-values.

Mapeie:

- primary outcomes;
- secondary outcomes;
- timepoints;
- subgroups;
- alternative models;
- transformations;
- pairwise comparisons;
- sensitivity analyses.

Depois classifique cada destaque como:

- prospectively primary/confirmatory;
- prospectively secondary;
- exploratory;
- post hoc;
- unclear.

## 13.1 Timeline de prespecificação

Use:

`study start → data collection/primary completion → registry/protocol/SAP timestamp → analysis/publication`

Pergunta decisiva:

> o documento estava publicamente/credivelmente fixado antes de os resultados relevantes poderem orientar escolhas?

Registro retrospectivo aumenta transparência sobre o que foi declarado posteriormente, mas não prova prespecificação prospectiva.

---

# 14. Etapa 9 — result robustness

Robustness não é “o p-value continuou <0.05”.

Pergunte se a interpretação muda sob decisões defensáveis:

- alternative reasonable model;
- missing-data assumptions;
- influential observations;
- transformed versus original scale;
- ITT versus completer/per-protocol;
- prespecified sensitivity analysis;
- objective versus subjective outcome;
- adjustment choices.

## 14.1 Robustness ≠ result shopping

Uma análise que aparece apenas porque a principal não foi favorável pode ser informativa exploratoriamente, mas não deve ser relabelada como confirmação.

## 14.2 Reprodutibilidade e dados abertos

Data/code sharing pode permitir checagem e reanalysis. Isso melhora auditabilidade, não muda retroativamente o desenho.

---

# 15. Etapa 10 — applicability | F0.8

Compare evidence versus target em pelo menos:

`Population → Intervention/exposure → Comparator → Outcome → Time → Setting → Decision context`

Pergunte por mecanismo de effect modification, não apenas por “diferença demográfica”.

Exemplos:

- untrained older men → trained female athletes;
- adequate baseline protein → low-protein population;
- 2 sessions/week → high-volume elite training;
- 12 weeks → multi-year adaptation;
- muscle thickness → competition performance.

Um estudo pode ter boa internal validity e applicability estreita.

Um estudo representativo pode continuar internamente biased.

---

# 16. Etapa 11 — authors' conclusion versus evidence

Agora leia a conclusão linha por linha.

Para cada claim, classifique:

- directly supported;
- supported with caveat;
- exploratory/plausible;
- overextended;
- unsupported by measured data.

## 16.1 Verbo importa

Compare:

- “we did not detect a difference”;
- “the data are compatible with no important difference”;
- “there is no effect”;
- “strategy X should not be used”.

Essas frases exigem níveis diferentes de evidência.

## 16.2 Explicação mecanística após o resultado

Uma explicação biologicamente plausível para o achado não demonstra que aquele mecanismo gerou o resultado observado.

---

# 17. Etapa 12 — what the paper does not establish

Todo appraisal termina com limites positivos de inferência.

Complete:

> **Este paper pode informar ______, mas não estabelece ______.**

Possíveis limites:

- população não estudada;
- dose/fonte não estudada;
- outcome diferente;
- janela temporal diferente;
- causalidade quando desenho é observational;
- equivalência quando trial não foi desenhado para equivalência;
- mecanismo quando apenas desfecho foi medido;
- efeito crônico a partir de outcome agudo;
- recommendation strength a partir de um único result.

Isso é mais rigoroso que encerrar com “mais estudos são necessários”.

---

# 18. O paper dentro do evidence body | F0.7 + F0.8

F0.9 avalia um paper, mas não o transforma em corpo de evidência.

Pergunte:

- o resultado é consistente com literatura anterior?
- há revisão/meta-analysis relevante?
- o paper mede o mesmo construct/estimand?
- sua existência atualiza materialmente a body-level certainty?

Mas não faça um GRADE completo de um body que você não reconstruiu.

`single-paper appraisal ≠ body-of-evidence certainty rating`.

Da mesma forma:

`one low-RoB result ≠ high-certainty field consensus`.

---

# 19. Reporting guidelines: mapa, não placar

CONSORT, STROBE e PRISMA podem ajudar a localizar:

- eligibility;
- randomization;
- outcomes;
- sample-size methods;
- registration;
- protocol/SAP;
- flow/missing data;
- analysis reporting.

Mas:

`checklist completion ≠ low risk of bias ≠ high certainty`.

A função correta é:

> “Que informação deveria estar visível para eu conseguir auditar?”

A função incorreta é:

> “Marquei 26/30; logo o estudo é 86,7% confiável.”

---

# 20. Evidence extraction before narrative — worked synthetic case

Paper sintético:

- 60 runners randomized to beverage X versus placebo;
- primary outcome: 10-km time after 8 weeks;
- secondary: RPE, body mass, CK, soreness;
- registry posted before recruitment;
- 10-km contrast: `MD -12 s [−40,+16]` where lower=faster;
- soreness: `MD -1.1 [−1.8,−0.4]`, one of four secondary outcomes;
- authors conclude “X improves endurance performance and recovery”.

## Extraction

Primary performance result:

- direction: point estimate favors X;
- magnitude: 12 s faster;
- CI: compatible with about 40 s faster through 16 s slower;
- no practical threshold supplied;
- no statistically detected primary difference is not proof of no performance effect.

Secondary soreness:

- estimate/CI favor X;
- multiplicity and secondary status matter;
- it does not transform the primary performance result.

Conclusion audit:

- “improves recovery” may be supported for the measured soreness construct, with secondary/multiplicity caveat;
- “improves endurance performance” is stronger than the uncertain primary contrast warrants.

This is the F0.9 habit: **extract first, narrate second**.

---

# 21. Standard appraisal note

For an unfamiliar paper, produce this compact output after completing the 12 steps:

## A. Research question / estimand
One paragraph.

## B. Design and execution
Architecture, sampling, intervention/exposure/comparator, outcomes.

## C. Analysis and prespecification
Sample-size rationale, model, missingness, multiplicity, registry/protocol/SAP timeline.

## D. Main result table
Estimate + CI + practical threshold/context.

## E. Material bias/robustness issues
Ranked by likely impact, not by checklist order.

## F. Applicability
Evidence target versus decision target.

## G. Strongest defensible inference
One calibrated statement.

## H. Authors' conclusion audit
Proportional / partly proportional / overextended, with reasons.

## I. What is not established
Explicit boundaries.

---

# 22. Critical fails

A F0.9 response fails structurally if it does any of the following:

1. appraises only title/abstract;
2. treats `RCT`, `cohort` ou outro design label como the appraisal;
3. substitutes checklist completion for reasoning;
4. interprets `p<0.05` as true/important effect;
5. interprets `p>0.05` as proof of no effect/equivalence;
6. uses observed/post hoc power to rescue a completed-study conclusion;
7. ignores multiplicity or prespecification when material;
8. treats CONSORT/STROBE/PRISMA completeness as low RoB;
9. uses one overall RoB/certainty label instead of result-specific mechanisms;
10. confuses within-group significance with between-group treatment effect;
11. extrapola acute/mechanistic outcomes para chronic performance/body composition sem support;
12. repete a conclusão dos autores sem reconstruir independently o estimand/result;
13. inventa informação ausente de protocol/SAP/measurement/blinding;
14. transforma data sharing em garantia de validade;
15. trata um paper isolado como certainty rating de todo o evidence body.

---

# 23. Active recall

Sem consultar:

1. recite the 12-step F0.9 sequence;
2. list article components you inspect beyond abstract;
3. build the eight-field PICO/estimand table from memory;
4. build the ten-field result table from memory;
5. explain why within-group improvement is not a treatment effect;
6. explain why `p>0.05` is not equivalence;
7. distinguish sample-size planning, precision and observed power;
8. reconstruct a prospective-versus-retrospective registration timeline;
9. distinguish missing reporting from demonstrated flawed conduct;
10. state how RoB 2 helps without becoming a quality score;
11. list the seven applicability comparison fields;
12. state the strongest defensible inference before reading authors' discussion;
13. name three claims a single paper usually cannot establish alone.

---

# 24. Performance-paper rule

The independent performance task uses a real full paper (`F0-S30`) and its registry (`F0-S31`).

The lesson deliberately does **not** provide the completed appraisal of that paper. The learner must inspect the full text and registry before opening `ANSWER_KEY.md`.

The assessment paper is used as a methodological training object. Its inclusion is not endorsement or rejection of its substantive nutrition claim.

---

# 25. Limites deliberados

F0.9 does not require:

- reproducing every statistical model from raw data;
- formal forensic misconduct investigation;
- exhaustive GRADE body-of-evidence rating from one paper;
- advanced causal inference derivations;
- meta-analysis re-estimation;
- journal prestige or citation-count scoring;
- recommendation writing for real patients/athletes.

F0.10 will teach calibrated synthesis/communication after an evidence judgment has been produced.

---

# 26. Regra final

Before accepting a paper's conclusion, you must be able to answer:

> **What exact question was operationalized, who and what created the contrast, which result estimates that contrast, what uncertainty and bias mechanisms remain, which analyses were prospectively auditable, how robust/applicable is the result, and what claim survives after removing everything the paper did not actually establish?**
