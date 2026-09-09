# F0.8 — Risk of bias, certeza da evidência e aplicabilidade

**Production state:** `APPROVED`

**Prerequisites P2:** F0.2 — desenhos de estudo e limites de inferência; F0.3 — viés, confounding, raciocínio causal e validade; F0.5 — estimativas, intervalos de confiança, magnitude e relevância prática; F0.7 — revisão sistemática, meta-análise, heterogeneidade e missing evidence.

**P0 ensinados localmente:** reporting completeness, critical appraisal, risk of bias, result-specific judgment, domain-based judgment, certainty of evidence, GRADE, inconsistency, indirectness, imprecision, dissemination bias, applicability, generalizability, transportability, recommendation strength.

**P1 ensinados localmente:** comparação estruturada evidence-PICO versus target-PICO; threshold/range reasoning para certainty; leitura de tabelas de risk of bias e Summary of Findings em nível conceitual.

**Core/method sources:** `F0-S01`, `F0-S02`, `F0-S03`, `F0-S05`, `F0-S07`, `F0-S18`, `F0-S19`, `F0-S20`.

## 1. Competência-alvo

Ao terminar esta unidade, você deve conseguir separar e julgar cinco perguntas diferentes:

1. **o estudo/review relatou informação suficiente para ser auditado?**
2. **o resultado específico pode estar sistematicamente enviesado?**
3. **quanta confiança cabe no efeito de um corpo de evidência para um outcome/pergunta?**
4. **até onde essa evidência se aplica à população, intervenção, comparator, outcome, tempo e contexto-alvo?**
5. **uma recomendação deve ser forte ou condicional?**

Essas perguntas se conectam, mas não são sinônimas.

Regra central:

> **Reporting torna o processo visível; risk-of-bias appraisal pergunta se um resultado pode estar sistematicamente distorcido; certainty pergunta quanta confiança cabe no corpo de evidência para um outcome/pergunta; applicability pergunta se a inferência transporta para o alvo; recommendation strength integra ainda outros critérios de decisão.**

---

# 2. Cinco objetos que não podem ser colapsados

## 2.1 Reporting completeness

Pergunta:

> Consigo reconstruir o que foi planejado, feito, analisado e reportado?

Exemplos de reporting guidelines:

- CONSORT para randomized trials;
- STROBE para observational studies;
- PRISMA para systematic reviews.

Essas guidelines melhoram transparência. Elas não certificam baixa bias.

`CONSORT/STROBE/PRISMA complete ≠ low risk of bias`

## 2.2 Critical appraisal

É o processo de examinar fit-to-question, desenho, condução, análise, transparência, bias, precisão, aplicabilidade e outros limites.

Uma checklist pode ajudar, mas não substitui reasoning causal/estatístico.

## 2.3 Risk of bias

Pergunta:

> Por mecanismos de desenho, condução, análise ou reporting, este **resultado** pode estar sistematicamente afastado do alvo que pretendemos estimar?

RoB é diferente de random error.

- bias → systematic distortion;
- imprecision → uncertainty/random error.

Um result pode ser precise e biased.

## 2.4 Certainty of evidence

Pergunta:

> Para este outcome/pergunta e faixa/threshold de interesse, quanta confiança temos sobre onde o efeito verdadeiro se encontra?

GRADE trabalha em **body-of-evidence + outcome/question level**, não como medalha para um paper.

## 2.5 Applicability / transportability

Pergunta:

> Mesmo que a estimate seja internamente válida, ela responde diretamente ao target real de decisão?

## 2.6 Recommendation strength

Pergunta:

> Considerando net effects e demais critérios de decisão, quão forte deve ser a recomendação?

Certainty é um input importante, mas não é igual à recommendation strength.

---

# 3. Reporting guideline não é risk-of-bias tool

Considere dois estudos.

### Estudo A

Relato impecável:

- protocolo acessível;
- fluxo completo;
- análises descritas;
- outcomes definidos;
- missing data transparentes.

Mas:

- outcome assessment não blinded e altamente subjetivo;
- differential missingness relacionada ao outcome;
- análise seleciona uma versão favorável entre várias elegíveis.

Pode ser **bem reportado e high risk** para aquele resultado.

