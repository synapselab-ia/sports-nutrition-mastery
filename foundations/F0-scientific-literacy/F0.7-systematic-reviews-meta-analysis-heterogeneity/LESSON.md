# F0.7 — Revisões sistemáticas, meta-análises e heterogeneidade

**Production state:** `APPROVED_PENDING_QA`

**Prerequisites P2:** F0.2 — desenhos de estudo e limites de inferência; F0.5 — estimativas, intervalos de confiança, effect measures e relevância prática; F0.6 — multiplicidade, prespecification e flexibilidade analítica. F0.3 é fortemente recomendado antes de interpretar formalmente risk of bias dentro de uma síntese.

**P0 ensinados localmente:** systematic review, meta-analysis, eligibility criteria, study selection, data extraction, synthesis, effect-measure compatibility, study weight, pooled estimate, fixed-effect meta-analysis, random-effects meta-analysis, heterogeneity, clinical diversity, methodological diversity, statistical heterogeneity, I², sensitivity analysis, subgroup analysis, meta-regression, small-study effects, non-reporting/publication bias.

**P1 ensinados localmente:** inverse-variance weighting intuition; log-scale reminder for ratio measures; forest-plot anatomy; prediction-interval intuition; direct interaction reasoning for subgroup differences.

**Core/method sources:** `F0-S03`, `F0-S04`, `F0-S05`, `F0-S06`.

## 1. Competência-alvo

Ao terminar esta unidade, você deve conseguir abrir uma revisão sistemática/meta-análise e responder, em sequência:

1. qual pergunta e eligibility criteria definem o corpo de evidência?
2. como os estudos foram procurados, selecionados e extraídos?
3. quais estudos e resultados realmente alimentam cada síntese?
4. os effect measures e outcomes são suficientemente compatíveis para pooling?
5. o que cada marcador, intervalo, peso e diamond representa no forest plot?
6. qual quantity o modelo fixed-effect ou random-effects está resumindo?
7. qual heterogeneidade clínica, metodológica e estatística existe?
8. o que I² informa e, principalmente, o que ele **não** prova?
9. a média pooled continua cientificamente útil diante da diversidade observada?
10. subgroup/meta-regression/sensitivity analyses foram prespecified ou escolhidas depois dos resultados?
11. existem sinais de small-study effects ou missing evidence, e quais explicações alternativas permanecem?
12. PRISMA torna o processo visível, mas o que ainda precisa de appraisal separado?
13. qual conclusão final preserva magnitude + CI de F0.5 e multiplicidade/prespecification de F0.6?

Regra central:

> **Uma meta-análise é uma operação de síntese sobre estudos; ela não converte estudos incompatíveis ou enviesados em verdade por média. Antes de perguntar “qual é o pooled effect?”, pergunte “o que exatamente está sendo combinado, por que essas estimativas são comparáveis e que diversidade a média pode estar escondendo?”.**

---

# 2. Systematic review não é sinônimo de meta-analysis

## 2.1 Systematic review

Uma **systematic review** é um processo estruturado para responder uma pergunta por meio de métodos explícitos de:

- protocolo/pergunta;
- eligibility criteria;
- busca de estudos;
- seleção;
- extração;
- avaliação dos estudos/resultados;
- síntese;
- interpretação.

Ela pode terminar com:

- síntese narrativa estruturada;
- tabelas;
- gráficos;
- meta-analysis;
- ou uma combinação dessas formas.

## 2.2 Meta-analysis

Uma **meta-analysis** é a combinação estatística de resultados de dois ou mais estudos.

Logo:

`systematic review ≠ meta-analysis`

Uma revisão sistemática pode legitimamente concluir:

> “não faremos pooling porque os estudos não respondem a uma quantity suficientemente comum.”

Isso não é fracasso. Às vezes é a conclusão metodologicamente correta.

## 2.3 Uma meta-analysis sem processo sistemático também é possível

É possível alguém combinar numericamente alguns estudos escolhidos sem ter conduzido uma busca e seleção sistemáticas.

O número pooled pode parecer sofisticado, mas a seleção do que entrou pode ser enviesada.

F0.7, portanto, separa:

`qualidade/transparência do processo de revisão` de `matemática da combinação`.

---

# 3. O workflow de uma revisão sistemática

Use esta cadeia:

`Protocol/question → Eligibility → Search → Screening → Extraction → Study/result appraisal → Effect measure → Synthesis plan → Heterogeneity → Missing evidence → Interpretation`

## 3.1 Protocol e pergunta

Antes de ver quais estudos “dão certo”, a revisão deve definir claramente:

- população/contexto;
- intervenção/exposição e comparator;
- outcomes e time windows;
- desenhos elegíveis;
- análises/sínteses principais;
- moderators/subgroups importantes quando possível.

F0.6 já mostrou por que timing e prespecification importam. A mesma lógica vale para reviews.

## 3.2 Eligibility criteria

Eligibility criteria determinam o universo que a revisão pretende representar.

Perguntas:

- quais populações entram?
- qual intervention/exposure?
- qual comparator?
- quais outcomes?
- quais desenhos?
- quais durations/time points?
- idiomas/status de publicação foram restringidos?

Modificar critérios depois de conhecer resultados pode alterar o evidence body.

## 3.3 Search

Uma busca deve ser suficientemente sensível à pergunta e às fontes relevantes.

Em uma auditoria, procure:

- bases pesquisadas;
- registros/trial registries quando pertinentes;
- data da última busca;
- termos/estratégia reproduzível;
- restrições de idioma/publication status;
- busca de referências/citações ou fontes adicionais quando justificadas.

Não localizar evidência existente é uma forma de o corpo disponível deixar de representar o corpo real.

## 3.4 Screening

Screening responde:

> “quais registros/relatórios realmente correspondem a estudos elegíveis?”

Cuidado: um **study** pode gerar vários **reports**.

Contar artigos como se fossem estudos independentes pode duplicar participantes/resultados.

## 3.5 Extraction

Data extraction precisa preservar:

- desenho;
- sample;
- intervention/comparator;
- outcome definition;
- time point;
- effect measure;
- estimate;
- SE/CI ou informação equivalente;
- analysis population;
- dados necessários para unit-of-analysis issues;
- decisões de transformação/conversão.

Erros de extração podem criar heterogeneidade artificial ou pesos incorretos.

---

# 4. PRISMA: transparência, não certificado de qualidade

`F0-S03` é PRISMA 2020, a guideline de reporting para systematic reviews.

Ela organiza o que deve ser reportado sobre:

- objetivo;
- eligibility;
- information sources/search;
- selection;
- appraisal;
- synthesis;
- resultados;
- heterogeneity investigations;
- sensitivity analyses;
- protocol/registration;
- certainty e materiais relacionados.

PRISMA 2020 contém 27 itens, além de expanded checklist, abstract checklist e flow diagrams.

### PRISMA ajuda a perguntar

> “consigo ver o que os autores fizeram?”

### PRISMA não responde sozinho

> “o que eles fizeram foi metodologicamente correto e o evidence body tem low risk of bias?”

Critical distinction:

`PRISMA-complete ≠ low risk of bias ≠ high certainty`

Uma review pode reportar perfeitamente um método ruim.

F0.8 tratará formalmente risk of bias/certainty. Em F0.7, PRISMA é usado para tornar o processo auditável.

---

# 5. Antes de pooling: effect-measure compatibility

F0.5 ensinou MD, SMD, RD, RR e OR. Agora essas escolhas tornam-se estrutura de síntese.

## 5.1 Mesma pergunta não garante mesma escala

Exemplo:

- Study A: `MD = +2 unidades`;
- Study B: `SMD = +0.50`;
- Study C: `RR = 0.80`.

Não é válido simplesmente calcular:

`(+2 + 0.50 + 0.80) / 3`.

São quantities diferentes.

## 5.2 Compatibility exige mais do que converter números

Pergunte:

1. o outcome representa o mesmo construct?
2. maior/menor valor tem o mesmo significado?
3. os time points são comparáveis?
4. o effect measure responde ao mesmo contraste?
5. existe transformação/conversão metodologicamente defensável?
6. a unit of analysis foi respeitada?

## 5.3 MD versus SMD

