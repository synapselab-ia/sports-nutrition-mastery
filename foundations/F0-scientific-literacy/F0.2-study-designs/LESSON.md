# F0.2 — Desenhos de estudo e o que eles podem responder

**Production state:** `APPROVED`

**Prerequisite P2:** F0.1 — perguntas científicas, hipóteses e operacionalização.

**P0 ensinados localmente:** alocação, seguimento, exposição, outcome, prospectivo, retrospectivo, unidade de alocação e unidade de análise.

**P1 ensinados localmente:** comparação within-subject versus between-subject; washout/carryover; dependência entre observações em clusters.

**Core sources:** `F0-S01`, `F0-S02`, `F0-S14`, `F0-S16`, `F0-S17`, `F0-S22`, `F0-S23`, `F0-S24`, `F0-S25`.

## 1. Competência-alvo

Ao terminar esta unidade, você deve conseguir olhar para uma pergunta e para a arquitetura de um estudo e responder:

1. **qual é o desenho?**
2. **o que foi alocado, observado ou comparado?**
3. **em que direção o tempo corre entre exposição/intervenção e outcome?**
4. **qual é a comparação relevante — entre pessoas/grupos ou dentro da mesma pessoa?**
5. **qual é a inferência mais forte que o desenho, por si só, torna defensável?**
6. **qual conclusão tentadora ainda não foi estabelecida?**

O objetivo não é decorar uma pirâmide de evidência. É aprender a raciocinar por estrutura.

A regra central desta unidade é:

> **desenho de estudo não é um selo de qualidade; é uma arquitetura que torna algumas perguntas mais diretamente respondíveis do que outras.**

F0.3 aprofundará por que uma estimativa pode ser distorcida por confounding, seleção, mensuração, missingness e outros mecanismos de viés. Aqui vamos apenas construir o esqueleto necessário para reconhecer essas ameaças depois.

---

## 2. O ponto de partida continua sendo a pergunta

F0.1 estabeleceu a sequência:

`pergunta → população → contraste → outcome → tempo → estimand`

F0.2 adiciona:

`→ desenho adequado → coleta/seguimento → análise → interpretação`

Se a pergunta é causal sobre uma intervenção, um desenho que cria um contraste de intervenção de maneira controlada pode ser apropriado. Se a pergunta é sobre prevalência, prognóstico, diagnóstico, efeitos raros ou exposições que não podem ser randomizadas de forma ética/prática, outro desenho pode ser mais informativo.

Por isso, a pergunta “qual desenho é melhor?” está incompleta.

A pergunta correta é:

> **melhor para estimar qual quantidade, em qual população, sob quais restrições?**

---

## 3. Vocabulário mínimo para ler um desenho

### 3.1 Intervenção versus exposição

**Intervenção** é uma condição deliberadamente aplicada ou atribuída como parte do estudo.

**Exposição** é uma característica, comportamento, estado ou condição que pode ser observada sem que o pesquisador a tenha atribuído.

Exemplos:

- intervenção: receber estratégia nutricional A ou B segundo protocolo;
- exposição: ingestão habitual de fibra observada na vida real;
- intervenção: executar protocolo de suplementação definido pelo estudo;
- exposição: uso espontâneo prévio de suplemento.

A mesma variável pode aparecer como intervenção em um estudo e como exposição em outro. O que muda é **como o contraste foi produzido**.

### 3.2 Alocação

**Alocação** é o processo que determina quem recebe qual condição/intervenção.

Em ensaios randomizados, a alocação é definida por um mecanismo aleatório. Em estudos não randomizados, ela pode depender de decisão clínica, preferência do participante, local, tempo, elegibilidade, disponibilidade ou outras regras.

### 3.3 Seguimento

**Seguimento** é o período em que participantes/unidades são observados para registrar outcomes após uma condição inicial, exposição ou intervenção.

### 3.4 Prospectivo e retrospectivo

Esses termos descrevem principalmente a relação entre o planejamento/observação do estudo e os dados utilizados — não substituem o nome do desenho.

Um **cohort retrospectivo** continua sendo cohort se a amostra é definida a partir de uma população/exposição no passado e os outcomes são reconstruídos em registros posteriores a esse ponto inicial.