### Estudo B

Relato incompleto:

- artigo omite detalhes sobre allocation concealment.

Isso cria **insufficient information** para appraisal. Não prova automaticamente que concealment foi ruim.

Critical distinction:

> missing reporting pode impedir um judgment; não deve ser inventado como evidence de método ruim nem transformado em low risk.

---

# 4. Risk of bias é result-specific

Um mesmo estudo pode ter risk of bias diferente para resultados diferentes.

Exemplo randomized trial:

- performance time medido automaticamente por timing system;
- perceived recovery medida por assessor sabendo o grupo;
- missingness maior no outcome de recovery;
- selective analysis options só existem para um dos outcomes.

O trial não tem uma única essência chamada “quality = 7/10”.

Pergunte:

`qual result → qual effect of interest → quais bias mechanisms → qual direction/impact plausível → qual judgment?`

Essa é a razão para evitar somar domínios em score.

---

# 5. RoB 2 — randomized trials

A versão atual para individually randomized parallel-group trials permanece **22 August 2019**. Cochrane Handbook v6.5 Chapter 8 descreve RoB 2 como a ferramenta recomendada para risk-of-bias assessment em randomized trials dentro de Cochrane Reviews.

RoB 2 avalia um **resultado específico**.

## 5.1 Domínios centrais

1. **bias arising from the randomization process**;
2. **bias due to deviations from intended interventions**;
3. **bias due to missing outcome data**;
4. **bias in measurement of the outcome**;
5. **bias in selection of the reported result**.

Cada domínio usa signalling questions e exige justification.

Judgments usuais:

- `Low risk of bias`;
- `Some concerns`;
- `High risk of bias`.

## 5.2 Randomized ≠ automatically low risk

Randomization ajuda fortemente contra baseline confounding quando corretamente implementada.

Mas depois da assignment ainda podem surgir:

- deviations;
- differential co-interventions;
- missing outcomes;
- unblinded measurement;
- selective result reporting.

Então:

`randomized = design feature`

não:

`randomized = low risk by definition`.

## 5.3 Overall judgment não é média dos domínios

Não faça:

`Low=0, Some concerns=1, High=2 → somar → quality score`.

Domínios representam mecanismos qualitativamente diferentes. Um único problema crítico ao result pode dominar a interpretação.

---

# 6. Worked RoB 2 audit

Trial sintético:

- 180 atletas randomized X versus control;
- sequence computadorizada e concealment adequado;
- outcome primário: time-trial automatizado em 12 weeks;
- 22% missing em X versus 6% control;
- principais losses em X ocorreram após sintomas e pior training tolerance;
- análise primary usa completers;
- registry anterior confirma outcome/timepoint;
- nenhuma alternative primary analysis destacada.

### Randomization process

Pouca preocupação se sequence/concealment estão adequados e não há evidence de quebra.

### Deviations

Depende do effect of interest e de deviations relevantes. Não conclua só pela palavra “adherence”.

### Missing outcome data

Preocupação material: missingness é diferencial e plausivelmente ligada ao verdadeiro outcome.

### Measurement

Timing automatizado reduz algumas oportunidades de differential subjective measurement.

### Selection of reported result

Registry/prespecification ajuda a auditar se estimate/reporting foi selecionado entre múltiplas opções.

Conclusão:

> o result pode continuar vulnerable por missing outcome data mesmo com randomização bem implementada.

---

# 7. ROBINS-I e target-trial logic

Non-randomized studies of interventions precisam enfrentar confounding/selection de uma forma que randomization tenta prevenir na origem.

ROBINS-I usa um **target trial** como benchmark causal:

> qual randomized trial hipotético, sem flaws relevantes, responderia a mesma intervention-effect question?

O appraisal pergunta como o non-randomized study se afasta desse benchmark.

## 7.1 Current version status

Em 2026-09-09, o site oficial mantém **ROBINS-I V2, revised draft posted 20 November 2025**, explicitamente sujeito a mudança.

Não escreva apenas “ROBINS-I V2 é o standard final”. Registre o status de draft.

## 7.2 Current V2 draft — conceptual domains

O draft Nov 2025 lista seis domínios principais:

1. confounding;
2. classification of intervention;
3. selection into the study;
4. missing data;
5. measurement of the outcome;
6. selection of the reported result.

Também inclui uma triage section para mapear casos adequados a `Critical risk of bias`.

Importante: o V2 atual removeu o domínio separado de deviations from intended intervention que existia no draft de 2024.

## 7.3 Observational ≠ automatically unusable

Não randomizar aumenta desafios de confounding/selection para intervention-effect questions, mas a validade real depende do desenho, dados, measurement, analysis e assumptions.

Um strong non-randomized study pode contribuir informação valiosa; um randomized study pode ser badly biased para um result.

Logo:

`observational = automatically useless` é tão ruim quanto `randomized = automatically trustworthy`.

---

# 8. Risk of bias versus study design hierarchy

Use design como informação causal relevante, não como ranking suficiente.

Pergunte:

1. o design é adequado para a question?
2. qual effect/estimand está sendo avaliado?
3. quais bias mechanisms são possíveis?
4. quais foram prevenidos por design?
5. quais permanecem?
6. que magnitude/direction de distortion é plausível?

Um enorme observational cohort não recebe exchangeability por tamanho.

Um tiny randomized trial não recebe precisão por randomization.

`validity`, `precision` e `applicability` continuam eixos diferentes.

---

# 9. Da study-level RoB para body-level certainty

GRADE não pergunta apenas:

> quantos studies são “low risk”?

Pergunta:

> os limitations do conjunto de results ameaçam nossa confiança sobre onde o effect verdadeiro está em relação ao range/threshold relevante?

Isso exige integrar:

- quais studies têm maior contribuição;
- se low- e high-risk studies apontam para ranges diferentes;
- se concerns podem mudar a decision-relevant interpretation;
- quanto random error impede detectar essa diferença.

Não existe mapping mecânico:

`1 high-risk study = downgrade 1`.

O judgment é body/outcome specific.

---

# 10. GRADE — quatro categorias de certainty

Current GRADE Book mantém quatro níveis:

- **High**;
- **Moderate**;
- **Low**;
- **Very low**.

A interpretação contemporânea é threshold/range aware:

> certainty representa confiança de que o true effect esteja no lado correto de um threshold ou dentro de uma faixa de interesse.

Isso preserva F0.5:

- point estimate;
- CI;
- magnitude;
- practical/decision threshold.

## 10.1 High certainty não significa large effect

Você pode ter:

> high certainty de que o effect é trivial ou próximo do null.

## 10.2 Low certainty não significa no effect

Significa baixa confiança sobre onde o true effect está, não evidence de zero.

## 10.3 Statistical significance não determina certainty

Um tiny p-value pode coexistir com:

- serious bias;
- indirectness;
- inconsistency;
- missing evidence.

E um body pode ter informative near-null CIs sem threshold-based “significance”.

---

# 11. Starting point e study design em GRADE

Para intervention effects, a regra básica atual é:

- body de RCTs geralmente começa em `High`;
- body de NRSI geralmente começa em `Low` pela vulnerabilidade inicial a confounding/selection.

Mas GRADE também reconhece uma abordagem avançada:

- NRSI pode começar em `High` quando um structured ROBINS-I approach é usado;
- então confounding e outras limitations são explicitamente avaliados e podem levar a rating down.

Os dois caminhos costumam convergir quando NRSI têm material confounding/selection concerns.

A mensagem pedagógica é:

> starting level não é final verdict e não autoriza atalhos “RCT good / observational bad”.

---

# 12. Cinco domains que podem reduzir certainty

Para intervention-effect evidence, os cinco principais downgrading domains ensinados aqui são:

1. **risk of bias**;
2. **inconsistency**;
3. **indirectness**;
4. **imprecision**;
5. **dissemination/publication/non-reporting bias**.

F0.8 ensina a lógica desses domains, não um ritual de “tirar estrelinhas”.

---

# 13. Risk of bias domain em GRADE

Leva study/result appraisal para o body level.

Pergunte:

- material low-risk evidence existe?
- high-risk evidence recebe grande weight?
- estimates mudam quando higher-risk results são removidos?
- identified bias pode deslocar o effect através de um decision threshold?