- MD é adequado quando outcomes estão em unidade comparável;
- SMD pode permitir combinar escalas diferentes que medem um construct semelhante, mas padronização não torna constructs diferentes equivalentes.

SMD também herda a dependência da dispersion usada na padronização.

## 5.4 Ratio measures

RR e OR continuam diferentes.

Ratio measures costumam ser analisadas na log scale; isso preserva a geometria adequada em torno do null `1`.

Não converta OR em RR por hábito sem considerar baseline risk e método.

---

# 6. O que uma meta-analysis está fazendo matematicamente

Em forma simples:

> combinar estimates de estudos dando pesos diferentes a cada estimate.

A maior parte dos métodos é uma forma de weighted average.

Se os effects dos estudos forem `theta_i` e os weights `w_i`:

`pooled estimate ≈ Σ(w_i × theta_i) / Σw_i`

Isso não significa que o pooled estimate é a “média das pessoas”.

É uma média **de estimates**, sob um modelo de síntese.

---

# 7. P1 — inverse-variance weighting

## 7.1 Intuição

Um estimate com menor standard error contém mais informação estatística sobre sua target quantity.

Por isso, em um inverse-variance framework simples:

`weight ≈ 1 / variance = 1 / SE²`

Menor SE → maior weight.

## 7.2 O peso não mede qualidade

Um estudo pode ter:

- n enorme;
- SE pequeno;
- weight alto;
- e ainda assim ter bias relevante.

Logo:

`weight estatístico ≠ methodological quality ≠ certainty`

F0.3 continua valendo.

## 7.3 Exemplo

- Study A: `SE=0.20` → variance `0.04` → inverse variance `25`;
- Study B: `SE=0.40` → variance `0.16` → inverse variance `6.25`.

No mesmo fixed-effect inverse-variance framework, A receberia aproximadamente quatro vezes o peso de B.

Isso é precisão, não autoridade epistemológica.

---

# 8. Fixed-effect meta-analysis

Em uma interpretação comum do fixed-effect model:

> os estudos estão estimando o mesmo underlying intervention effect, e diferenças observadas decorrem de sampling variation.

Nesse framework, weights dependem principalmente da within-study variance.

### O pooled estimate responde

> “qual é o melhor estimate do common/typical effect sob esse modelo para os estudos incluídos?”

### Problema

Se os true effects realmente diferem materialmente por population, intervention, setting ou método, uma única common-effect quantity pode ser pouco defensável.

### Critical safeguard

Não escolha fixed-effect apenas porque um heterogeneity test “não foi significativo”.

Poucos estudos podem dar baixa capacidade de detectar heterogeneity.

---

# 9. Random-effects meta-analysis

Um random-effects model assume que os estudos podem estimar **effects diferentes, porém relacionados**, representáveis por uma distribution de effects.

O pooled estimate representa a **média dessa distribution assumida** para o conjunto/modelo.

## 9.1 Between-study variance

Além da within-study variance, o modelo incorpora uma estimate de between-study variance, frequentemente representada por `tau²`.

Intuição de weight:

`weight_i ≈ 1 / (SE_i² + tau²)`

Quando `tau²` aumenta:

- diferenças de weight entre studies podem diminuir;
- estudos menores tendem a receber relativamente mais weight do que receberiam em fixed-effect.

## 9.2 Random-effects não “resolve” heterogeneity

Critical rule:

> **Adicionar tau² ao modelo não transforma diversidade em irrelevância.**

Uma random-effects average pode ser precisa sobre o **mean effect** e ainda esconder ampla variation entre settings.

## 9.3 Fixed versus random não é campeonato

Não existe regra:

- fixed = errado;
- random = sempre melhor.

A escolha depende da target quantity e da plausibilidade do model.

A pergunta é:

> “qual quantity queremos resumir e quais assumptions tornam essa summary interpretable?”

---

# 10. Prediction interval — intuição útil

Em random-effects, o CI do pooled mean responde à uncertainty sobre a **média dos effects**.

Ele não mostra diretamente toda a spread de effects entre estudos/contextos.

Uma **prediction interval** tenta representar uma faixa na qual um effect de um novo estudo/contexto comparável poderia cair sob o model.

F0.7 não exige derivação matemática de prediction intervals.

