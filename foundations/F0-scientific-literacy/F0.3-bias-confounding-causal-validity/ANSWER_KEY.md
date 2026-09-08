# F0.3 — Gabarito comentado

Este gabarito descreve respostas **aceitáveis** e os critérios de raciocínio esperados. Em questões abertas, redações diferentes podem receber pontuação integral se preservarem a estrutura causal correta.

O critério principal é:

> **definir a pergunta causal, identificar o mecanismo de distortion e limitar a conclusão de acordo com a informação realmente disponível.**

---

# Parte A — Recuperação ativa

## A1

**Random error** é variação amostral/measurement variation não sistemática que faz estimates oscilarem entre repetições. **Systematic error/bias** é um processo que desloca estruturalmente a estimate em relação ao target quantity/causal effect.

Aumentar sample size pode reduzir parte do random error, mas não elimina um processo sistematicamente errado.

## A2

Confounding ocorre quando uma causa comum anterior influencia exposição/intervenção e outcome, abrindo um caminho não causal entre eles.

Estrutura mínima:

```text
C ──► A
└───► Y
A ──► Y
```

Sem controle apropriado, parte da associação A–Y pode refletir `A ◄ C ► Y`, não o efeito A→Y.

## A3

**Residual confounding** é confounding que permanece após tentativa de controle.

Duas ou mais causas aceitáveis:

- confounder não medido;
- measurement error no confounder;
- categorização muito grosseira;
- proxy incompleto;
- modelagem inadequada;
- estrutura causal incompleta.

## A4

Para total causal effect:

- **confounder:** common cause de A e Y; frequentemente precisa ser bloqueado/controlado;
- **mediator:** causado por A e causa Y; faz parte do caminho do total effect e não deve ser automaticamente ajustado;
- **collider:** common effect de duas causas; conditioning pode abrir associação não causal.

O papel é específico à pergunta/estimand.

## A5

Porque associação estatística não define causal role. A variável pode ser:

- confounder que deve ser controlado;
- mediator cujo ajuste bloqueia parte do total effect;
- collider cujo ajuste abre bias;
- consequência da exposição;
- proxy mal medido.

“Mais covariáveis” não equivale a “menos bias”.

## A6

DAG representa **assumptions causais explícitas**: nós, relações direcionais, temporalidade/caminhos e possíveis adjustment sets.

Não prova que as setas estão corretas, que todos os confounders foram incluídos, que measurement é válido ou que o causal effect foi identificado.

## A7

Complete-case analysis condiciona implicitamente em “ter dado completo”. Se a probabilidade de ter dado completo depende de exposição/intervenção e de causas/outcomes relevantes, a analytical sample pode adquirir associação artificial e deixar de preservar o contraste original.

## A8

Porque o **mecanismo** de missingness importa mais que o percentual isolado. Dois braços podem perder 10% cada, mas um perder preferentially poor responders e outro perder pessoas por motivos não relacionados ao outcome. A seleção resultante é diferente.

## A9

Randomization ajuda a tornar assignment independente, em expectativa, de características pré-intervenção, reduzindo baseline confounding medido e não medido.

Problemas que não resolve automaticamente incluem:

- missing outcomes/attrition;
- nonadherence;
- differential co-interventions;
- measurement bias;
- outcome assessment sem blinding;
- inappropriate post-randomization selection;
- selective analysis/reporting;
- external validity.

## A10

**Internal validity:** se a estimate representa adequadamente o target effect/quantity nas pessoas/condições efetivamente estudadas.

**External validity/applicability:** até onde a inferência pode ser generalizada/transportada para outra população, intervenção, comparator, outcome, tempo ou contexto.

Um estudo pode ser internamente forte e externamente estreito.

---

# Parte B — DAGs, causal roles e adjustment

## B1 — Training load, suplemento e desempenho

### Target causal effect

Efeito total de `A` versus não-A/comparator definido sobre `Y` em 12 semanas na população-alvo.

### Papel de T