F0.3 fornece o mecanismo; RoB tools estruturam o judgment; GRADE pergunta o impacto disso na certainty do evidence body.

---

# 14. Inconsistency

F0.7 ensinou que heterogeneity tem componentes:

- clinical;
- methodological;
- statistical.

GRADE inconsistency pergunta se observed effects variam de modo que reduz nossa confiança no range/threshold que importa.

Não faça:

`I² high → automatic downgrade`

nem:

`I² low → certainty protected`.

Examine:

- magnitude/direction;
- overlap relativo aos decision ranges;
- plausible effect modifiers;
- prespecified explanations;
- whether residual heterogeneity remains decision-relevant.

---

# 15. Indirectness

Current GRADE indirectness guidance liga directness à correspondência entre evidence e target question.

Comece por PICO:

- Population;
- Intervention/exposure;
- Comparator;
- Outcome.

F0.8 amplia operacionalmente para:

- time horizon;
- setting;
- decision context.

Indirectness não significa “qualquer diferença = downgrade”.

A pergunta é:

> há razão plausível para essas diferenças produzirem mudança material no effect ou absolute impact relevante à decisão?

## 15.1 Surrogate outcomes

Um physiological marker pode ser mechanistically interesting sem substituir automaticamente performance, morbidity ou outro target outcome.

Use F0.1 operationalization e F0.3 external-validity reasoning.

## 15.2 Baseline risk

Para ratio effects, F0.5 já mostrou que absolute impact depende do baseline.

Se target population tem baseline risk incerto/diferente, a directness do absolute effect pode cair mesmo quando relative effect transporta razoavelmente.

---

# 16. Applicability audit — evidence versus target

Use esta tabela mental:

| Element | Evidence body | Target | Pode mudar effect/absolute impact? |
|---|---|---|---|
| Population | quem foi estudado | para quem decidir | sim/não + por quê |
| Intervention/exposure | dose, delivery, adherence | estratégia real | sim/não + por quê |
| Comparator | placebo/usual care/etc. | comparator real | sim/não + por quê |
| Outcome | construct/measure | outcome importante | sim/não + por quê |
| Time | follow-up | decisão temporal | sim/não + por quê |
| Setting | lab/clinic/field | contexto-alvo | sim/não + por quê |
| Decision context | benefits/harms/resources | decisão real | afeta recommendation |

Do not score mismatches. Explain mechanism.

---

# 17. Internal validity versus applicability

Quatro combinações são possíveis:

1. internally strong + directly applicable;
2. internally strong + indirect/narrow applicability;
3. internally biased + apparently representative;
4. internally biased + indirect.

Amostra representativa não repara bias interno.

Low bias interno não garante transportability.

`direct evidence ≠ unbiased evidence`.

---

# 18. Imprecision

GRADE imprecision deve preservar F0.5 threshold-aware CI reasoning.

Pergunte:

> o CI/range permite efeitos em diferentes decision categories?

Exemplo threshold de benefit relevante = `+1.0`.

### Body A

`MD +1.5 [1.2, 1.8]`

O interval fica acima do threshold.

### Body B

`MD +1.5 [-0.4, 3.4]`

Mesmo point estimate, mas o range inclui harm/triviality e large benefit.

Body B é muito menos informative.

Não use:

`p<0.05 = precise enough`.

---

# 19. Dissemination / publication / missing evidence

F0.7 ensinou small-study effects e funnel limits.

GRADE pergunta se **missing evidence** plausivelmente deslocaria a conclusion relativa ao threshold/range.

Possíveis sinais:

- registry/results mismatches;
- unpublished studies;
- outcome non-reporting;
- selective timepoint/reporting;
- small-study pattern;
- sponsor/information-access context.

Funnel symmetry não prova ausência de dissemination bias.

Funnel asymmetry não prova sua presença.

---

# 20. Avoid double counting

Domains podem se sobrepor causalmente.

Exemplo:

- small high-risk studies mostram effects maiores;
- mesmo padrão gera apparent heterogeneity;
- same studies são mais likely unpublished when null.

Não aplique automaticamente três downgrades pelo mesmo mecanismo sem justificar que existem ameaças distintas.

