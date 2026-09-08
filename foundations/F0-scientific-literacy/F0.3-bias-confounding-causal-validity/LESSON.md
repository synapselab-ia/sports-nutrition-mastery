# F0.3 — Viés, confounding, raciocínio causal e validade

**Production state:** `APPROVED`

**Prerequisites P2:** F0.1 — perguntas científicas, hipóteses e operacionalização; F0.2 — desenhos de estudo e limites de inferência.

**P0 ensinados localmente:** bias/viés, confounder, mediator, collider, selection, information bias, measurement error, misclassification, missingness, attrition, reverse causation, internal validity, external validity, generalizability, transportability/applicability.

**P1 ensinados localmente:** intuição contrafactual; directed acyclic graphs (DAGs) simples; caminhos causais versus não causais; ajuste como operação que depende do estimand e da estrutura causal.

**Core sources:** `F0-S07`, `F0-S11`, `F0-S14`, `F0-S16`, `F0-S17`, `F0-S26`.

## 1. Competência-alvo

Ao terminar esta unidade, você deve conseguir receber uma associação ou estimativa de efeito e perguntar, antes de acreditar nela:

1. **qual é a pergunta causal exata?**
2. **qual contraste/estimand está sendo buscado?**
3. **como o desenho criou ou observou esse contraste?**
4. **quais caminhos podem produzir associação sem representar o efeito causal de interesse?**
5. **quais variáveis são confounders, mediators ou colliders para essa pergunta específica?**
6. **qual seleção, mensuração ou missingness pode distorcer a estimativa?**
7. **o que randomização resolveu e o que continuou vulnerável?**
8. **qual problema pode ser prevenido ou mitigado por desenho, mensuração ou análise — e qual informação simplesmente não existe nos dados?**
9. **a conclusão vale internamente para o estudo e, separadamente, até onde pode ser transportada para outra população/contexto?**
10. **que grau de certeza verbal é compatível com as assumptions que ainda precisam ser verdadeiras?**

A regra central é:

> **um número observado pode estar errado não apenas por acaso, mas porque o processo que gerou, selecionou, mediu ou analisou os dados desviou sistematicamente a estimativa do alvo causal.**

F0.4–F0.6 ensinarão a parte quantitativa de random error, precisão, intervalos, testes e multiplicidade. F0.8 ensinará formalmente risk-of-bias tools e certeza de corpos de evidência. Nesta unidade, o objetivo é construir o **modelo causal de raciocínio** que torna esses módulos possíveis.

---

## 2. F0.1 + F0.2 + F0.3: da pergunta à ameaça de validade

F0.1 construiu:

`pergunta → população → contraste → outcome → tempo → estimand`

F0.2 acrescentou:

`→ desenho → alocação/observação → seguimento → comparação → limite de inferência`

F0.3 pergunta:

`→ por quais mecanismos a estimativa pode se afastar do efeito/quantidade-alvo?`

Isso muda a forma de ler um estudo. Em vez de perguntar apenas “é RCT?” ou “ajustou covariáveis?”, você passa a perguntar:

- o desenho identifica o contraste que interessa?
- a seleção da amostra/analítica depende de fatores ligados à exposição e ao outcome?
- exposição, outcome e covariáveis foram medidos de forma comparável?
- perdas mudaram quem continua observável?
- a análise condicionou em variável que deveria ficar aberta ou fechou caminho que fazia parte do efeito de interesse?
- existe confounding não medido ou medido de forma inadequada?
- o tempo permite causa antes de efeito?

A palavra **bias** não é uma acusação moral ao pesquisador. É um conceito técnico sobre **desvio sistemático**.

---

# 3. Associação, efeito causal e a intuição contrafactual

## 3.1 O problema básico

Suponha que a pergunta seja:

> Em adultos treinados, qual seria o efeito de seguir estratégia nutricional A, comparada a estratégia B, sobre o desempenho após 12 semanas?

Para uma pessoa específica, o ideal causal seria conhecer dois resultados:

- o desempenho que ela teria **se seguisse A**;
- o desempenho que a mesma pessoa teria **se, nas mesmas condições relevantes, seguisse B**.

Mas, no mesmo período histórico, a pessoa não pode viver simultaneamente as duas versões completas. Observamos um dos resultados; o outro é **contrafactual**.

Podemos representar a intuição como:

- `Y(A)` = outcome que ocorreria sob A;
- `Y(B)` = outcome que ocorreria sob B.

O efeito causal individual seria algo como a diferença entre esses dois outcomes potenciais. Como não observamos ambos na mesma pessoa ao mesmo tempo, pesquisa causal precisa usar desenho e assumptions para construir comparações que funcionem como aproximações válidas do contraste contrafactual.

Você não precisa dominar notação formal nesta etapa. Precisa entender a consequência:

> **uma diferença observada entre pessoas expostas e não expostas só representa efeito causal se os grupos forem comparáveis nos aspectos necessários para aquele contraste.**