Um **case-control** não vira “cohort” apenas porque usa registros antigos. O que o define é que a amostragem começa pelo **status de outcome** (casos e controles) e então compara exposições anteriores.

Esse é um erro de classificação muito comum.

### 3.5 Unidade de alocação, observação e análise

- **Unidade de alocação:** entidade que recebe a condição designada.
- **Unidade de observação:** entidade na qual o outcome é medido.
- **Unidade de análise:** unidade cuja dependência/estrutura é considerada na análise.

Em um ensaio individual simples, as três podem coincidir: pessoa → pessoa → pessoa.

Em um cluster trial, podem divergir:

- academias são randomizadas;
- atletas são medidos;
- a análise precisa reconhecer que atletas da mesma academia não são observações totalmente independentes.

A diferença entre essas unidades é parte do desenho, não detalhe burocrático.

---

## 4. Between-subject versus within-subject

### 4.1 Between-subject

Em uma comparação **between-subject**, pessoas diferentes fornecem os dados das condições comparadas.

Exemplo:

- grupo A recebe estratégia nutricional A;
- grupo B recebe estratégia B;
- comparamos outcomes entre grupos.

Um ensaio paralelo clássico é between-subject.

### 4.2 Within-subject

Em uma comparação **within-subject**, a mesma pessoa contribui com dados em mais de uma condição.

Exemplo:

- cada ciclista realiza um teste após estratégia A;
- o mesmo ciclista realiza outro teste após estratégia B;
- a comparação relevante é a diferença A versus B dentro de cada participante.

Isso pode reduzir o ruído produzido por diferenças estáveis entre pessoas, porque cada participante funciona como seu próprio controle.

Mas essa vantagem só é útil quando a condição anterior não altera de forma relevante a seguinte e quando o sistema estudado é suficientemente estável.

---

# 5. Ensaios randomizados

## 5.1 O que a randomização compra — e o que não compra

Randomização significa que a regra de alocação não escolhe conscientemente participantes com certas características para uma condição específica.

Em termos causais introdutórios, seu valor central é criar grupos que, **em expectativa**, sejam comparáveis quanto a características anteriores à intervenção, inclusive características não medidas.

Isso não significa que, em uma amostra finita, todos os valores basais ficarão numericamente iguais. Também não significa que todo problema posterior desaparece.

Randomização não garante, por si só:

- adesão perfeita;
- ausência de perdas de seguimento;
- cegamento possível;
- measurement perfeito;
- protocolo executado sem desvios;
- amostra representativa de toda população;
- outcome clinicamente/praticamente relevante;
- interpretação correta.

Esses problemas serão formalizados em F0.3 e F0.8.

A inferência correta nesta etapa é:

> **randomização fortalece a identificação de efeitos do contraste atribuído porque separa o mecanismo de alocação das características prévias dos participantes; não transforma automaticamente qualquer estimativa em verdade causal.**

---

## 5.2 Ensaio paralelo randomizado

### Estrutura

Participantes são randomizados para uma condição e permanecem nela durante o período de comparação principal.

Exemplo hipotético:

- 120 adultos treinados;
- randomização para estratégia A ou B;
- 12 semanas;
- outcome: mudança no 1RM.

### Comparação

**Between-subject:** A versus B entre grupos distintos.

### Perguntas que o desenho atende bem

- efeito da atribuição a A versus B no outcome definido;
- diferenças acumuladas durante um período em que crossover seria inadequado;
- intervenções com efeitos persistentes ou adaptações de longo prazo.

### Inferência mais forte defensável

Se conduzido e analisado adequadamente, sustenta uma estimativa do efeito causal do contraste randomizado para a população/condições estudadas.

### Inferência tentadora que não vem automaticamente

> “Como é RCT, o resultado vale para qualquer atleta, qualquer dose e qualquer duração.”

Não. O desenho fortalece validade interna do contraste; não apaga limites de população, intervenção, outcome e tempo.

---

## 5.3 Ensaio crossover randomizado

### Estrutura

Cada participante recebe duas ou mais condições em uma **sequência** definida, geralmente randomizada.

Um esquema simples é:

- sequência AB: A → washout → B;
- sequência BA: B → washout → A.

### Comparação

**Within-subject:** a pessoa é comparada consigo mesma.