Current GRADE principles enfatizam judgments explícitos, não checklist arithmetic.

---

# 21. Certainty é outcome/question-specific

Uma mesma intervention pode ter:

- high certainty para performance outcome;
- low certainty para rare harm;
- moderate certainty para adherence;
- very low certainty para long-term outcome.

Não escreva:

> “A evidência sobre Intervention X é high certainty.”

Sem dizer:

- para qual population;
- comparison;
- outcome;
- horizon/threshold.

---

# 22. Certainty ≠ effect magnitude

Compare:

### Evidence Body C

`MD +0.1 [0.0, 0.2]`, threshold importante `+1.0`, low RoB, direct, consistent.

Pode sustentar **high certainty de trivial effect**.

### Evidence Body D

`MD +3.0 [-1.5, 7.5]`, serious bias, indirectness, imprecision.

Pode ter large point estimate e **low/very-low certainty**.

Logo:

`large effect estimate ≠ high certainty`.

---

# 23. Recommendation strength é outra camada

Uma recommendation precisa integrar mais do que certainty de um outcome.

Pode considerar:

- balance desirable/undesirable effects;
- certainty across critical outcomes;
- values/preferences;
- resources/costs;
- equity;
- acceptability;
- feasibility;
- context.

Portanto:

`high certainty on one outcome ≠ strong recommendation`.

E strong recommendations podem, em contextos específicos, existir mesmo com limitations — desde que o decision reasoning justifique.

F0.8 ensina apenas a separação conceitual; formal guideline decision frameworks ficam fora do escopo principal.

---

# 24. Integrated evidence-body comparison

Target decision:

> Em trained adult endurance athletes, Intervention X versus control melhora standardized performance score após ~12 weeks? Higher = better. Practical benefit threshold = `+1.0` point.

Tudo abaixo é sintético.

## Evidence Body A

Four randomized parallel trials:

- target population predominantly trained adults;
- intervention/dose/duration muito próximas ao target;
- automated/blinded primary performance assessment;
- adequate randomization/concealment;
- low differential missingness;
- primary analyses consistent with registrations;
- pooled MD `+1.5 [1.2, 1.8]`;
- effects `+1.2`, `+1.4`, `+1.6`, `+1.7`;
- no material unexplained heterogeneity;
- search includes registries and unpublished-result contact attempts.

Reasoning:

- risk of bias: low concerns for the critical result across most weight;
- inconsistency: effects remain in same decision-relevant range;
- indirectness: small;
- imprecision: CI stays above +1.0 threshold;
- dissemination bias: no guarantee of absence, but no strong signal supplied.

Possible certainty: relatively high, if no unlisted concern changes the judgment.

Applicability: good to trained adult endurance athletes under similar delivery/context.

## Evidence Body B

Five non-randomized cohort studies:

- mostly recreational/untrained adults;
- Intervention X self-selected;
- higher baseline motivation/training volume strongly predicts X use;
- training volume measured crudely;
- completers-only analysis after differential dropout;
- subjective performance proxy in three studies;
- pooled transformed MD-equivalent `+1.6 [-0.2, 3.4]`;
- study estimates range `-0.3` to `+3.8`;
- larger estimates concentrated in short-duration studies;
- no prespecified moderator analysis;
- target is trained endurance athletes at 12 weeks, but most follow-up is 2–4 weeks.

Reasoning:

- risk of bias: confounding/selection/missingness concerns can materially move estimate;
- inconsistency: effects span different decision ranges;
- indirectness: population + follow-up + measurement differ from target;
- imprecision: CI crosses harm/trivial/meaningful-benefit ranges;
- dissemination bias: unresolved.

Possible certainty: materially lower than Body A despite similar point estimate.

Applicability: limited for trained endurance athletes at 12 weeks.

## Core lesson

Same point estimate does not imply same certainty.

`effect estimate` and `confidence in that estimate` are different objects.

---

# 25. Required 13-field F0.8 audit

Use this sequence:

`1. Target question/outcome → 2. Reporting visibility → 3. Design/effect of interest → 4. Result-level RoB mechanisms → 5. RoB judgment/rationale → 6. Body estimate + threshold → 7. Inconsistency → 8. Indirectness → 9. Imprecision → 10. Missing/dissemination evidence → 11. Overall certainty → 12. Applicability to target → 13. Recommendation-strength boundary`