## 3.2 Exchangeability em linguagem simples

Uma ideia central de causal inference é **exchangeability**: para o contraste causal desejado, os grupos comparados precisam ser intercambiáveis quanto ao outcome que teriam sob as estratégias alternativas, condicionado ao que o desenho/análise exige.

Em linguagem operacional:

> Se eu trocasse as estratégias entre grupos sem mudar mais nada causalmente relevante, eu esperaria outcomes comparáveis exceto pelo efeito da estratégia?

Randomização tenta criar essa propriedade na origem da alocação. Estudos observacionais precisam justificá-la por design, mensuração e assumptions adicionais.

Não transforme “exchangeability” em palavra mágica. A pergunta real é: **quais causas compartilhadas ou mecanismos de seleção tornam os grupos não comparáveis?**

---

# 4. Random error versus systematic error

## 4.1 Random error

**Random error** é variação que faz a estimativa oscilar entre amostras mesmo quando o processo de estudo não tem um desvio sistemático específico.

Exemplos intuitivos:

- duas amostras pequenas sorteadas da mesma população terão médias um pouco diferentes;
- um teste de desempenho varia de sessão para sessão mesmo com protocolo estável;
- um grupo randomizado pode, por acaso, ter baseline numericamente diferente do outro.

A linguagem quantitativa de sampling variation, standard error, confidence intervals e power será ensinada em F0.4–F0.6.

## 4.2 Systematic error / bias

**Systematic error (bias)** é uma tendência do processo de estudo a deslocar a estimativa em determinada direção ou de forma estruturalmente não aleatória em relação ao alvo de interesse.

Exemplos:

- pessoas mais motivadas têm maior chance de usar o suplemento e também de treinar mais;
- participantes com pior resposta abandonam mais um braço e somem do outcome final;
- quem sabe que recebeu intervenção relata sintomas de forma diferente;
- a análise condiciona em um collider e cria uma associação que não existia na população-alvo.

## 4.3 “Aumentar n” não é tratamento universal

Um estudo enorme pode reduzir random error e ainda estar sistematicamente errado.

Imagine uma balança que sempre adiciona 2 kg. Pesar 10.000 pessoas não elimina o erro de calibração. Você pode obter uma estimativa **muito precisa do valor errado**.

Em pesquisa causal:

- aumentar amostra pode melhorar precisão;
- não recupera automaticamente confounder não medido;
- não desfaz seleção inadequada;
- não corrige um outcome medido por instrumento sistematicamente enviesado;
- não cria temporalidade que o desenho não possui.

Esse contraste será crucial quando F0.5 ensinar precisão: **precisão e validade são propriedades diferentes**.

---

# 5. Confounding: uma causa alternativa para a associação

## 5.1 Definição causal

Para uma pergunta causal sobre exposição/intervenção `A` e outcome `Y`, um **confounder** é, conceitualmente, uma causa anterior que influencia tanto `A` quanto `Y` ou abre um caminho não causal relevante entre eles.

Estrutura simples:

```text
C ──► A
│
└──► Y

A ──► Y   (efeito causal que queremos estimar)
```

O caminho `A ◄── C ──► Y` produz associação entre A e Y mesmo sem passar pelo efeito causal de A sobre Y.

## 5.2 Exemplo em nutrição esportiva

Pergunta:

> Uso habitual de suplemento X melhora desempenho em corrida?

Observação:

> Usuários de X correm mais rápido.

Possível confounder:

**volume/qualidade de treinamento**.

É plausível que atletas mais comprometidos:

- treinem com maior volume/estrutura;
- sejam mais propensos a comprar/usar suplementos;
- tenham melhor desempenho por causa do treinamento.

Então:

```text
Comprometimento/treino ──► uso de X
          │
          └──────────────► desempenho
```

A associação `uso de X ↔ desempenho` não identifica sozinha o efeito do suplemento.

## 5.3 Temporalidade importa

Um candidato a confounder para o **efeito total** normalmente precisa existir causalmente antes da exposição ou não ser consequência dela.

Se A causa M, e M causa Y, M não é simplesmente “mais uma covariável que pode confundir”. M pode ser um **mediator**.

Esse é um motivo para abandonar regras puramente estatísticas como:

> “Se a variável está associada a exposição e outcome, ajuste.”

Associação não define papel causal.

## 5.4 Residual confounding

**Residual confounding** é confounding que permanece depois de uma tentativa de controle.

Pode acontecer porque:

- um confounder importante não foi medido;
- foi medido com erro;
- foi categorizado de forma grosseira;
- um proxy captura apenas parte da causa relevante;
- a relação foi modelada de forma inadequada;
- há causas compartilhadas desconhecidas;
- o ajuste disponível não corresponde ao verdadeiro mecanismo causal.

Portanto:

> “O estudo ajustou para 25 covariáveis” não significa “o confounding acabou”.

O número de covariáveis não é evidência de ajuste correto.