### Quando faz sentido

Crossover é especialmente útil quando:

- o efeito da intervenção é relativamente rápido e reversível;
- o participante/condição é estável ao longo dos períodos;
- é plausível retornar a uma condição de base entre intervenções;
- o outcome pode ser repetido de modo comparável.

Em nutrição esportiva, isso pode ser útil para efeitos agudos em testes padronizados, desde que o primeiro protocolo não altere permanentemente o segundo.

### Washout

**Washout** é um período destinado a reduzir a persistência da condição anterior antes da seguinte.

Ele não é um ritual com duração universal. Precisa ser biologicamente suficiente para o efeito relevante que poderia persistir.

### Carryover

**Carryover** ocorre quando a condição de um período continua influenciando o período seguinte.

Se A ainda afeta o participante quando B começa, a comparação B versus A fica contaminada pela ordem/sequência.

### Period effect

Um **period effect** é uma diferença sistemática entre períodos que não é causada pela intervenção em si: aprendizado no teste, mudança no treinamento, progressão da condição, estação, fadiga acumulada etc.

### Quando crossover é inadequado

- hipertrofia produzida ao longo de semanas que não “desaparece” antes do próximo braço;
- vacinação ou intervenção irreversível;
- doença/condição que muda rapidamente ao longo do tempo;
- washout impossível ou capaz de gerar rebote relevante.

### Inferência mais forte defensável

Diferença entre condições **dentro das mesmas pessoas**, sob sequências/períodos adequados e com carryover suficientemente controlado.

### Inferência tentadora não estabelecida

> “Crossover é sempre superior ao paralelo porque controla diferenças individuais.”

Não. Se o efeito persistir, a condição mudar com o tempo ou a ordem importar, a própria arquitetura pode ser inadequada.

---

## 5.4 Cluster-randomized trial

### Estrutura

A unidade randomizada é um **grupo**: academia, escola, equipe, clínica, município, turma etc.

Exemplo hipotético:

- 20 equipes são randomizadas para programa nutricional A ou rotina usual;
- outcomes são medidos em 300 atletas.

### Por que randomizar clusters?

Pode ser necessário quando:

- a intervenção é aplicada coletivamente;
- randomização individual geraria contaminação entre participantes;
- a logística real opera no nível da equipe/instituição.

### Unidade de alocação versus unidade de análise

No exemplo:

- alocação = equipe;
- observação = atleta;
- análise = precisa reconhecer clustering por equipe.

Atletas da mesma equipe compartilham treinador, ambiente, rotina, alimentação institucional e várias influências. Tratar 300 atletas como se fossem 300 unidades randomizadas independentes ignora a arquitetura do experimento.

### Inferência mais forte defensável

Efeito do contraste **atribuído no nível do cluster**, respeitando a estrutura de dependência do desenho.

### Inferência tentadora não estabelecida

> “Foram 300 participantes; portanto houve 300 unidades independentes randomizadas.”

Não. O número de indivíduos observados não muda a unidade que foi randomizada.

---

## 5.5 Ensaio factorial randomizado

### Estrutura

Um factorial trial avalia dois ou mais **fatores/intervenções** no mesmo experimento.

No caso 2 × 2 com fatores A e B, há quatro combinações:

1. nem A nem B;
2. A sem B;
3. B sem A;
4. A + B.

Um participante é randomizado em relação a cada fator segundo o esquema do estudo.

### Por que usar

Permite investigar mais de uma intervenção usando o mesmo conjunto de participantes e pode ser eficiente para estimar efeitos de fatores quando a estrutura e as suposições são apropriadas.

### O ponto que costuma confundir

“Efeito de A” pode depender de B.

Se A funciona de um jeito sem B e de outro quando B está presente, existe **interação** entre fatores. F0.6 aprofundará problemas de múltiplas comparações; aqui basta entender que o desenho precisa declarar quais comparações são principais e como interação entra na pergunta.

### Inferência mais forte defensável

Pode estimar efeitos dos fatores randomizados e, quando planejado, investigar se o efeito de um fator varia conforme o outro.

### Inferência tentadora não estabelecida

> “Como A e B funcionaram separadamente, A+B necessariamente produz a soma dos dois efeitos.”