`T` é um **confounder/common cause** porque precede A e influencia tanto A quanto Y:

```text
A ◄── T ──► Y
```

### Se T não for controlado

A associação A–Y mistura o possível efeito A→Y com diferença de training load. Usuários de A podem ter melhor desempenho parcialmente porque treinam mais/melhor.

### T medido grosseiramente

Pode haver **residual confounding**. Ajustar uma versão mal medida de T não necessariamente fecha o caminho causal relevante.

### Randomization de A

Se implementada corretamente, randomization quebra, em expectativa, a ligação sistemática T→A no baseline. Portanto não é necessário identificar/ajustar cada confounder baseline para criar comparabilidade inicial do assignment.

Ainda podem surgir problemas pós-randomização.

**Pontuação completa:** common cause + residual confounding + benefício causal específico da randomization, sem afirmar validade total.

---

## B2 — Mecanismo intermediário

### Papel de M

`M` é **mediator**:

```text
A → M → Y
```

Ele participa do mecanismo pelo qual A afeta Y.

### Ajustar M para total effect

Não. Se o objetivo é total effect, conditioning em M bloqueia a parte mediada A→M→Y e muda o estimand.

### Quando M pode ser relevante

Em perguntas de direct effect/mediation, desde que o estimand seja redefinido e assumptions/métodos apropriados sejam usados.

Não é suficiente dizer “vamos ajustar M e pronto”; mediation analysis formal é mais complexa.

### Por que associação M–Y não basta

Porque causal role depende de temporalidade e estrutura, não de associação. Uma variável associada ao outcome pode ser confounder, mediator, collider ou apenas marcador.

**Falha crítica:** defender ajuste de M para total effect apenas porque M prediz Y.

---

## B3 — Seleção para grupo elite

### Papel de S

`S` é um **collider/common effect** de A e U:

```text
A → S ← U → Y
```

### Por que S=1 cria associação A–U

Ao condicionar em ser selecionado, saber que uma pessoa teve menor valor de uma causa de S torna, dentro da selected sample, mais provável que ela tenha maior valor de outra causa necessária para alcançar S=1. Isso pode tornar A e U associados apesar de não o serem na população de origem.

Como U causa Y, abre-se um caminho não causal A↔U→Y.

### Ajustar S dentro da amostra

Não resolve. Na amostra, S é constante (`S=1`) e o problema foi criado **pela seleção que definiu quem entrou no banco**. A informação sobre não selecionados e sobre U pode simplesmente não existir.

Correções exigiriam dados/assumptions sobre o selection process, não uma coluna S constante no modelo.

### Melhor decisão de design

Se a target population é “atletas elegíveis antes da seleção elite”, coletar/analisar essa população antes ou independentemente de S, ou obter dados que permitam modelar adequadamente o selection process.

**Ponto central:** seleção pode induzir collider bias; nem toda covariate pode ser “adjusted away” depois.

---

# Parte C — Mecanismos de bias e repairability

A pontuação completa exige os cinco componentes pedidos, não apenas nomear o bias.

## C1 — Reverse causation

### 1. Target causal question

Exemplo:

> Entre atletas comparáveis, reduzir habitual energy intake, versus manter ingestão suficiente definida, causa maior fadiga ao longo de uma janela temporal definida?

### 2. Causal structure

O survey permite pelo menos:

```text
Energy intake → fatigue
```

e também:

```text
Fatigue/illness/overreaching → appetite/intake
```

Além de common causes como training load ou illness.

### 3. Distortion mechanism

Exposure e outcome são medidos na mesma semana. Não há temporal ordering suficiente para distinguir causa de consequência. A associação pode refletir reverse causation ou confounding.

### 4. Repairability

**Melhorável por design:** medir intake antes do onset/change de fatigue; longitudinal follow-up; experimental contrast quando ético/viável; medir common causes.

**Não recuperável automaticamente:** o corte transversal não contém o passado causal que não foi coletado.

### 5. Calibrated conclusion