---

# 6. DAGs: representar assumptions causais antes de escolher ajuste

## 6.1 O que é um DAG?

Um **directed acyclic graph (DAG)** é um diagrama em que:

- variáveis são representadas por nós;
- setas representam relações causais assumidas;
- as setas têm direção;
- o grafo não forma um ciclo causal instantâneo que retorna ao próprio ponto de origem.

Exemplo:

```text
Treino ──► Suplemento ──► Desempenho
   └────────────────────►
```

O DAG não “descobre” automaticamente a verdade. Ele torna explícita uma hipótese sobre como os dados foram gerados.

## 6.2 Uma seta é uma assumption, não uma correlação

`A ──► Y` significa:

> Estamos assumindo que A pode causar Y no contexto representado.

Não significa:

> Encontramos correlação estatística entre A e Y.

Da mesma forma, **a ausência de uma seta também é uma assumption**: você está afirmando que não existe aquela relação causal direta relevante no modelo.

## 6.3 Para que DAGs ajudam

DAGs podem ajudar a:

- tornar explícita a pergunta causal;
- organizar temporalidade;
- distinguir causas comuns, mediators e colliders;
- visualizar caminhos não causais;
- justificar o que deve e o que não deve ser ajustado;
- revelar variáveis importantes que nem sequer foram medidas;
- comunicar assumptions para crítica externa.

## 6.4 O que DAGs não fazem

Um DAG não:

- prova que as setas estão corretas;
- garante que todos os confounders foram incluídos;
- mede o tamanho do bias;
- substitui conhecimento biológico/contextual;
- transforma dados ruins em bons;
- cria temporalidade ausente;
- elimina measurement error;
- torna uma análise causal só porque existe um desenho bonito.

Regra de segurança:

> **DAG é um mapa das assumptions. Um mapa pode revelar onde você pretende ir e onde pode se perder; ele não prova que o terreno real é igual ao desenho.**

---

# 7. Confounder, mediator e collider

O mesmo nome de variável pode ter papéis diferentes em perguntas diferentes. O papel depende da estrutura causal e do estimand.

## 7.1 Confounder: causa comum

```text
C ──► A
└───► Y
A ──► Y
```

Se queremos o efeito de A sobre Y, deixar `C` sem controle pode manter aberto um caminho não causal `A ◄ C ► Y`.

Ajustar adequadamente para C pode ajudar a bloquear esse caminho, sob assumptions apropriadas.

## 7.2 Mediator: parte do mecanismo causal

```text
A ──► M ──► Y
└──────────► Y
```

`M` é causado por A e participa do caminho pelo qual A afeta Y.

Exemplo hipotético:

```text
Estratégia de carboidrato ──► disponibilidade de substrato ──► desempenho
```

Se a pergunta é o **efeito total** da estratégia sobre desempenho, ajustar por um mediator pode remover justamente parte do efeito que queremos estimar.

Isso não significa que “nunca se ajusta mediator”. Se a pergunta for sobre efeito direto, mediação pode exigir outro estimand e métodos apropriados. Essa análise formal está além de F0.3.

A regra introdutória é:

> **não ajuste uma variável pós-exposição sem saber se ela faz parte do mecanismo que define o efeito de interesse.**

## 7.3 Collider: efeito comum

Estrutura:

```text
A ──► S ◄── U ──► Y
```

`S` recebe setas de dois lados. Ele é um **collider** naquele caminho.

Sem condicionar em S, o caminho entre A e U através de S está fechado.

Se você:

- seleciona apenas pessoas com `S=1`;
- estratifica por S;
- ajusta estatisticamente por S;

você pode abrir associação entre A e U e, por consequência, distorcer a relação A–Y.

### Exemplo hipotético

Considere:

- `A`: uso de suplemento;
- `U`: potencial genético/talento não medido;
- `S`: entrar em equipe de elite;
- `Y`: desempenho.

Tanto uso de suplemento quanto talento podem aumentar chance de seleção para a equipe:

```text
Suplemento ──► Seleção elite ◄── Talento ──► Desempenho
```

Se você analisa **somente atletas selecionados**, conhecer que alguém usa menos suplemento pode implicitamente selecionar pessoas com maior talento para ainda assim terem chegado ao grupo. Isso pode induzir uma associação entre suplemento e talento que não existia na população original.

O detalhe importante não é decorar “collider bias”. É reconhecer o mecanismo:

> **condicionar em um efeito comum pode criar um caminho de associação que antes estava fechado.**

---

# 8. Ajuste: por que “controlar tudo” pode aumentar bias

## 8.1 Ajuste não é sinônimo de rigor

Um modelo com 40 covariáveis pode ser pior que um modelo com 6 se as 40 incluírem mediators, colliders ou variáveis medidas depois da exposição que alteram o estimand.

A seleção de covariáveis deve partir de:

1. pergunta causal;
2. time ordering;
3. knowledge do domínio;
4. estrutura causal assumida;
5. estimand.