Não. Interações podem tornar a combinação diferente da soma simples.

---

# 6. Estudos de intervenção não randomizados

## 6.1 O que são

O pesquisador introduz ou acompanha uma intervenção, mas a alocação não é produzida por mecanismo aleatório.

Exemplos de regras de alocação:

- participante escolhe a estratégia;
- uma equipe adota o programa e outra não;
- protocolo muda em janeiro e resultados antes/depois são comparados;
- intervenção é determinada por disponibilidade, decisão clínica ou política local.

### O que podem mostrar diretamente

Dependendo da arquitetura, podem mostrar:

- que o outcome mudou após introdução da intervenção;
- que grupos expostos a estratégias diferentes apresentaram outcomes diferentes;
- que a intervenção precedeu temporalmente o outcome em um seguimento.

### O que não deve ser concluído automaticamente

A ausência de randomização significa que diferenças na alocação podem estar ligadas a diferenças entre participantes/contextos. Isso não torna todo estudo não randomizado “inútil” nem significa que causalidade jamais possa ser estudada com dados observacionais.

Significa que a inferência causal depende de **mais estrutura, dados e pressupostos** do que o rótulo “houve uma intervenção”. F0.3 ensinará exatamente como pensar nesses caminhos.

### Inferência mais forte defensável nesta unidade

Descrever a mudança/diferença observada sob uma intervenção não randomizada, preservando temporalidade e reconhecendo que atribuição causal exige justificativa adicional.

### Inferência tentadora não estabelecida

> “O grupo que escolheu a dieta A melhorou mais; portanto A causou a melhora.”

Essa conclusão ainda não foi garantida pela arquitetura de alocação.

---

# 7. Estudos observacionais analíticos

## 7.1 Cohort

### Estrutura

Uma cohort parte de pessoas classificadas por uma característica/exposição em um ponto inicial e observa outcomes que ocorrem depois.

Pode ser:

- **prospectiva:** o estudo define baseline agora e acompanha para frente;
- **retrospectiva:** registros existentes permitem reconstruir baseline/exposição e outcomes que ocorreram depois.

O princípio estrutural é:

`exposição/grupo inicial → tempo → outcome`

### O que faz bem

- estabelece ordem temporal quando exposição é conhecida antes do outcome;
- estima ocorrência/incidência em grupos acompanhados quando dados permitem;
- estuda múltiplos outcomes após uma exposição.

### Inferência mais forte defensável

Associação longitudinal entre exposição previamente definida e outcome posterior, com temporal ordering explícito.

### Inferência tentadora não estabelecida

> “A exposição veio antes do outcome, então necessariamente causou o outcome.”

Temporalidade é necessária para muitas relações causais, mas não é suficiente. Confounding e outros mecanismos ficam para F0.3.

---

## 7.2 Case-control

### Estrutura

A amostragem começa pelo **outcome**:

- casos = pessoas com o outcome;
- controles = pessoas sem o outcome ou representando a população que originou os casos;
- então compara-se a frequência/história de exposições anteriores.

O fluxo lógico é:

`selecionar por outcome → reconstruir exposição anterior`

Isso é diferente de uma cohort retrospectiva.

### Por que pode ser útil

É especialmente eficiente para outcomes raros ou com longa latência, porque o pesquisador não precisa acompanhar uma enorme cohort esperando poucos eventos aparecerem.

### Inferência mais forte defensável

Mostra se exposições anteriores estão diferencialmente representadas entre casos e controles adequadamente selecionados; sustenta medidas de associação apropriadas ao desenho.

### Inferência tentadora não estabelecida

> “60% dos casos foram expostos, então a exposição causa 60% de risco.”

Amostragem por outcome não fornece diretamente risco/incidência populacional dessa forma.

---

## 7.3 Cross-sectional

### Estrutura

Exposição e outcome são medidos em uma janela ou ponto de tempo essencialmente transversal.

Exemplo:

- dieta habitual atual;
- prevalência atual de sintomas;
- medidos na mesma avaliação.

### O que faz bem

- descreve prevalência;
- descreve distribuição de características;
- detecta associações contemporâneas;
- gera hipóteses.

### Limite estrutural central

Frequentemente não sabemos com segurança se a exposição precedeu o outcome.