> “Lower intake and greater fatigue were associated in the same time window; the data do not establish whether lower intake caused fatigue, fatigue reduced intake, or both reflect other factors.”

---

## C2 — Differential measurement

### 1. Target causal question

Efeito de assignment ao suplemento versus control sobre recuperação subjetiva no horizonte definido.

### 2. Causal structure

```text
Assignment → expectation → reported recovery
Assignment → true recovery → reported recovery
Evaluator knowledge → recorded outcome
```

### 3. Distortion mechanism

Knowledge/expectation difere por grupo e pode alterar tanto experiência/reporting quanto observer recording. A diferença medida pode misturar intervention effect com differential outcome measurement/placebo-expectancy process, dependendo do estimand.

### 4. Repairability

**Design:** blinding/placebo adequado quando possível; standardized scripts; blinded assessors; validated outcome procedure; objective corroborating measures se representarem o construct.

**Limite:** depois de coleta com differential measurement sem validation data, não há garantia de decompor true effect e reporting/observer bias.

### 5. Calibrated conclusion

> “Because outcome assessment was unblinded and expectation differed between groups, the observed subjective recovery difference may not represent only the causal physiological effect of the supplement.”

---

## C3 — Attrition por tolerabilidade

### 1. Target causal question

Efeito do assignment/início de A versus placebo sobre performance em toda a randomized population no período definido.

### 2. Causal structure

Uma estrutura plausível:

```text
A → GI symptoms → dropout/observed outcome
GI symptoms → worse training/performance
```

Também podem existir prognostic factors → dropout e performance.

### 3. Distortion mechanism

Completer analysis condiciona em permanecer observado. Se permanência depende de treatment-related symptoms e fatores prognósticos, a analyzed sample deixa de refletir o contraste randomizado inicial.

### 4. Repairability

**Design:** retenção; continuar outcome collection após intervention discontinuation quando possível; registrar razões; minimize losses.

**Analysis:** métodos apropriados e sensitivity analyses sob assumptions podem ajudar.

**Limite:** outcomes nunca observados e determinantes não medidos de dropout deixam incerteza que não pode ser removida sem assumptions.

### 5. Calibrated conclusion

> “Randomization supports baseline comparability, but differential treatment-related attrition and completer-only analysis can bias the final performance estimate.”

---

## C4 — Exposure misclassification

### 1. Target causal question

Efeito de sustained/habitual high versus low protein intake, definido operacionalmente, sobre performance ao longo de dois anos.

### 2. Causal structure

```text
True habitual intake → measured one-day recall category
True habitual intake → outcome
Measurement error → incorrect exposure category
```

### 3. Distortion mechanism

Uma única memória de “dia típico” pode não representar habitual exposure por dois anos; pessoas são classificadas incorretamente e exposure pode mudar durante follow-up.

Direction do bias não deve ser assumida automaticamente.

### 4. Repairability

**Design/measurement:** repeated dietary measures, validated instruments, objective biomarkers quando apropriados, update exposure over time, validation subsample.

**Analysis:** correction/sensitivity methods podem ajudar se measurement-error parameters forem informativos.

**Limite:** sem validation/repeated data, true habitual exposure pode não ser recuperável de forma confiável.

### 5. Calibrated conclusion

> “The cohort can estimate an association using the measured baseline category, but causal interpretation for habitual two-year intake is limited by potentially substantial exposure misclassification and exposure change.”

---

## C5 — Residual confounding

### 1. Target causal question

Efeito de iniciar/usar X versus não usar X sobre performance sob estratégias comparáveis de training.

### 2. Causal structure

```text
Training quality/volume/commitment → X use
Training quality/volume/commitment → performance
```

“Days/week” é um proxy incompleto.

### 3. Distortion mechanism

Adjustment fecha apenas parte da informação sobre training. Differences em volume, intensity, coaching e commitment podem continuar ligadas a X e Y.

### 4. Repairability

**Melhorável:** measure confounders melhor no design; repeated/validated training data; randomization de X quando viável.