Não deve partir apenas de:

- p-value de associação com outcome;
- diferença de baseline isolada;
- algoritmo automático;
- disponibilidade de colunas no banco;
- regra “ajuste tudo que puder”.

## 8.2 Três erros clássicos

### Erro 1 — deixar causa comum aberta

Se `C` causa A e Y, não considerar C pode deixar confounding.

### Erro 2 — ajustar mediator quando quer efeito total

Se `A → M → Y`, controlar M bloqueia parte do efeito total.

### Erro 3 — ajustar collider

Se `A → S ← U → Y`, controlar S abre um caminho não causal.

## 8.3 “Baseline imbalance” e causal role são coisas diferentes

Em um RCT, uma covariável pode estar numericamente diferente no baseline por acaso. Isso não transforma automaticamente a variável em confounder criado pela randomização.

Em um estudo observacional, uma variável pode ter médias muito parecidas entre grupos e ainda ser causalmente importante.

Portanto, escolher ajuste apenas pela diferença observada em tabela baseline é uma heurística fraca.

---

# 9. Selection: quem entra, fica e aparece na análise

## 9.1 Selection bias não é uma única coisa

Seleção pode ocorrer em vários estágios:

- quem aceita participar;
- quem é elegível;
- quem chega ao estudo;
- quem permanece em follow-up;
- quem possui dado completo;
- quem entra na análise final;
- quem é incluído por uma regra definida depois da exposição/outcome.

O problema causal aparece quando o mecanismo de seleção cria uma amostra/analytical set no qual exposição e causas do outcome ficam artificialmente associadas, ou quando a população observada deixa de representar a população-alvo relevante para a inferência que está sendo feita.

## 9.2 Não representatividade ≠ automaticamente internal bias

Uma amostra muito específica pode ter ótima internal validity para o efeito naquele grupo e pouca generalização para outros grupos.

Exemplo:

- RCT bem conduzido em homens jovens treinados;
- efeito causal internamente válido para as condições estudadas;
- incerteza para mulheres, idosos, iniciantes ou atletas de outra modalidade.

Isso é principalmente um problema de **external validity/applicability**, não necessariamente de internal validity.

## 9.3 Seleção que depende de exposição e outcome/c suas causas

Uma seleção pode comprometer internal validity quando condiciona em um processo que recebe influência de exposição e de determinantes do outcome.

Estrutura genérica:

```text
A ──► S ◄── U ──► Y
```

Analisar apenas `S=1` pode abrir A–U e distorcer A–Y.

## 9.4 “Só complete cases” pode ser seleção

Se a presença do dado final depende de fatores relacionados à exposição e ao verdadeiro outcome, restringir a quem tem dado completo é uma forma de condicionar na seleção.

Por isso, missingness entra na próxima seção como um mecanismo causal possível, não como mera célula vazia de planilha.

---

# 10. Measurement / information bias

## 10.1 Measurement error

**Measurement error** é diferença entre o valor que queremos medir e o valor registrado pelo procedimento de mensuração.

Pode ocorrer em:

- exposição/intervenção;
- adherence;
- confounder;
- mediator;
- outcome;
- covariáveis de seleção.

Erro de mensuração pode ser predominantemente aleatório ou sistemático. F0.3 se concentra no potencial de **distortion sistemática**.

## 10.2 Information bias

**Information bias** é um termo amplo para distorções sistemáticas na coleta, recordação, registro, classificação ou handling da informação.

Exemplos:

- participantes recordam ingestão de forma diferente conforme sabem seu status de outcome;
- avaliador interpreta um teste subjetivo de forma diferente ao conhecer o grupo;
- um grupo é monitorado com dispositivo mais sensível que outro;
- exposição habitual é classificada por um único questionário pouco adequado ao horizonte de interesse.

## 10.3 Misclassification

**Misclassification** ocorre quando pessoas/observações são colocadas em categoria diferente da verdadeira categoria relevante.

Exemplo:

- classificar atleta como “alta ingestão proteica” versus “baixa” com medida que erra sistematicamente em certo subgrupo.

### Differential misclassification

A chance/direção do erro difere entre grupos relevantes.

### Non-differential misclassification

O erro não depende da comparação principal segundo uma definição específica.

Cuidado com uma regra popular incorreta:

> “Non-differential misclassification sempre puxa para o null.”

Não é uma lei universal. Direção/magnitude dependem da estrutura da variável, categorias, sensibilidade/especificidade e do efeito verdadeiro.

## 10.4 Medir confounder mal pode deixar residual confounding

Você pode “ajustar para treino semanal”, mas se mediu treino com uma pergunta grosseira que não captura volume/intensidade relevantes, parte do confounding pode permanecer.

Assim, mensuração ruim não afeta só o outcome; ela também pode tornar um ajuste causal incompleto.

## 10.5 O que pode prevenir/mitigar

Dependendo do contexto:

- protocolo padronizado;
- instrumentos validados para o construct relevante;
- blinding quando viável e pertinente;
- mesma intensidade de mensuração entre grupos;
- treinamento/calibração de avaliadores;
- repetição de medidas;
- medidas objetivas quando realmente representam melhor o construct;
- validation subsamples;
- sensitivity analyses apropriadas.

Mas análise estatística não consegue reconstruir automaticamente um valor nunca medido de forma informativa.

---

# 11. Attrition e missingness como mecanismos de bias

## 11.1 Missing data não é automaticamente bias

Ter 5%, 20% ou 40% de dados faltantes não determina sozinho o bias.

A pergunta é:

> **por que os dados estão faltando e como esse mecanismo se relaciona com exposição/intervenção, outcome e seus determinantes?**

## 11.2 Attrition

**Attrition** é perda de participantes ao longo do estudo/follow-up.

Exemplo:

- suplemento causa desconforto gastrointestinal;
- participantes com desconforto abandonam o estudo;
- desconforto também reduz treinamento e performance;
- os que permanecem no grupo suplemento são uma seleção mais tolerante.

Se a análise usa apenas completers, o grupo final pode não representar mais o contraste criado no início.

## 11.3 Mesmo percentual de perda pode esconder mecanismos diferentes

Dois braços podem perder 10% cada e ainda assim haver bias se:

- em A, saem os piores respondedores;
- em B, saem pessoas aleatórias por mudança de cidade.

Percentual igual não significa mecanismo igual.

Da mesma forma, perda desigual não prova automaticamente bias grave se o mecanismo e a informação disponível permitirem inferência adequada sob assumptions justificáveis.

## 11.4 Complete-case analysis não é neutro por padrão

Excluir toda pessoa sem outcome final cria uma nova condição de entrada na análise: “ter dado completo”.

Se ter dado completo depende de causas da exposição/outcome, essa seleção pode distorcer a comparação.

## 11.5 O que análise pode e não pode reparar

Métodos como imputation, weighting e sensitivity analysis podem ajudar em situações apropriadas, **mas dependem de assumptions e informação observada**.

Se o fator que determina missingness e o verdadeiro outcome não foi medido, nenhum método consegue garantir recuperação da verdade sem assumptions externas.

A ideia que você deve carregar para frente é:

> **missingness é um processo causal a ser entendido, não uma porcentagem a ser tolerada por convenção.**

A modelagem formal de missing data fica para módulos posteriores/aprofundamento.

---

# 12. Reverse causation

## 12.1 Definição

**Reverse causation** ocorre quando interpretamos `A → Y`, mas o processo verdadeiro pode ser `Y → A` total ou parcialmente.

Exemplo transversal:

> atletas com menor ingestão energética relatam mais fadiga.

Interpretação apressada:

> baixa ingestão causou fadiga.

Alternativa:

> fadiga/doença/overreaching reduziu apetite e ingestão.

Estruturas possíveis:

```text
Ingestão ──► Fadiga
```

ou

```text
Fadiga ──► Ingestão
```

ou ambas em feedback ao longo do tempo.

## 12.2 Por que F0.2 era pré-requisito

Cross-sectional designs frequentemente medem exposição e outcome na mesma janela, tornando temporal ordering ambígua.

Cohort pode melhorar a ordenação temporal, mas “A medido antes de Y” ainda não elimina confounding ou processos subclínicos já em curso que influenciaram A.

Temporalidade é necessária para muitos claims causais, mas não suficiente.

---

# 13. Randomization: o que reduz e o que não elimina

## 13.1 O ganho causal da randomização

Quando corretamente implementada, random assignment quebra, em expectativa, a ligação sistemática entre características pré-intervenção e a condição atribuída.

Isso ajuda a controlar **confounding baseline medido e não medido** sem precisar identificar cada causa comum individualmente.

## 13.2 O que randomização não corrige

Depois da alocação ainda podem surgir:

- nonadherence;
- crossover entre intervenções;
- differential co-interventions;
- loss to follow-up;
- missing outcomes;
- outcome measurement influenciado por conhecimento de grupo;
- problemas de implementação;
- selective analysis/reporting;
- estimand mal definido;
- outcome inadequado;
- análise incompatível com cluster/crossover;
- interpretação além da população e contexto estudados.

Portanto:

> **randomização protege principalmente a origem do contraste; ela não congela todo o restante do estudo em estado livre de bias.**

## 13.3 Pós-randomização pode destruir a comparabilidade inicial

Se você randomiza corretamente e depois analisa apenas um subconjunto definido por uma variável pós-randomização, pode reintroduzir seleção/collider bias.

Exemplo:

> analisar apenas “aderentes perfeitos” se adesão é influenciada pela intervenção e por fatores prognósticos.

O fato de o estudo começar randomizado não torna qualquer análise de subgrupo causal.

## 13.4 Ferramentas formais ficam para F0.8