Se atletas com maior fadiga relatam menor ingestão energética, duas histórias são compatíveis:

- menor ingestão antecedeu e contribuiu para fadiga;
- fadiga/rotina alterada levou a menor ingestão;
- ambos refletem outra condição.

F0.3 aprofundará reverse causation e confounding.

### Inferência mais forte defensável

Prevalência e associação no recorte temporal estudado.

### Inferência tentadora não estabelecida

> “X está associado a Y no levantamento; portanto X causa Y.”

---

# 8. Acute mechanistic versus chronic outcome studies

Este contraste é crucial em nutrição esportiva.

## 8.1 Estudo agudo mecanístico

Mede respostas próximas ao estímulo:

- sinalização molecular;
- síntese proteica em horas;
- glicemia pós-prandial;
- oxidação de substrato durante exercício;
- concentração hormonal aguda;
- performance em uma sessão.

Ele pode responder muito bem:

> “O que acontece durante ou logo após esta condição?”

Pode também testar mecanismos plausíveis.

## 8.2 Estudo crônico de outcome/adaptação

Acompanha mudanças acumuladas:

- hipertrofia em semanas/meses;
- força após ciclo de treinamento;
- composição corporal;
- incidência de lesão/evento;
- desempenho após intervenção longitudinal.

## 8.3 O erro de inferência

> “A intervenção aumentou um marcador anabólico por duas horas, portanto produzirá mais hipertrofia em 16 semanas.”

O primeiro resultado pode gerar ou sustentar uma hipótese mecanística, mas a conclusão crônica exige evidência que cubra a cadeia e o outcome de longo prazo.

### Inferência mais forte defensável

Agudo mecanístico → resposta aguda/mecanismo sob aquelas condições.

Crônico → mudança acumulada no outcome medido durante aquele horizonte.

### Inferência tentadora não estabelecida

Agudo ≠ crônico por definição.

---

# 9. Perguntas diagnósticas e prognósticas não são versões inferiores de RCT

Nem toda pergunta científica é “a intervenção causa melhora?”.

## 9.1 Diagnóstico

Pergunta típica:

> “Este teste distingue adequadamente quem tem e quem não tem determinada condição em relação a uma referência apropriada?”

A arquitetura frequentemente compara um teste índice com uma referência em pessoas avaliadas em janela próxima. O foco é classificação/accuracy, não o efeito de atribuir uma intervenção.

Um RCT não é automaticamente o desenho principal para estimar sensibilidade/especificidade de um teste.

## 9.2 Prognóstico

Pergunta típica:

> “Entre pessoas com um estado inicial definido, quais outcomes futuros ocorrem e quão bem características basais os predizem?”

Cohorts longitudinais são frequentemente naturais para esse problema porque partem de baseline e observam o futuro.

## 9.3 Predição não é causalidade

Uma variável pode prever um outcome sem ser uma causa manipulável do outcome.

Portanto:

> “prediz quem terá pior resultado” ≠ “intervir nessa variável melhorará o resultado”.

Essa distinção será importante mais tarde quando evidência aplicada for interpretada.

---

# 10. Target trial: usar um ensaio hipotético para clarificar uma pergunta causal observacional

Às vezes queremos responder uma pergunta causal de intervenção, mas um ensaio randomizado real não existe, é impraticável ou não pode ser realizado.

O **target trial framework** propõe começar especificando o protocolo do ensaio randomizado pragmático hipotético que responderia à pergunta causal.

Em versão introdutória, explicite:

1. critérios de elegibilidade;
2. estratégias comparadas;
3. como seria a alocação no ensaio-alvo;
4. início e duração do seguimento;
5. outcome;
6. contraste causal/estimand;
7. plano de análise coerente com esse alvo.

Depois, pergunta-se se dados observacionais permitem **emular** suficientemente essa arquitetura.

### O que isso ajuda a evitar

Obriga o pesquisador a explicitar decisões de design que poderiam ficar escondidas em uma análise observacional vaga: quando começa o seguimento, quem era elegível, qual estratégia está sendo comparada e qual outcome interessa.

### O que isso não faz

Emulação não cria randomização retrospectivamente.

O framework pode reduzir problemas produzidos por desenho mal especificado, mas não conserta dados inadequados nem elimina automaticamente confounding não medido.