A habilidade é reconhecer:

- `CI of pooled mean` e
- `between-study variation / prediction interval`

como objetos diferentes.

---

# 11. Forest plot: anatomia

Um forest plot normalmente contém:

1. nome/ID do study;
2. effect estimate de cada study;
3. marker (square/point) para o estimate;
4. horizontal line para o CI;
5. marker size relacionado ao weight em muitos plots;
6. vertical null line;
7. scale do effect measure;
8. pooled diamond quando há synthesis;
9. heterogeneity statistics;
10. subgroup labels quando aplicável.

## 11.1 Null line

- MD/SMD/RD: null geralmente `0`;
- RR/OR: null `1`.

## 11.2 Diamond

Centro:

- pooled point estimate.

Largura:

- pooled CI.

O diamond não é “a verdade”. Ele é o output do model aplicado aos inputs escolhidos.

---

# 12. Como ler um forest plot sem cair no threshold trap

A sequência F0.5 continua obrigatória.

Para cada study e para o pooled result:

`Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`

F0.7 adiciona quatro blocos:

`Compatibility → Weight/model → Heterogeneity → Synthesis defensibility`

Portanto, um forest plot deve ser lido assim:

1. qual effect measure?
2. qual null?
3. directions/magnitudes individuais;
4. CIs individuais;
5. weights;
6. pooled estimate/CI;
7. variability entre studies;
8. clinical/methodological differences;
9. model used;
10. se a pooled quantity faz sentido.

---

# 13. Heterogeneity: três camadas

## 13.1 Clinical diversity

Diferenças em:

- participants;
- baseline risk/status;
- intervention dose/form/duration;
- comparator;
- outcome definition;
- follow-up;
- setting.

Essas diferenças podem alterar o true effect.

## 13.2 Methodological diversity

Diferenças em:

- study design;
- allocation/blinding;
- measurement;
- analysis population;
- missing-data handling;
- risk of bias;
- unit-of-analysis treatment.

Isso pode produzir diferenças no observed effect até sem real effect modification.

## 13.3 Statistical heterogeneity

É a variation observada entre effect estimates que excede o esperado apenas por sampling error sob o model relevante.

Statistical heterogeneity pode refletir:

- real effect modification;
- methodological bias differences;
- measurement differences;
- extraction/analysis problems;
- combinação desses fatores.

Não existe tradução automática:

`heterogeneity = biological variability`.

---

# 14. I²: útil, mas facilmente abusado

I² é uma statistic que descreve, em termos aproximados, a proportion da variability observada entre effect estimates atribuível à heterogeneity em vez de sampling error no framework usado.

## 14.1 I² NÃO é

- percentual de studies “heterogêneos”;
- percentual do effect “explicado”;
- study-quality score;
- probabilidade de a meta-analysis estar errada;
- prova de que studies são equivalentes quando baixo;
- veto automático ao pooling quando alto.

## 14.2 Thresholds são rough guides

Cochrane fornece ranges aproximados, mas alerta que thresholds podem enganar.

A importância de I² depende de:

- magnitude/direction dos effects;
- quantidade de studies;
- uncertainty do I²;
- clinical/methodological context.

Com poucos studies, a estimate de heterogeneity pode ser muito incerta.

## 14.3 Dois traps

### Trap A

`I²=0% → todos os studies são iguais.`

Errado. Pode haver pouca informação para detectar variation e pode existir clinical/methodological diversity não refletida por I².

### Trap B

`I²=85% → meta-analysis é inválida por definição.`

Também errado. Pode haver uma meaningful average, subgroups legítimos ou uma synthesis útil, mas a heterogeneity precisa ser explicada/representada e a pooled mean pode não ser suficiente.

---

# 15. Quando NÃO fazer pooling

Meta-analysis deve ser considerada apenas quando os studies são suficientemente comparáveis para que a summary responda algo meaningful.

Sinais contra pooling incluem:

1. perguntas/estimands materialmente diferentes;
2. outcomes que parecem semelhantes mas medem constructs diferentes;
3. effect measures incompatíveis sem conversão defensável;
4. directions/scales invertidas ou mal harmonizadas;
5. clinical diversity tão ampla que uma average perde utilidade;
6. methodological diversity que sugere diferentes bias mechanisms dominantes;
7. data/extraction/unit-of-analysis problems não resolvidos;
8. mistura de time horizons que muda a scientific question;
9. tão poucos dados que o random-effects distribution/heterogeneity é mal estimado e a summary seria enganosa;
10. divergência de direção/magnitude que torna uma single number inadequada para decisão.

Importante:

> “não poolar” não significa “não sintetizar”.

A review ainda deve organizar e interpretar os evidence patterns de forma estruturada.

---

# 16. Sensitivity analysis

Uma **sensitivity analysis** pergunta:

> “a conclusão muda se uma assumption ou decisão razoável mudar?”

Exemplos:

- excluir studies com unit-of-analysis problem;
- fixed versus random-effects;
- diferentes reasonable effect conversions;
- excluir um study extremamente influential;
- usar alternative missing-data assumptions;
- restringir a um outcome definition mais consistente.

Sensitivity analysis não é:

> tentar infinitas versões até encontrar o resultado desejado.

F0.6 applies: ideally define important sensitivity analyses before outcomes direcionarem as escolhas e report all material variants.

---

# 17. Subgroup analyses em meta-analysis

Subgroups podem investigar effect modification por:

- population;
- dose/duration;
- setting;
- study design;
- outcome method;
- outras characteristics justificadas.

## 17.1 O erro que continua proibido

`subgroup A significant + subgroup B nonsignificant = subgroups differ`

Isso não prova interaction.

A pergunta correta exige uma direct comparison/interaction.

## 17.2 Prespecification

Um subgroup definido depois de observar a forest plot é diferente de um moderator prespecified por rationale científico.

Post hoc subgroup patterns podem gerar hypotheses.

Não devem ser apresentados como mecanismos comprovados de heterogeneity.

---

# 18. Meta-regression — conceito, não catálogo

Meta-regression relaciona study-level effect estimates a study-level characteristics.

Exemplo conceitual:

`effect estimate ~ intervention duration`

Pode perguntar se studies mais longos tendem a mostrar effects diferentes.

Limites críticos:

- normalmente há poucos studies;
- múltiplos candidate moderators criam multiplicity;
- study-level associations podem sofrer confounding;
- moderator distributions podem ser estreitas;
- post hoc model selection aumenta false-story risk;
- association não prova causal explanation da heterogeneity.

Logo:

`meta-regression pattern ≠ proven mechanism`.

---

# 19. Small-study effects e missing evidence

Uma review tenta representar **toda** evidência elegível, mas alguns studies/results podem estar missing.

Isso pode ocorrer quando dissemination/reporting depende de:

- direction;
- magnitude;
- p-value;
- perceived novelty.

## 19.1 Small-study effect

É o pattern em que smaller studies tendem a mostrar effects diferentes de larger studies.

Isso pode ocorrer por:

- non-reporting/publication bias;
- maior risk of bias em small studies;
- real clinical differences;
- artefatos do effect measure;
- chance.

Portanto:

`small-study effect ≠ publication bias proven`.

## 19.2 Funnel plot

Um funnel plot mostra effect estimates contra uma medida de precision/size.

Asymmetry pode levantar suspeitas, mas não diagnostica missing evidence sozinha.

Cochrane recomenda cautela: tests de funnel-plot asymmetry geralmente têm baixo power e são tipicamente considerados apenas quando há número suficiente de studies; a regra prática clássica é cerca de 10 ou mais studies para muitos desses tests.

Mesmo com ≥10, interpretation precisa considerar explicações alternativas.

## 19.3 Symmetry também não prova ausência de bias

Um funnel plot aparentemente symmetric não garante que todos os studies/results existem.

A evidence audit precisa combinar:

- search completeness;
- registries/protocols;
- known studies;
- selective outcome reporting;
- funnel/small-study patterns quando aplicável.

---

# 20. Publication bias versus non-reporting bias

“Publication bias” é um termo familiar, mas a missing-evidence problem é mais ampla.

Pode faltar:

- o study inteiro;
- um outcome;
- um time point;
- um subgroup;
- uma analysis;
- uma unfavorable estimate.