**Analysis:** richer measured covariates/sensitivity analyses podem melhorar avaliação.

**Não garantido:** unmeasured aspects não são magicamente removidos pelo modelo atual.

### 5. Calibrated conclusion

> “The adjusted association remains vulnerable to residual confounding because training was measured incompletely; it does not by itself identify the effect of initiating X.”

---

# Parte D — Randomization + target-trial thinking

## D1 — “É RCT, então acabou”

### 1. Problema baseline reduzido — 1 ponto

Randomization reduz systematic baseline confounding da assignment: características pré-intervenção, medidas e não medidas, não deveriam determinar treatment assignment exceto por chance.

### 2. Três ameaças pós-randomização — 3 pontos

Qualquer três bem explicadas:

- differential missing outcomes/attrition;
- unblinded outcome measurement;
- adherence-based selection;
- possible collider/selection bias from conditioning on adherence;
- loss of initial group comparability;
- estimand shift from effect of assignment to effect among selected adherers.

### 3. Apenas >90% adherent — 2 pontos

Adherence é pós-randomização e também depende de baseline motivation. Ao selecionar apenas highly adherent participants, a análise condiciona em um processo influenciado por treatment experience e prognostic factors. Os grupos que restam podem não preservar a comparabilidade randomizada.

### 4. Calibrated sentence — 1 ponto

Exemplo:

> “Although randomization supports baseline causal comparability of assignment, differential missingness, unblinded assessment and adherence-based selection can materially bias the reported completer/adherent estimate.”

**Falha crítica:** “Como foi randomizado, esses problemas só afetam generalização, não o causal effect.”

---

## D2 — Target trial observational

Há várias respostas válidas. Avaliar coerência interna.

### 1. Pergunta precisa — 2 pontos

Exemplo:

> Em corredores recreacionais adultos que treinam ≥3 vezes/semana e não usam habitualmente cafeína pré-treino, iniciar uma estratégia padronizada de café/cafeína 45 minutos antes das sessões-chave, comparado a não usar cafeína pré-treino, altera a mudança em um teste padronizado de performance após seis meses?

Não é necessário usar exatamente essa population/dose/horizonte; precisam estar definidos.

### 2. Target trial — 3 pontos

Exemplo:

- **Eligibility:** corredores recreacionais adultos, critérios pré-definidos, baseline antes da estratégia.
- **Strategies:** cafeína/café pré-treino segundo protocolo versus no-caffeine strategy.
- **Time zero:** momento hipotético da assignment, coincidente com eligibility e início de follow-up.
- **Outcome/follow-up:** mudança em standardized performance test após seis meses.
- **Causal contrast:** diferença no outcome sob assignment às duas estratégias, com estimand explicitado.

### 3. Duas divergências observacionais — 2 pontos

Exemplos:

- habitual users já diferem em training/sleep/motivation;
- exposure começa antes do baseline observado;
- time zero é mal definido;
- dose/timing variam;
- adherence/switching não são medidos;
- confounders relevantes ausentes;
- outcome measurement não coincide entre grupos;
- seleção exige sobrevivência/participação até um ponto futuro.

### 4. Limite — 1 ponto

O framework especifica o causal design-alvo e ajuda a alinhar dados, mas não randomiza retrospectivamente, não cria exchangeability e não mede confounders que o banco nunca coletou.

---

# Parte E — Caso integrativo de sports nutrition

## 1. Target question/estimand — 2 pontos

Exemplo:

> Entre corredores recreacionais elegíveis no baseline, qual é o total causal effect de iniciar e seguir uma estratégia definida de suplemento Z, versus não usar Z, sobre a mudança no time padronizado de 10 km em seis meses?

Resposta completa deve definir population, strategy/comparator, outcome/time e deixar claro que o alvo é causal, não apenas association entre current users e nonusers.

## 2. DAG verbal/setas — 2 pontos

Exemplo aceitável:

```text
Training load/quality ──► Z use ──► Body-mass change ──► 10-km performance
        │                    │
        ├───────────────────► performance
        └──► injury ──► observed at follow-up

Coaching quality ──► Z use
Coaching quality ──► performance
```

Elementos esperados:

- **confounder:** training load/quality e/ou coaching quality;
- **possible mediator:** body-mass change se Z pode causá-la e ela causa performance;
- **selection node:** ter outcome final / completar follow-up, influenciado por injury e talvez outros fatores.

## 3. Dois adjustment problems — 2 pontos

Respostas possíveis:

### Inadequate confounder adjustment

Ajustar só “training days/week” pode deixar residual confounding por volume/intensity/coaching/commitment.

### Adjusting possible mediator

Se o alvo é total effect, ajustar body-mass change pode bloquear parte do caminho Z→body mass→performance e mudar o estimand.

### Conditioning on completers

Analisar apenas quem realizou novo 10 km condiciona em follow-up observation. Como injury depende de high training load e remove pessoas do outcome, a analytical sample pode ser selected com relação a prognostic factors.

Qualquer dois com mecanismo correto recebem pontuação.

## 4. Repairable vs unrecoverable — 2 pontos

Exemplo:

- **Mitigável sob assumptions:** modelar observed selection/missingness com dados ricos, usar appropriate missing-data methods/sensitivity analysis, ou melhorar adjustment usando measured confounders realmente disponíveis.
- **Não garantidamente recuperável:** coaching quality, training volume/intensity ou outros confounders nunca medidos não podem ser reconstruídos com certeza; true outcomes de pessoas perdidas também não são conhecidos sem assumptions/informação adicional.

A resposta precisa distinguir “método possível” de “verdade recuperada”.

## 5. Calibrated conclusion — 2 pontos

Exemplo:

> “Z use was associated with faster 10-km performance among runners with observed follow-up, but the causal interpretation is limited by residual confounding from incompletely measured training/coaching, selection related to injury/follow-up, and possible overadjustment for post-exposure body-mass change. The data do not establish that initiating Z would cause the reported improvement without additional causal assumptions.”

**Falha crítica:** aceitar “causes faster running” apenas porque o modelo foi multivariable-adjusted.

---

# Rubrica de correção

## 90–100

Raciocínio causal estável. O estudante:

- começa pelo estimand;
- desenha/explica estruturas causais sem depender de labels;
- distingue confounder/mediator/collider pelo papel e tempo;
- identifica selection/missingness como processos;
- separa measurement de causal adjustment;
- reconhece o que randomization resolve e o que não resolve;
- distingue repairable from unavailable information;
- escreve conclusões calibradas.

## 80–89

Competência suficiente para avançar. Pode haver pequenas imprecisões terminológicas, mas adjustment decisions e causal limits permanecem corretos.

## 70–79

Compreensão parcial. Requer correção dirigida, especialmente se houver tendência a:

- selecionar covariáveis por associação;
- esquecer temporal ordering;
- tratar missingness por percentual;
- subestimar post-randomization selection.

## <70

A estrutura causal ainda não está estável. Revisar F0.3 e resolver novos DAGs/casos equivalentes antes de depender desses conceitos em F0.7/F0.8.

---

# Falhas críticas

Mesmo com nota total alta, não considerar F0.3 aplicado se o estudante:

- trata DAG como evidência de que uma relação existe;
- confunde adjustment quantity com adjustment quality;
- condiciona collider como regra de “controle”;
- bloqueia mediator sem perceber que mudou o total-effect estimand;
- considera randomization proteção contra toda forma de bias;
- chama target-trial emulation de randomized trial;
- ignora reverse causation quando temporal ordering é ambígua;
- usa missing-data percentage como único critério de bias;
- afirma que unmeasured confounding foi eliminado sem informação/assumptions capazes de sustentá-lo.

Esses erros atingem diretamente `K4`, `K5`, `K6`, `K7` e `K8` e devem ser corrigidos antes de formal risk-of-bias/certainty appraisal em F0.8.