A mecânica causal detalhada pertence a F0.3.

---

# 11. Por que “RCT > observational” é uma regra pobre

Uma hierarquia mecânica ignora a pergunta.

Considere:

### Pergunta A — efeito causal de uma estratégia de curto prazo

Um RCT adequado pode ser extremamente informativo.

### Pergunta B — prevalência de deficiência em determinada população

Um estudo transversal representativo pode responder melhor do que um RCT, porque não há intervenção a randomizar.

### Pergunta C — prognóstico em cinco anos

Uma cohort adequada pode ser a arquitetura natural.

### Pergunta D — efeito adverso raríssimo que aparece após anos

RCTs típicos podem ser pequenos/curtos demais; grandes bases observacionais podem fornecer sinal importante.

### Pergunta E — mecanismo agudo

Um pequeno crossover controlado pode responder um mecanismo fisiológico específico com grande eficiência, sem responder eficácia crônica.

Portanto:

> **adequação do desenho à pergunta vem antes do prestígio do rótulo.**

Isso não significa que todos os desenhos suportam a mesma inferência. Significa que a força de um desenho é sempre relativa ao estimand e ao problema.

---

# 12. Reporting guideline não é design e não é quality score

CONSORT e suas extensões dizem **o que deveria ser relatado** para tornar um ensaio compreensível e auditável.

STROBE faz o mesmo para cohort, case-control e cross-sectional.

PRISMA trata de relato de revisões sistemáticas.

Essas ferramentas ajudam você a localizar informação sobre o desenho. Elas não substituem raciocínio causal, avaliação de risco de viés ou julgamento de certeza.

Uma checklist preenchida não transforma um desenho inadequado em adequado.

---

# 13. Um algoritmo para identificar o desenho

Quando encontrar um estudo, responda nesta ordem.

## Passo 1 — qual é a pergunta?

- intervenção/efeito causal?
- associação?
- prevalência?
- prognóstico?
- diagnóstico?
- mecanismo agudo?
- adaptação crônica?

## Passo 2 — quem determinou a exposição/intervenção?

- pesquisador por randomização;
- pesquisador sem randomização;
- participante/contexto naturalmente.

## Passo 3 — por onde a amostragem começou?

- intervenção/exposição/baseline → cohort ou intervenção;
- outcome/caso-controle → case-control;
- recorte contemporâneo → cross-sectional.

## Passo 4 — quem foi randomizado?

- indivíduo;
- cluster;
- múltiplos fatores;
- sequência de condições na mesma pessoa.

## Passo 5 — mesma pessoa recebe mais de uma condição?

Se sim, pense em within-subject/crossover e pergunte por sequência, washout, carryover e period effects.

## Passo 6 — qual é a direção temporal?

O outcome veio depois da exposição? Foi medido simultaneamente? A exposição foi reconstruída após seleção por outcome?

## Passo 7 — qual é a unidade de alocação e qual é a de observação?

Se diferem, a estrutura de dependência precisa aparecer na análise.

## Passo 8 — escreva duas frases obrigatórias

1. **Inferência mais forte defensável:** “Este desenho sustenta...”
2. **Inferência tentadora não estabelecida:** “Este desenho, sozinho, não demonstra...”

Se você não consegue escrever as duas, ainda não entendeu o desenho.

---

# 14. Tabela de alta retenção

| Desenho | Como o contraste nasce | Tempo típico | Comparação | Inferência estrutural forte | Não estabelece automaticamente |
|---|---|---|---|---|---|
| RCT paralelo | randomização individual | longitudinal | between-subject | efeito do contraste randomizado sob condições estudadas | universalidade/ausência de outros problemas |
| Crossover randomizado | randomização de sequência; todos recebem condições | múltiplos períodos | within-subject | diferença entre condições na mesma pessoa | validade quando há carryover/efeito irreversível |
| Cluster RCT | clusters randomizados | longitudinal | entre clusters/indivíduos aninhados | efeito da atribuição no nível do cluster | independência de todos os indivíduos observados |
| Factorial RCT | randomização para ≥2 fatores | longitudinal | múltiplos contrastes | efeitos de fatores e possível interação | aditividade automática entre intervenções |
| Intervenção não randomizada | regra não aleatória | geralmente longitudinal | entre grupos/períodos | mudança/diferença temporal observada | causalidade só porque houve intervenção |
| Cohort | começa por exposição/baseline | longitudinal | expostos vs não expostos/grupos | associação com temporal ordering | causalidade apenas pela precedência temporal |
| Case-control | começa por outcome | reconstrução de exposição anterior | casos vs controles | associação de exposições prévias com status de caso | risco/incidência direta ou causalidade automática |
| Cross-sectional | recorte contemporâneo | transversal | grupos/variáveis no mesmo período | prevalência/associação contemporânea | ordem temporal/causalidade |