RoB 2 e ROBINS-I/ROBINS-I V2 organizam domínios de bias de forma estruturada. Nesta unidade, eles são usados apenas como evidência de que problemas como confounding, selection, missing data e outcome measurement são **mecanismos distintos**.

Não memorize domínios nem transforme ferramentas em score. A aplicação formal virá em F0.8.

---

# 14. Target-trial thinking como benchmark de desenho causal

F0.2 apresentou o target trial. Agora usamos o conceito como detector de bias arquitetural.

## 14.1 Pergunta central

Se você quer interpretar dados observacionais como resposta causal sobre estratégias/intervenções, pergunte:

> **qual seria o protocolo do ensaio randomizado hipotético que responderia exatamente esta pergunta?**

Elementos mínimos:

- eligibility;
- estratégias comparadas;
- momento zero;
- regra de assignment hipotética;
- follow-up;
- outcome;
- causal contrast/estimand;
- analysis plan em nível conceitual.

## 14.2 Emulation

Depois pergunte:

- os dados observacionais conseguem reproduzir eligibility?
- exposição foi definida no mesmo momento em que follow-up começa?
- outcome ocorre depois da estratégia?
- há variáveis para controlar confounding relevante?
- adherence/switching estão observáveis se importam para o estimand?
- pessoas elegíveis não foram selecionadas com informação do futuro?

A lógica é:

`especificar target trial → avaliar se os dados conseguem emular → declarar divergências e assumptions`

## 14.3 O framework não cria dados ausentes

Target-trial thinking pode prevenir biases criados por desenho ruim, como desalinhamento entre início de follow-up e definição de exposição.

Mas não pode:

- randomizar retrospectivamente;
- medir confounder inexistente;
- corrigir exposure misclassification sem informação;
- recuperar outcomes nunca observados sem assumptions;
- provar exchangeability.

Ele é um **benchmark de desenho**, não uma máquina de causalidade.

---

# 15. Internal validity versus external validity/applicability

## 15.1 Internal validity

Pergunta:

> **A estimativa representa adequadamente o efeito/quantidade-alvo para a população e condições efetivamente estudadas?**

Ameaças incluem:

- confounding;
- selection que distorce o contraste interno;
- measurement/information bias;
- missingness/attrition;
- análise que condiciona variáveis inadequadas;
- violations importantes do desenho.

## 15.2 External validity / generalizability

Pergunta:

> **O efeito estimado pode ser generalizado para uma população-alvo mais ampla da qual a amostra pretende representar um subconjunto?**

Exemplo:

- homens jovens treinados em laboratório;
- target: atletas adultos de ambos os sexos e vários níveis competitivos.

A diferença de população pode limitar generalização mesmo com ótimo RCT.

## 15.3 Transportability

**Transportability** enfatiza mover uma inferência para uma população/contexto que não é simplesmente a população de origem da amostra.

Exemplo:

- estudo em corredores recreacionais em clima temperado;
- decisão para ultramaratonistas em calor extremo.

Isso pode exigir knowledge adicional sobre effect modification e contexto.

## 15.4 Applicability

**Applicability** é a pergunta prática: quão diretamente a evidência corresponde à população, intervenção/exposição, comparador, outcome, tempo e contexto da decisão?

F0.8 tratará isso junto de certainty/indirectness. Aqui basta separar:

> **um estudo pode ser internamente forte e externamente estreito.**

E também:

> **uma amostra “representativa” não salva uma estimativa internamente biased.**

---

# 16. O que pode ser reparado — e o que não pode ser recuperado dos dados

Um bom crítico não diz apenas “há bias”. Ele pergunta **onde intervir**.

| Problema | Melhor prevenção/mitigação típica | Limite fundamental |
|---|---|---|
| confounder conhecido antes da exposição | randomização; restriction/matching/design; medir bem; ajuste causal apropriado | confounder não medido pode permanecer |
| confounder medido grosseiramente | melhorar instrumento/repetição/validation | análise não recria informação que nunca foi capturada adequadamente |
| mediator ajustado quando alvo é efeito total | definir estimand antes; não condicionar no caminho causal total | se só existe análise condicionada, o efeito total pode não ser recuperável sem dados/modelo adequado |
| collider criado por seleção/ajuste | redesenhar critérios; evitar condicionamento; modelar seleção sob assumptions | se mecanismo/variáveis de seleção não foram observados, correção pode ser impossível ou altamente assumption-dependent |
| differential outcome measurement | blinding quando viável; standardization; objective/validated measurement | não há correção garantida sem informação sobre o processo de erro |
| exposure misclassification | measurement melhor; repeated measures; validation subsample | classificação verdadeira ausente limita correção |
| attrition/missing outcome | retenção; documentar razões; coletar outcome mesmo após interrupção quando possível; métodos apropriados/sensitivity | outcomes ausentes dependentes de fatores não medidos podem deixar incerteza irredutível |
| reverse causation | desenho longitudinal/experimental; definir time zero; medir estado prévio | corte transversal não cria passado ausente |
| baixa external validity | amostragem/replicação em targets relevantes; transport analyses quando justificadas | não há guarantee de transporte para contextos não estudados |