Por isso, F0.7 prefere perguntar:

> “qual evidence pode estar missing em função do resultado?”

em vez de procurar apenas journals que não publicaram estudos negativos.

Formal ROB-ME pertence à F0.8.

---

# 21. Worked example — weights

Considere cinco studies com o mesmo MD scale e SEs:

| Study | MD | SE |
|---|---:|---:|
| A | +0.2 | 0.35 |
| B | +0.5 | 0.40 |
| C | +1.1 | 0.30 |
| D | +2.4 | 0.45 |
| E | +3.0 | 0.50 |

Approximate inverse-variance weights em fixed-effect:

- A ≈ 23.7%;
- B ≈ 18.1%;
- C ≈ 32.2%;
- D ≈ 14.3%;
- E ≈ 11.6%.

Study C pesa mais porque tem menor SE.

Não porque seja automaticamente “melhor study”.

---

# 22. Worked example — heterogeneous forest plot

Synthetic software output para os cinco studies acima:

- fixed-effect pooled MD ≈ `+1.18`;
- heterogeneity: `I² ≈ 87%`;
- illustrative random-effects pooled MD ≈ `+1.40`;
- random-effects 95% CI ≈ `+0.44 a +2.36`.

Não memorize esses números.

A interpretação é:

1. individual effects variam de +0.2 a +3.0;
2. variation é grande em relação à within-study uncertainty;
3. random-effects average resume o centre de uma assumed distribution;
4. o pooled CI não representa toda between-study spread;
5. precisamos perguntar por que studies diferem antes de converter +1.40 em universal effect.

---

# 23. Worked example — duas explicações antes de subgroup story

Imagine que A–C recrutaram recreational athletes e D–E elite athletes.

Também imagine que:

- A–C usaram intervention duration de 2–4 weeks;
- D–E usaram 12 weeks;
- measurement setting também difere.

Forest plot mostra maiores effects em D–E.

Temos pelo menos três stories possíveis:

1. training status modifica o effect;
2. duration modifica o effect;
3. measurement/methodological differences produzem parte do pattern.

Se você escolher “elite athletes respondem melhor” só porque isso encaixa no pattern observado, está fazendo post hoc storytelling.

A análise correta:

- verificar prespecified moderators;
- avaliar collinearity entre study characteristics;
- olhar interaction/meta-regression com cautela;
- reconhecer poucos studies;
- manter hipóteses alternativas vivas.

---

# 24. Integrated review audit framework

Use estes **12 campos**:

`1. Review question → 2. Eligibility → 3. Search/selection → 4. Extraction/unit structure → 5. Effect measure compatibility → 6. Study estimates/precision → 7. Weight/model → 8. Clinical/methodological heterogeneity → 9. Statistical heterogeneity → 10. Sensitivity/subgroup/meta-regression prespecification → 11. Missing-evidence/small-study signals → 12. Pooling/conclusion defensibility`

## 24.1 Review question

O que exatamente a review quer estimar/sintetizar?

## 24.2 Eligibility

Que evidence universe foi definido?

## 24.3 Search/selection

Há chance material de studies/reports elegíveis terem sido perdidos ou selecionados por result?

## 24.4 Extraction/unit structure

Studies duplicados? Cluster/crossover/repeated measures tratados corretamente? Time points harmonizados?

## 24.5 Effect measure compatibility

Todos os estimates representam a mesma quantity ou houve conversão defensável?

## 24.6 Study estimates/precision

Magnitude + CI por study, preservando F0.5.

## 24.7 Weight/model

Qual model e qual lógica de weight?

## 24.8 Clinical/methodological heterogeneity

Quais diferenças substantivas existem?

## 24.9 Statistical heterogeneity

O que I²/Q/tau²/prediction information sugere sem threshold worship?

## 24.10 Exploration/prespecification

Subgroups/meta-regressions/sensitivity analyses eram planned? Quantos caminhos foram testados?

## 24.11 Missing evidence

Small-study/funnel patterns, protocols/registries e selective result availability sugerem o quê?

## 24.12 Pooling/conclusion

Poolar o quê, sob qual model, com qual caveat? Ou não poolar?

---