---

# 15. Checkpoints de recuperação ativa

Sem consultar acima:

1. Qual é a diferença estrutural entre cohort retrospectiva e case-control?
2. O que randomização melhora e o que ela não garante?
3. Por que crossover pode ser inadequado para hipertrofia de longo prazo?
4. Diferencie washout de carryover.
5. Em um cluster trial, por que 300 atletas não significam 300 unidades randomizadas?
6. O que um factorial 2 × 2 permite perguntar que um paralelo simples A versus B não permite tão diretamente?
7. Por que temporal ordering fortalece uma cohort sem provar causalidade?
8. Qual a inferência mais forte de um cross-sectional?
9. Por que um estudo agudo de sinalização não responde automaticamente uma pergunta de hipertrofia crônica?
10. O que target-trial emulation esclarece e o que ela não cria?

---

# 16. Resumo de domínio

Para F0.2, memorize menos rótulos e recupere este mapa:

`pergunta → origem do contraste → direção temporal → unidade de alocação → estrutura da comparação → outcome → inferência permitida → inferência proibida`

Os hábitos decisivos são:

- randomização é um mecanismo de alocação, não um certificado universal;
- cohort começa por exposição/baseline, case-control por outcome;
- cross-sectional é forte para prevalência/associação contemporânea, fraco para temporal ordering;
- crossover é within-subject e exige reversibilidade/controle de carryover;
- cluster exige distinguir unidade de alocação de unidade observada/analisada;
- factorial testa múltiplos fatores e precisa respeitar possíveis interações;
- intervenção não randomizada não é automaticamente causal nem automaticamente inútil;
- mecanismo agudo e outcome crônico são perguntas diferentes;
- desenho deve ser julgado contra a pergunta, não contra uma pirâmide abstrata;
- target-trial thinking explicita o ensaio causal que dados observacionais tentariam emular, sem fabricar randomização.

A competência desta unidade está demonstrada quando você consegue receber uma descrição nova e produzir, sem checklist mecânico:

> **“Este é o desenho; esta é a comparação; esta é a inferência mais forte; e esta é a conclusão que ainda seria exagerada.”**

---

# 17. Fontes e função pedagógica

- `F0-S01` — CONSORT 2025: padrão geral atual para relato de ensaios randomizados e referência para identificar arquitetura básica de trials.
- `F0-S02` — STROBE: relato de cohort, case-control e cross-sectional; usado como mapa de elementos observacionais, nunca como quality score.
- `F0-S14` — ICH E9/E9(R1): alinhamento entre objetivo, estimand, desenho e análise.
- `F0-S16` — Hernán & Robins, *Causal Inference: What If*: base conceitual para distinguir associação, experimento randomizado e pergunta causal.
- `F0-S17` — Hernán et al. 2025: target-trial framework; especificar primeiro o ensaio-alvo e depois avaliar se dados observacionais podem emulá-lo.
- `F0-S22` — Cochrane Handbook v6.5, Chapter 23: variantes de ensaios randomizados, especialmente cluster e crossover, unidade de análise, carryover e period effects.
- `F0-S23` — CONSORT crossover extension: características específicas de sequência, períodos e carryover em crossover trials.
- `F0-S24` — CONSORT cluster extension: requisitos específicos para unidade de randomização, fluxo de clusters/indivíduos e análise compatível com clustering.
- `F0-S25` — CONSORT factorial extension + explanation/elaboration: estrutura de 2 × 2, comparações principais e interação entre fatores.

As fontes de CONSORT/STROBE são guias de relato. Elas não são ferramentas de risco de viés e não autorizam ranking mecânico de desenhos.