Regra:

> **statistical sophistication não substitui informação causal que o desenho nunca coletou.**

---

# 17. Worked example — suplemento, treinamento e performance

Considere um estudo observacional hipotético.

## 17.1 Claim bruto

> “Atletas que usam suplemento X têm 6% melhor desempenho; portanto X melhora performance.”

Antes de discutir números, reconstrua a pergunta:

> Entre atletas adultos treinados elegíveis no baseline, iniciar/usar protocolo definido de X, comparado a não usar X, causa melhora de performance em teste padronizado após 12 semanas?

## 17.2 Estrutura causal inicial

Considere:

- `A`: uso de X;
- `Y`: performance em 12 semanas;
- `T`: carga/qualidade de treinamento prévia;
- `M`: variável fisiológica causada por X que faz parte do mecanismo;
- `S`: permanecer no estudo até 12 semanas;
- `U`: motivação/tolerância não medida.

DAG simplificado:

```text
T ──► A ──► M ──► Y
│     │           ▲
└─────┼───────────┘
      │
      └──► S ◄── U ──► Y
```

Interpretação:

- `T` é confounder se causa uso de X e performance;
- `M` é mediator para o efeito total de X;
- `S` pode funcionar como collider se permanecer no estudo depende de X e de U;
- `U` é causa não medida do outcome e da seleção.

## 17.3 Estratégias de ajuste

### Ajustar T

Pode ser apropriado para bloquear `A ◄ T ► Y`, se T for medido adequadamente e o DAG estiver plausível.

### Ajustar M

Se o alvo é **efeito total**, ajustar M bloqueia parte do mecanismo A→M→Y e muda o estimand.

### Analisar apenas S=1

Se S recebe influência de A e U, condicionar em S pode abrir associação A↔U→Y.

### “Ajustar por tudo”

Misturar T, M e S no mesmo modelo não é automaticamente mais rigoroso. Pode simultaneamente reduzir um bias e introduzir outro.

## 17.4 Missingness

Se usuários de X com sintomas GI abandonam mais e sintomas também reduzem performance, os completers do braço/exposição X podem parecer melhores do que o grupo original.

Pergunta correta:

> quem ficou sem outcome e por quê?

## 17.5 Measurement

Se uso de X e training load são auto-relatados com erro, o ajuste para T pode deixar residual confounding e A pode ser misclassified.

## 17.6 Conclusão proporcional

Uma conclusão defensável poderia ser:

> “Foi observada associação entre uso de X e melhor performance, mas a interpretação causal depende de assumptions fortes sobre confounding pré-exposição, selection/missingness e measurement. O estudo não estabelece, por si só, que iniciar X causaria o mesmo ganho.”

Isso é mais informativo do que simplesmente escrever “correlation ≠ causation”, porque identifica **por quais caminhos** a associação pode não ser causal.

---

# 18. Worked contrast — randomized trial também pode ser biased

Agora imagine um RCT:

- 200 atletas randomizados para X ou placebo;
- boa allocation concealment;
- 12 semanas;
- 25% do grupo X abandona por sintomas;
- 8% do placebo abandona;
- outcome subjetivo é avaliado por pessoas que conhecem o grupo;
- análise final inclui apenas completers.

## 18.1 O que randomização resolveu

No início, ela protegeu contra confounding sistemático baseline da **assignment**.

## 18.2 O que ficou vulnerável

- differential attrition;
- selection pela análise de completers;
- outcome measurement influenciado por conhecimento de grupo;
- possível alteração do contraste causal se adherence/dropout é tratado inadequadamente.

Logo:

> “Randomized” descreve uma característica crucial do desenho, não uma garantia de unbiased result.

F0.8 formalizará como avaliar isso por domínio e resultado.

---

# 19. Um algoritmo de raciocínio causal para F0.3

Ao ler um claim causal, percorra esta sequência.

## Passo 1 — escreva a pergunta causal

Defina:

`population + strategy/exposure A + comparator B + outcome + time + causal estimand`

Se a pergunta não está clara, o ajuste também não pode estar.

## Passo 2 — desenhe a ordem temporal mínima

O que existe antes de A?
O que é causado por A?
O que acontece depois?
O que define entrada/permanência na análise?

## Passo 3 — faça um DAG simples

Inclua mesmo variáveis não medidas se causalmente relevantes. Não desenhe apenas colunas disponíveis no dataset.

## Passo 4 — classifique papéis

Para a pergunta atual:

- common cause → possível confounder;
- no caminho A→Y → possível mediator;
- common effect → possível collider;
- selection node → possível caminho de selection bias;
- measured proxy → pergunte quão bem representa a causa relevante.

## Passo 5 — pergunte o que a randomização fez