Do not skip straight from study design to certainty label.

---

# 26. Critical fails

Reject these statements:

1. `CONSORT/STROBE/PRISMA complete = low risk of bias`;
2. `quality score 8/10 summarizes bias better than domain reasoning`;
3. `randomized = automatically low risk of bias`;
4. `observational = automatically high risk/unusable`;
5. `low certainty = no effect`;
6. `high certainty = large/important effect`;
7. `statistical significance = high certainty`;
8. `direct evidence = unbiased evidence`;
9. `representative sample repairs internal bias`;
10. `low I² = high certainty`;
11. `one high-risk study automatically downgrades one level`;
12. `GRADE certainty is a score for an individual paper`;
13. `high certainty for one outcome = strong recommendation`;
14. `applicable = internally valid`;
15. `ROBINS-I V2 Nov 2025 is finalized and stable`.

---

# 27. Active recall

Sem consultar a aula:

1. reporting completeness versus risk of bias;
2. risk of bias versus imprecision;
3. why RoB is result-specific;
4. five RoB 2 domains;
5. why randomization does not guarantee low RoB;
6. why a domain score should not be summed into quality total;
7. target-trial logic in ROBINS-I;
8. current ROBINS-I V2 status;
9. six V2 Nov-2025 conceptual domains;
10. four GRADE certainty categories;
11. five GRADE downgrading domains;
12. certainty versus effect magnitude;
13. inconsistency versus I²;
14. indirectness versus any mere PICO difference;
15. threshold-aware imprecision;
16. dissemination bias versus funnel asymmetry;
17. internal validity versus applicability;
18. certainty versus recommendation strength;
19. two ways RCT evidence can become low certainty;
20. two ways NRSI can remain informative;
21. compare the two integrated evidence bodies;
22. execute the 13-field F0.8 audit from memory.

---

# 28. Scope boundary

F0.8 does **not** require:

- memorizing every signalling question in RoB 2/ROBINS-I;
- running the official tools mechanically without training;
- scoring all GRADE subdomains exhaustively;
- advanced ROB-ME application;
- full Evidence-to-Decision guideline panel process;
- formal transportability estimators;
- network meta-analysis certainty;
- guideline recommendation authoring.

The target is structured appraisal and separation of concepts.

---

# 29. Source/version notes — rechecked 2026-09-09

## `F0-S07` — riskofbias.info

- RoB 2 main individually randomized parallel-group tool remains current version `22 August 2019`;
- cluster/crossover variants remain available separately;
- ROBINS-I V2 revised draft remains posted `20 November 2025` and explicitly subject to change;
- V2 Nov 2025 currently lists confounding, classification, selection into study, missing data, measurement and selection of reported result, with triage for Critical risk.

## `F0-S05` — Cochrane Handbook

Handbook landing page remains Version 6.5 (2024). Chapter 8 continues to describe RoB 2 as result-specific and domain-based for randomized trials.

## `F0-S18` — GRADE overview

Current living chapter last modified `12 May 2026`; retains four certainty categories and the core separation between certainty assessment and recommendations.

## `F0-S19` — GRADE certainty principles

Current chapter last modified `21 August 2025`; certainty is outcome/body specific and threshold/range aware, not a single-paper score.

## `F0-S20` — GRADE indirectness

Current chapter last modified `12 May 2026`; PICO mismatches matter when they plausibly create meaningful systematic differences in effect/absolute impact.

## Reporting contrast — `F0-S01`, `F0-S02`, `F0-S03`

CONSORT/STROBE/PRISMA remain reporting resources. This unit uses them only to block the false equivalence `complete reporting = low bias/high certainty`.

---

# 30. Regra final

Quando alguém disser “esse estudo é de alta qualidade” ou “essa evidência é forte”, não aceite a frase sem decompor:

> **qual result está sendo julgado, por quais bias mechanisms, qual body/outcome está recebendo certainty, em relação a qual threshold, e quão diretamente essa evidência corresponde ao target real de decisão?**