# 25. Integrated synthetic audit scenario

Uma systematic review avalia `Intervention X versus control` sobre um synthetic performance score; maior valor = melhor.

Protocol anterior à busca especificou:

- adult trained/recreational athletes;
- randomized parallel trials;
- primary outcome: performance score at 8–12 weeks;
- MD como preferred effect quando a mesma scale estivesse disponível;
- random-effects synthesis devido a expected clinical diversity;
- prespecified subgroup: trained versus recreational;
- sensitivity analysis excluindo high attrition.

Busca:

- quatro bibliographic databases;
- trial registry;
- sem language restriction;
- search date reportada.

Cinco studies usam a mesma scale:

| Study | Population / context | MD | 95% CI | SE |
|---|---|---:|---:|---:|
| A | recreational, 2–4 wk extension accepted by protocol amendment before extraction | +0.2 | −0.5 to +0.9 | 0.35 |
| B | recreational | +0.5 | −0.3 to +1.3 | 0.40 |
| C | trained | +1.1 | +0.5 to +1.7 | 0.30 |
| D | elite, different measurement setting | +2.4 | +1.5 to +3.3 | 0.45 |
| E | elite, different measurement setting | +3.0 | +2.0 to +4.0 | 0.50 |

Software reports:

- random-effects pooled MD `+1.4 [0.4,+2.4]`;
- `I²=87%`;
- fixed-effect estimate `+1.18`;
- strong difference in weights between fixed and random effects.

Sixth study F uses a different questionnaire/construct and reports `SMD=+0.60 [0.10,+1.10]`.

Authors propose adding `0.60` directly into the MD meta-analysis “because both favor intervention”.

After seeing I²=87%, they additionally test:

- duration `<8 vs ≥8 weeks`;
- elite vs non-elite;
- indoor vs outdoor;
- high vs low baseline score;
- one leave-one-out analysis per study.

They highlight elite status because subgroup interaction `p=0.04`, even though elite status is nearly collinear with measurement setting and was not prespecified.

Only five compatible studies exist, but authors draw a funnel plot and state:

> “The plot looks symmetric, proving no publication bias.”

Their report completes every PRISMA checklist item and concludes:

> “The meta-analysis proves Intervention X improves performance by approximately 1.4 units in athletes; high heterogeneity merely justifies random effects and does not affect interpretation.”

### Auditoria esperada

Uma resposta defensável deve identificar:

- systematic process strengths without turning PRISMA into quality certification;
- why Study F cannot be numerically appended as 0.60 to an MD synthesis;
- inverse-variance weight as precision, not quality;
- random-effects mean as an average, not universal effect;
- I²=87% as a signal requiring interpretation, not automatic invalidity;
- clinical/methodological alternatives for the heterogeneity;
- post hoc moderator multiplicity and collinearity;
- why subgroup p=0.04 does not prove a causal explanation;
- why funnel symmetry with five studies cannot prove absence of missing evidence;
- whether a pooled MD should be shown and, if shown, what caveats/alternative synthesis are required.

---

# 26. Critical-fail statements

Rejeite explicitamente:

1. `pooled estimate = automaticamente true/superior evidence`;
2. `I² baixo = studies clinically/methodologically identical`;
3. `I² alto = meta-analysis automaticamente inválida`;
4. `PRISMA completo = low risk of bias / high study quality`;
5. “se numbers favorecem o mesmo lado, MD/SMD/RR/OR podem ser pooled diretamente”;
6. `random effects resolves heterogeneity`;
7. `study weight = study quality`;
8. `significant subgroup + nonsignificant subgroup = interaction`;
9. post hoc subgroup/meta-regression pattern tratado como proven explanation;
10. funnel-plot symmetry tratado como proof of no publication bias;
11. funnel asymmetry tratado como proof of publication bias;
12. pooled p-value usado para substituir magnitude/CI/context;
13. fixed versus random escolhido apenas pelo p-value do heterogeneity test;
14. sensitivity analysis escolhida/reported apenas porque muda o conclusion favoravelmente;
15. meta-analysis usada para esconder that studies answer materially different questions.

---

# 27. Active recall

Sem consultar:

1. Diferencie systematic review e meta-analysis.
2. Dê o workflow mínimo de uma systematic review.
3. Por que um study pode ter múltiplos reports?
4. O que effect-measure compatibility exige antes de pooling?
5. Explique inverse-variance weighting.
6. Por que weight não é quality?
7. Defina fixed-effect em linguagem de target quantity.
8. Defina random-effects em linguagem de distribution/average effect.
9. O que tau² representa conceitualmente?
10. Diferencie pooled CI e prediction interval.
11. Identifique os elementos de um forest plot.
12. Diferencie clinical, methodological e statistical heterogeneity.
13. O que I² informa?
14. Cite cinco coisas que I² não informa.
15. Dê três situações em que pooling pode ser inadequado.
16. Defina sensitivity analysis.
17. Por que subgroup A significant/B nonsignificant não prova interaction?
18. O que meta-regression tenta fazer?
19. Por que post hoc moderator stories são frágeis?
20. Defina small-study effects.
21. Por que funnel asymmetry não prova publication bias?
22. Por que funnel symmetry não prova ausência de missing evidence?
23. O que PRISMA faz?
24. O que PRISMA não faz?
25. Execute os 12 campos do integrated audit sem consultar a lista.

---

# 28. Integração com F0.2, F0.5 e F0.6

## F0.2 fornece

- study-design architecture;
- unit-of-allocation/analysis awareness;
- inference boundaries.

## F0.5 fornece

- effect measures;
- estimate + CI;
- magnitude/practical meaning;
- ratio log-scale intuition.

## F0.6 fornece

- prespecification;
- multiplicity;
- analytical paths;
- subgroup interaction caution;
- transparency of deviations.

## F0.7 adiciona

- evidence-body assembly;
- weighted synthesis;
- heterogeneity;
- sensitivity/subgroup/meta-regression at review level;
- missing-evidence/small-study reasoning.

Nenhuma layer substitui as anteriores.

---

# 29. Limites deliberados

F0.7 não ensina em profundidade:

- derivation of Q/I²/tau² estimators;
- Hartung-Knapp, REML, Paule-Mandel ou exhaustive random-effects estimator catalog;
- network meta-analysis;
- individual-participant-data meta-analysis;
- multivariate/meta-analytic structural equation models;
- formal ROB-ME application;
- detailed publication-bias correction models;
- formal GRADE certainty judgments;
- recommendation formulation.

RoB/certainty/applicability formal entram em F0.8.

---

# 30. Fontes e função

## `F0-S03` — PRISMA 2020

Função:

- reporting transparency para systematic reviews;
- eligibility/search/selection/synthesis flow;
- protocol/registration, heterogeneity investigation e sensitivity reporting.

Limite:

- reporting guideline; não é risk-of-bias ou certainty score.

## `F0-S04` — Cochrane Handbook Chapter 10

Função:

- meta-analysis principles;
- inverse-variance weighting;
- fixed/random-effects;
- heterogeneity/I²/tau²;
- subgroups/meta-regression;
- sensitivity analyses;
- quando não poolar.

Version note rechecked 2026-09-09:

- chapter page cites Handbook v6.5 and chapter last update November 2024;
- Cochrane versions page records patch-level 6.5.1 changes through 2026, but none changes the F0.7 Chapter-10 teaching points used here.

## `F0-S05` — Cochrane Handbook current core methods

Função:

- systematic-review workflow across question, eligibility, search, synthesis and missing-evidence appraisal;
- current Chapter 13 supports introductory small-study/non-reporting-bias cautions.

Limit:

- Handbook chapters have different update dates; version literacy is required.

## `F0-S06` — Cochrane Chapter 6 effect measures

Função:

- compatibility of data types/effect measures;
- MD/SMD/RD/RR/OR scale logic;
- unit-of-analysis awareness;
- log scale for ratio measures.

---

# 31. Regra final

Ao encontrar uma meta-analysis, não pergunte primeiro:

> “qual o pooled effect?”

Pergunte:

> **qual evidence universe foi construído, que quantities entram na synthesis, como os studies foram weighted, que diversity existe, quais analytical choices foram prespecified, o que pode estar missing e se uma pooled average ainda representa uma scientific question útil?**