Se não randomizado: quais assumptions de exchangeability são necessárias?

Se randomizado: o contraste pós-randomização foi preservado?

## Passo 6 — audite measurement

- A foi medido/classificado corretamente?
- Y foi medido igualmente entre grupos?
- confounders foram medidos com qualidade suficiente?
- existe differential recall/observer/detection process?

## Passo 7 — audite missingness/selection

- quem entrou?
- quem saiu?
- quem tem outcome?
- por que?
- selecionar completers abre caminho causal indesejado?

## Passo 8 — teste reverse causation

É possível Y ou um processo pré-clínico relacionado a Y ter influenciado A?

## Passo 9 — se a pergunta é intervention-like, especifique o target trial

Compare o estudo real com o ensaio-alvo e liste divergências.

## Passo 10 — separe validity interna de applicability

Primeiro: “a estimativa é válida no estudo?”
Depois: “para quem/contexto ela pode ser transportada?”

## Passo 11 — classifique repairability

Para cada ameaça, diga:

- prevenir no design;
- melhorar measurement;
- mitigar em analysis sob assumptions;
- ou **não recuperável dos dados disponíveis**.

## Passo 12 — escreva conclusão calibrada

Use linguagem proporcional:

- “associação compatível com...”;
- “efeito causal é plausível se...”;
- “randomization supports causal interpretation of assignment, but...”;
- “não é possível distinguir X de Y com os dados disponíveis”.

Evite:

- “prova”;
- “ajustado = causal”;
- “RCT = sem bias”;
- “DAG mostrou que...” quando o DAG apenas codificou assumptions.

---

# 20. Micro-checks de recuperação ativa

Tente responder sem consultar acima.

1. Por que aumentar sample size não elimina systematic bias?
2. Defina confounding por estrutura causal, não por correlação.
3. O que residual confounding pode significar após ajuste?
4. Qual a diferença entre mediator e confounder para efeito total?
5. Por que conditioning em collider pode criar associação?
6. Um DAG prova que as relações causais desenhadas são verdadeiras?
7. Por que “ajuste todas as covariáveis disponíveis” é estratégia perigosa?
8. Como complete-case analysis pode funcionar como seleção?
9. Por que percentual de missing data isolado não mede bias?
10. Dê um exemplo de reverse causation em nutrição/performance.
11. O que randomização resolve na origem do contraste?
12. Cite três ameaças pós-randomização que podem permanecer.
13. Para que serve o target-trial framework?
14. Por que target-trial emulation não cria randomização?
15. Diferencie internal validity de external validity/applicability.
16. Qual problema existe em ajustar um mediator se você quer o efeito total?
17. Dê um exemplo de problema que análise não consegue reparar porque a informação nunca foi coletada.
18. Por que não representatividade e internal bias não são a mesma coisa?

Se você só consegue repetir definições, ainda não atingiu a competência. A próxima etapa é `EXERCISES.md`, que exige identificar estruturas causais, escolher ajuste, explicar mecanismos de distortion e delimitar conclusões.

---

# 21. Limites deliberados desta unidade

F0.3 **não** ensina formalmente:

- algorithms completos de RoB 2;
- ROBINS-I/ROBINS-I V2 item a item;
- ROBINS-E;
- GRADE certainty ratings;
- quantitative bias analysis;
- inverse-probability weighting em matemática;
- multiple imputation em matemática;
- g-methods/time-varying confounding;
- mediation analysis formal;
- instrumental variables;
- propensity scores em detalhe;
- confidence intervals/p-values/power;
- meta-analysis.

Esses assuntos exigem pré-requisitos adicionais ou pertencem a F0.4–F0.8/aprofundamentos.

O objetivo aqui é mais fundamental:

> **conseguir olhar para a arquitetura causal de um estudo e explicar por qual mecanismo a estimativa pode se afastar do efeito que a pergunta pretendia identificar.**

---

# 22. Fontes e função instrucional

As referências completas estão em `../SOURCE_INDEX.md`.

- `F0-S16` — foundation para counterfactuals, exchangeability, confounding, selection e causal identification.
- `F0-S17` — target-trial framework e limite explícito de emulation com dados inadequados.
- `F0-S26` — guia clínico atual de DAGs, causal roles, confounder/mediator/collider e escolha de adjustment sets.
- `F0-S11` — exemplos concretos de confounding, collider bias, selection, attrition, information bias e misclassification; usado como catálogo de mecanismos, não como checklist de nomes.
- `F0-S07` — confirma separação operacional entre diferentes bias domains e a existência de ferramentas específicas para randomized/non-randomized evidence; aplicação formal é deliberadamente adiada para F0.8.
- `F0-S14` — mantém alinhamento entre objective/estimand/design e lembra que análises/sensitivity assumptions precisam responder ao efeito definido.

Nenhuma fonte de nutrição esportiva é tratada como autoridade metodológica nesta unidade. Os exemplos são hipotéticos para transferência pedagógica.