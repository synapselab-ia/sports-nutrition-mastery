# F0.6 — Power, Type I/II error, multiplicidade e flexibilidade analítica

**Production state:** `APPROVED_PENDING_QA`

**Prerequisites P2:** F0.4 — estatística descritiva, distribuições e variação amostral; F0.5 — estimativas, intervalos de confiança, p-values, effect sizes e relevância prática.

**P0 ensinados localmente:** hipótese nula, regra de decisão, Type I error, Type II error, alpha, beta, power, family of hypotheses, multiplicity, family-wise error, primary/secondary/exploratory analysis, preregistration, trial registration, protocol, statistical analysis plan (SAP), analytical flexibility.

**P1 ensinados localmente:** complemento de probabilidade; leitura conceitual de uma power curve; cálculo ilustrativo de pelo menos um falso positivo entre testes independentes.

**Core/method sources:** `F0-S01`, `F0-S08`, `F0-S09`, `F0-S10`, `F0-S13`, `F0-S28`, `F0-S29`.

## 1. Competência-alvo

Ao terminar esta unidade, você deve conseguir olhar para o planejamento e para o relatório de um estudo e responder:

1. **qual regra de decisão estatística foi planejada?**
2. **qual erro Type I essa regra controla e em que sentido?**
3. **qual erro Type II/power foi calculado para qual efeito específico?**
4. **o tamanho amostral foi justificado pelo objetivo inferencial ou apenas por convenção?**
5. **a precisão observada responde melhor à pergunta pós-estudo do que um “observed power”?**
6. **qual é a família de hipóteses/claims confirmatórios que está sendo protegida?**
7. **quantos outcomes, time points, subgrupos, modelos ou escolhas analíticas poderiam gerar resultados selecionáveis?**
8. **como a multiplicidade altera o risco de pelo menos uma conclusão falsa?**
9. **o que foi prespecificado e o que foi decidido depois de ver os dados?**
10. **o resultado é confirmatório ou exploratório?**
11. **o que registro, protocolo e SAP tornam auditável — e o que eles não garantem?**
12. **qual conclusão permanece suportada depois de integrar magnitude/CI de F0.5 com a arquitetura analítica do estudo?**

Regra central:

> **power é propriedade de um procedimento antes dos dados, condicionada a efeito e assumptions; precisão é informação do resultado observado; multiplicidade e flexibilidade analítica mudam o comportamento do processo de inferência; prespecificação aumenta transparência, mas não transforma um desenho ruim em evidência boa.**

---

# 2. O ponto de partida: uma regra de decisão repetida

F0.5 ensinou que um p-value não é a probabilidade de H0 ser verdadeira e que resultados não devem ser reduzidos a `significant / nonsignificant`.

F0.6 pergunta outra coisa:

> se repetirmos um procedimento estatístico sob condições definidas, com que frequência ele toma decisões corretas ou erradas?

Para construir a intuição, use a regra simples:

- se `p < alpha`, rejeitar H0;
- se `p >= alpha`, **não rejeitar** H0.

Importante:

`não rejeitar H0` não significa `aceitar H0 como verdadeira`.

Essa regra binária é uma ferramenta pedagógica para entender error rates. A interpretação científica final continua exigindo estimativa, CI, magnitude, practical threshold, desenho e bias.

---

# 3. Type I error e alpha

## 3.1 Type I error

Um **Type I error** ocorre quando a regra rejeita H0 em uma repetição na qual o modelo nulo relevante é verdadeiro.

Em linguagem curta:

`H0 verdadeira → regra rejeita H0`.

## 3.2 Alpha

`alpha` é o erro Type I nominal da regra sob as condições/modelo usados.

Em um teste simples com `alpha = 0.05`:

> se o modelo nulo for verdadeiro e o procedimento for repetido muitas vezes de acordo com suas assumptions, aproximadamente 5% das repetições cairão na região de rejeição.

### Alpha NÃO é

- 5% de probabilidade de H0 ser verdadeira depois de um resultado positivo;
- 5% de probabilidade de este artigo específico ser falso;
- “chance de o resultado ter acontecido por acaso”;
- uma taxa garantida de falsos papers na literatura.

Alpha descreve o comportamento de uma **regra/procedimento** sob uma condição especificada.

---

# 4. Type II error, beta e efeito específico

## 4.1 Type II error

Um **Type II error** ocorre quando a regra não rejeita H0 mesmo existindo um efeito/estado alternativo relevante definido para o cálculo.

Forma simplificada:

`efeito verdadeiro especificado ≠ null → regra não rejeita H0`.

## 4.2 Beta depende da alternativa

Dizer apenas:

> “beta = 0.20”

é incompleto.

Pergunte:

- para qual diferença verdadeira?
- qual SD/variabilidade?
- qual n?
- qual alpha?
- teste unilateral ou bilateral?
- qual desenho e alocação?
- qual perda amostral esperada?
- quais assumptions?

Em geral, `beta` muda quando o efeito verdadeiro considerado muda.

Portanto, uma study design não possui um único beta universal para toda possível alternativa.

---

# 5. Statistical power

Power é:

`power = 1 − beta`

Mas a definição importante é:

> **power é a probabilidade, antes de observar os dados, de um procedimento rejeitar H0 quando um efeito verdadeiro específico e as demais assumptions do cálculo são as adotadas.**

Exemplo:

> “Com n=80, alpha=0.05 bilateral, SD assumido X e diferença verdadeira de +2 unidades, o teste tem power de 80%.”

Isso significa, conceitualmente:

- sob esse efeito e essas assumptions;
- em muitas repetições do desenho;
- cerca de 80% produziriam rejeição de H0 pela regra especificada.

## 5.1 Power não é probabilidade da hipótese

`80% power` NÃO significa:

- 80% de probabilidade de H1 ser verdadeira;
- 80% de chance de o estudo “dar certo” em qualquer sentido;
- 80% de chance de o efeito observado ser real;
- 20% de chance de um resultado não significativo específico ser “falso negativo”.

Power é uma probabilidade **condicionada a um estado de mundo/effect size assumido**, não uma probabilidade posterior sobre o mundo depois de ver os dados.

---

# 6. A power curve: não existe “o power” sem efeito

Imagine testar diferenças verdadeiras de magnitudes diferentes.

Com o mesmo n e alpha:

- efeito muito pequeno → power menor;
- efeito intermediário → power maior;
- efeito grande → power ainda maior.

Uma **power curve** mostra:

`efeito verdadeiro assumido → probabilidade de rejeitar H0`.

P1 essencial:

> **power é uma função do efeito e do desenho, não um selo único da amostra.**

Quando alguém diz “o estudo teve 80% de power”, a pergunta correta é:

> “80% para detectar qual efeito, sob quais assumptions?”

---

# 7. O que tende a alterar power

Mantendo outros componentes comparáveis:

## Maior tamanho amostral

Tende a aumentar power porque reduz sampling uncertainty/SE.

## Maior efeito verdadeiro considerado

Tende a aumentar power porque o sinal se separa mais do null.

## Menor variabilidade

Tende a aumentar power porque melhora signal-to-noise.

## Alpha mais estrito

Exemplo: `0.01` em vez de `0.05`.

Tende a reduzir power para o mesmo n/effect, porque a região de rejeição fica mais difícil de alcançar.

## Desenho mais eficiente

Pareamento, medidas repetidas ou covariates prognósticas podem melhorar eficiência em contextos apropriados, mas dependem de modelagem correta. Não generalize sem respeitar estrutura do desenho.

---

# 8. Power versus precision

Essa distinção é central.

## Power

Pergunta pré-estudo:

> “Sob um efeito verdadeiro especificado, com este desenho e regra de decisão, qual a probabilidade de rejeitar H0?”

Objeto:

- design;
- assumptions;
- target effect;
- decisão repetida.

## Precision

Pergunta pós-estudo:

> “Quão estreita é a incerteza em torno da estimativa que observamos?”

Objetos:

- SE;
- CI;
- escala do effect estimate.

F0.5 já mostrou que dois resultados `p>0.05` podem ser muito diferentes:

- um CI enorme → pouca informação;
- um CI estreito dentro da zona trivial → informação forte contra efeitos considerados importantes.

Portanto:

> **depois de observar o estudo, estimate + CI + practical threshold são normalmente mais úteis para interpretar informativeness do que calcular observed power a partir do próprio efeito observado.**

---

# 9. Por que post hoc / observed power é geralmente não informativo

Um uso problemático comum é:

1. executar o estudo;
2. observar `p>0.05`;
3. inserir o effect size observado na fórmula de power;
4. obter “power observado baixo”;
5. concluir que “o estudo não encontrou efeito porque teve pouco power”.

Isso não resolve o problema.

Heinsberg & Weeks (2022) mostram por simulação e argumentação que **observed/post hoc power calculado a partir do efeito observado é redundante/misleading** e não ajuda a distinguir:

- efeito realmente ausente/trivial;
- efeito relevante com amostra imprecisa;
- diferença entre effect size verdadeiro e observado;
- outras limitações do estudo.

Em configurações comuns, observed power fica fortemente ligado ao próprio p-value e estimate usados para calculá-lo.

### Regra F0.6

Depois do estudo, não faça:

`p alto → observed power baixo → “faltou power”`.

Faça:

`estimativa → CI → threshold prático → design/bias → o que permanece compatível`.

### Distinção importante

Uma análise de planejamento/sensibilidade que pergunta:

> “Com este n e desenho, qual seria o power para uma diferença externamente especificada de +2?”

é conceitualmente diferente de calcular power usando o **efeito observado** para explicar o próprio resultado.

Mesmo assim, ela descreve o design sob uma hipótese específica; não transforma o resultado observado em probabilidade posterior de efeito.

---

# 10. Sample-size justification: n precisa responder a uma meta

Lakens (2022) organiza várias formas defensáveis de justificar tamanho amostral, incluindo:

- medir quase toda a população quando isso faz sentido;
- restrições de recursos explicitadas;
- a-priori power analysis;
- precisão/accuracy desejada;
- heurísticas justificadas com cautela;
- reconhecer honestamente ausência de justificativa.

A pergunta principal é:

> **o n escolhido consegue produzir informação útil para o objetivo inferencial?**

## 10.1 Para a-priori power

Especifique pelo menos:

- teste/modelo principal;
- alpha;
- power alvo;
- effect size de planejamento;
- origem/justificativa desse effect size;
- variabilidade/baseline assumptions;
- desenho/alocação;
- perdas esperadas quando pertinentes.

## 10.2 Effect size de planejamento

Evite escolher apenas:

> “o effect size publicado no estudo anterior porque foi significativo”.

Pode ser mais defensável usar:

- smallest effect of interest;
- efeito clinicamente/esportivamente relevante;
- faixa plausível baseada em literatura robusta;
- precisão necessária para decisão.

F0.5 já ensinou que um effect size só faz sentido em escala/contexto.

---

# 11. Power e smallest effect of interest

Suponha que diferenças menores que `+2 unidades` sejam consideradas pouco relevantes para a decisão.

Uma pergunta útil de planejamento é:

> “Qual n fornece power adequado para detectar +2 unidades sob variabilidade plausível?”

Ou, se a meta for estimação:

> “Qual n tende a produzir um CI estreito o suficiente para distinguir efeitos acima e abaixo de +2?”

Essas são metas diferentes:

- uma baseada em decisão de teste/power;
- outra baseada em precisão.

Não existe obrigação de justificar toda amostra por power analysis. A justificativa precisa corresponder ao objetivo inferencial.

---

# 12. Type II error não salva um resultado não significativo

Considere um estudo concluído:

`MD = +1.1`

`95% CI = −1.5 a +3.7`

`p = 0.40`

Threshold de benefício relevante = `+2.0`.

É errado dizer:

> “como o study power era 60%, esse resultado provavelmente foi um false negative.”

Por quê?

- 60% power era uma propriedade planejada para **algum efeito assumido**;
- não fornece `P(false negative | dados)`;
- o resultado observado continua compatível com diferentes magnitudes;
- o CI já mostra diretamente a imprecisão relevante para o estimate observado.

A conclusão correta é calibrada ao CI e ao desenho, não convertida em probabilidade posterior via power.

---

# 13. Multiplicity: uma regra repetida muitas vezes

Suponha um único teste com alpha=0.05 sob H0 verdadeira.

Risco nominal de rejeição falsa naquele teste:

`5%`.

Agora execute muitos testes e procure **qualquer** `p<0.05`.

Mesmo que cada teste mantenha alpha=0.05, a chance de pelo menos uma rejeição falsa pode aumentar.

Esse é o núcleo da **multiplicity**.

---

# 14. P1 — complemento de probabilidade e FWER ilustrativa

Se houver `m` testes:

- independentes;
- todos com H0 verdadeira;
- cada um com alpha `0.05`;

então:

`P(nenhum falso positivo) = 0.95^m`

Logo:

`P(pelo menos um falso positivo) = 1 − 0.95^m`.

### Exemplos

| Número de testes independentes | Chance ilustrativa de ≥1 falso positivo |
|---:|---:|
| 1 | 5.0% |
| 3 | 14.3% |
| 5 | 22.6% |
| 10 | 40.1% |
| 20 | 64.2% |

### Cuidado crítico

Na prática, outcomes/time points frequentemente são correlacionados.

Então `1 − (1−alpha)^m` **não é fórmula universal** para qualquer paper. Aqui ela serve para mostrar por que repetição de oportunidades de teste pode inflar o risco conjunto.

---

# 15. Family-wise error rate (FWER)

Uma **family of hypotheses** é um conjunto de hipóteses/claims que precisam ser considerados conjuntamente para controlar o erro relevante à decisão científica.

A **family-wise error rate** é, em termos conceituais, a probabilidade de ocorrer pelo menos uma rejeição Type I dentro da família sob a configuração de nulls relevante ao procedimento.

Para F0.6, a pergunta prática é:

> “Quais testes alimentam o mesmo conjunto de claims confirmatórios e, portanto, não devem ser fingidos como oportunidades completamente isoladas?”

## Família não é sinônimo de “todos os p-values do paper”

A família depende de:

- pergunta;
- claims pretendidos;
- desenho;
- estratégia confirmatória;
- endpoint hierarchy;
- decisão/regra de inferência.

Mas também é incorreto fragmentar artificialmente um programa de testes só para evitar reconhecer multiplicidade.

---

# 16. De onde nasce multiplicidade

## 16.1 Muitos endpoints

Exemplo:

- desempenho;
- massa corporal;
- força;
- soreness;
- biomarcadores;
- sleep;
- mood;
- vários outros.

Se cada outcome puder gerar o headline principal, existem múltiplas oportunidades para uma conclusão favorável.

## 16.2 Muitos time points

Um outcome em:

- week 2;
- week 4;
- week 8;
- week 12.

Escolher depois o time point com menor p é diferente de testar um primary time point prespecificado.

## 16.3 Muitos subgrupos

Exemplos:

- homens/mulheres;
- treinados/menos treinados;
- responders/non-responders definidos post hoc;
- tercis de baseline;
- várias faixas etárias.

Quanto mais splits são explorados, mais padrões aparentes podem surgir por sampling variation.

## 16.4 Muitos modelos

Exemplos:

- unadjusted;
- adjusted por age;
- adjusted por baseline;
- adjusted por baseline + sex;
- com/sem outlier;
- transformação log ou escala original.

Testar muitos caminhos e reportar apenas o mais favorável cria **analytical-path multiplicity**, mesmo quando o scientific hypothesis nominal parece “a mesma”.

## 16.5 Muitas stopping/analysis choices

Exemplos:

- olhar dados repetidamente e parar quando p<0.05;
- alterar n após ver tendência sem procedimento válido;
- adicionar/remover participantes segundo resultado intermediário;
- redefinir analysis population após outcome inspection.

Essas escolhas podem alterar error rates se não forem incorporadas ao desenho/procedimento.

---

# 17. Multiplicity não significa “múltiplos testes são proibidos”

A resposta correta não é:

> “só pode testar uma coisa por estudo”.

É possível estudar múltiplos endpoints/claims com planejamento adequado.

Estratégias conceituais incluem:

1. **um primary endpoint/contrast claramente definido**;
2. **endpoint hierarchy / gatekeeping**;
3. **divisão/controle de alpha entre claims**;
4. **p-values/intervalos ajustados para multiplicidade**;
5. **classificar analyses adicionais como exploratory**;
6. **reportar a família inteira em vez de só os resultados favoráveis**.

F0.6 não exige dominar todos os algoritmos de ajuste.

O objetivo é reconhecer o problema e entender o tipo de solução.

---

# 18. Endpoint hierarchy

Uma **hierarchy** organiza claims em ordem prespecificada.

Exemplo conceitual:

1. primary endpoint A;
2. se A satisfizer o critério planejado, testar key secondary B;
3. depois C.

A lógica pode preservar error control melhor do que testar tudo como se cada hipótese tivesse um alpha independente disponível.

### Limites

Uma hierarchy não:

- torna outcome ruim em outcome bom;
- corrige measurement bias;
- garante causal validity;
- garante que o efeito é importante;
- substitui transparência sobre todos os resultados.

---

# 19. Bonferroni como intuição, não como catálogo

Um exemplo simples de controle é dividir alpha:

Se família tem 5 testes e alpha familiar alvo = 0.05:

`0.05 / 5 = 0.01` por teste.

Essa é a ideia de **Bonferroni**.

Vantagem didática:

- simples;
- deixa claro que o “orçamento de erro” não pode ser reutilizado infinitamente.

Limites:

- pode ser conservador;
- não é sempre a melhor estratégia;
- há métodos hierárquicos/stepwise e procedures específicos ao desenho.

F0.6 precisa entender o princípio, não memorizar uma lista de corrections.

---

# 20. Secondary e subgroup analyses

## Secondary outcomes

Podem ser importantes e planejados.

Mas “secondary” não significa automaticamente:

- sem multiplicity issue;
- confirmatory;
- livre para usar p<0.05 isolado como claim definitivo.

Pergunte:

- foram prespecified?
- qual family/hierarchy?
- qual adjustment?
- foram todos reportados?

## Subgroup analyses

Um erro frequente é concluir:

> “significativo em subgroup A, não significativo em subgroup B; logo os subgroups diferem.”

Isso é incorreto sem um teste/interpretação de **interaction** apropriado.

Mesmo interaction prespecified precisa ser julgada com magnitude, CI, multiplicity e plausibilidade.

F0.6 ensina a estrutura; modelagem detalhada de interaction não é objetivo principal.

---

# 21. Exploratory analyses não são “inferiores” por definição

Exploração é essencial para ciência.

Ela pode:

- gerar hipóteses;
- localizar padrões inesperados;
- sugerir mediadores/modificadores;
- informar estudos futuros.

O problema é **relabeling**:

`exploratory descoberta após dados → escrita como hipótese confirmatória prespecified`.

Uma boa análise exploratória é:

- identificada como exploratória;
- transparente sobre quantas oportunidades analíticas existiram;
- acompanhada de estimates/CIs;
- interpretada como geradora de hipótese quando apropriado;
- sujeita a validação/replicação posterior.

---

# 22. Researcher degrees of freedom / analytical flexibility

Um dataset raramente possui apenas um caminho analítico possível.

Escolhas podem incluir:

- outcome definition;
- time window;
- exclusion rules;
- missing-data handling;
- transformation;
- covariates;
- interaction terms;
- subgroup definitions;
- model family;
- analysis population;
- outlier handling;
- stopping rule;
- reporting threshold.

Isso é **analytical flexibility**.

Flexibilidade não é automaticamente misconduct.

Ela se torna problemática para error control e interpretabilidade quando:

1. muitas opções são experimentadas;
2. resultados influenciam quais opções são mantidas;
3. só o caminho favorável é reportado;
4. o leitor é levado a acreditar que aquele caminho foi planejado de antemão.

---

# 23. O “garden of forking paths” em linguagem operacional

Mesmo sem rodar conscientemente 200 modelos, decisões podem depender do que foi visto:

- “se baseline estiver desequilibrado, ajustamos”;
- “se um outlier mudar p, removemos”;
- “se week 12 não der, mostramos week 8”;
- “se total sample não der, tentamos subgroup”.

Cada bifurcação pode alterar o resultado selecionado.

Por isso a pergunta não é apenas:

> “quantos p-values aparecem na tabela?”

É também:

> **quantos caminhos de análise poderiam plausivelmente ter produzido o resultado que foi escolhido para aparecer?**

---

# 24. Trial registration, preregistration, protocol e SAP

Esses documentos têm funções diferentes.

## 24.1 Trial registration

Registro público mínimo do estudo, idealmente antes do início/recrutamento conforme o contexto.

Pode expor:

- primary outcomes;
- secondary outcomes;
- timing;
- intervention/comparator;
- sample-size target;
- status/dates.

Mas registros podem ser resumidos e ambíguos.

## 24.2 Preregistration

Registro timestamped de hipóteses/métodos/analyses antes de observar resultados relevantes.

Pode ser mais ou menos detalhado.

## 24.3 Protocol

Documento mais amplo do desenho e métodos planejados.

CONSORT 2025 reforça acesso ao protocolo e sua relação com transparência de métodos.

## 24.4 Statistical Analysis Plan (SAP)

Documento detalhando como análises serão executadas.

Pode incluir:

- primary/secondary analyses;
- analysis population;
- covariates;
- missing data;
- transformations;
- subgroup analyses;
- multiplicity strategy;
- sensitivity analyses.

CONSORT 2025 inclui explicitamente trial registration e acesso ao protocol/SAP em sua seção de open science.

---

# 25. Timing, versioning e deviations importam

Um arquivo chamado “protocol.pdf” não prova prespecification.

Pergunte:

- quando foi criado?
- quando foi registrado?
- houve versão anterior?
- quando dados ficaram disponíveis?
- SAP foi finalizado antes de unblinding/data lock quando pertinente?
- alterações foram registradas?
- existe rationale para mudanças?

CONSORT 2025 recomenda tornar acessíveis protocol/SAP e documentar mudanças com timing/rationale.

A questão é **audit trail**.

---

# 26. Preregistration não é garantia de baixo bias

Critical principle:

> **prespecification/transparency reduz ambiguidade sobre o que foi planejado; não certifica que o plano era cientificamente correto.**

Um estudo preregistered ainda pode ter:

- outcome inválido;
- randomização ruim;
- missingness problemática;
- baixa adesão;
- measurement bias;
- estimand inadequado;
- análise estatística imprópria;
- amostra não aplicável;
- effect estimate trivial;
- baixa precisão.

Logo:

`preregistered ≠ low risk of bias`

Assim como:

`CONSORT-complete ≠ high-quality trial`.

Transparência facilita appraisal; não substitui appraisal.

---

# 27. Confirmatory versus exploratory

## Confirmatory

Um claim confirmatório exige maior clareza sobre:

- hipótese/estimand;
- primary outcome/time point;
- effect measure;
- analysis population;
- model/contrast;
- multiplicity strategy;
- alpha/decision rule quando teste formal for usado;
- sample-size rationale;
- protocol/SAP;
- deviations.

## Exploratory

Pode envolver:

- vários outcomes;
- subgroups;
- alternative models;
- pattern discovery;
- post hoc hypotheses.

A linguagem deve refletir isso.

### Não existe vergonha em “exploratory”

O erro científico é esconder exploração sob aparência confirmatória.

---

# 28. ASA 2016 e ASA 2021: duas proteções complementares

## ASA 2016

Protege contra:

- p-value como probabilidade de hipótese;
- threshold como decisão científica suficiente;
- esconder analyses;
- p-value como effect size/importance.

## ASA Task Force 2021

Protege contra overcorrection:

> “como p-values são mal usados, p-values não servem para nada.”

O Task Force afirma que p-values/significance tests podem ser ferramentas úteis quando corretamente aplicados e interpretados, enfatizando uncertainty, variability, multiplicity e replicability.

F0.6 conclui:

> **não idolatrar nem banir um número; especificar o procedimento, controlar os erros relevantes e interpretar resultados no contexto completo.**

---

# 29. Worked example — power antes do estudo

Planejamento sintético:

- two-group randomized study;
- outcome contínuo;
- alpha `0.05` bilateral;
- target difference `+2.0`;
- SD esperada `4.0`;
- desired power `80%`.

Interpretação correta:

> O n é escolhido para que, se o verdadeiro efeito for +2.0 e as assumptions de variabilidade/modelo forem adequadas, o procedimento tenha aproximadamente 80% de chance de rejeitar H0 nas repetições do desenho.

Não conclua:

> “Existe 80% de chance de +2 ser o efeito verdadeiro.”

---

# 30. Worked example — resultado depois do estudo

Resultado observado:

`MD = +0.8`

`95% CI = −0.6 a +2.2`

`p = 0.26`

SESOI = `+2.0`.

### Leitura F0.5

- estimate positivo, +0.8;
- CI inclui pequeno dano/trivialidade e benefício acima do SESOI;
- impreciso para decidir se há benefício relevante.

### Leitura F0.6

Mesmo que o planejamento declarasse 80% power para +2.0:

- isso não transforma `p=0.26` em “20% chance de false negative”;
- observed power baseado em +0.8 não resolve o significado do resultado;
- o CI continua sendo a informação direta sobre a precisão observada.

---

# 31. Worked example — multiplicidade simples

Um paper mede 20 outcomes independentes e trata qualquer `p<0.05` como confirmação de eficácia.

Sob a hipótese ilustrativa de que todos os nulls são verdadeiros e os testes são independentes:

`P(≥1 false positive) = 1 − 0.95^20 ≈ 0.642`.

Ou cerca de `64.2%`.

Isso não significa que o paper tem “64.2% de chance de estar errado”.

Significa:

> sob esse cenário matemático simplificado e essa estratégia de procurar qualquer positivo, o procedimento produz pelo menos uma rejeição Type I em cerca de 64% das repetições.

---

# 32. Worked example — analytical flexibility

Estudo registra:

- primary outcome = performance at week 12;
- model = change adjusted for baseline;
- alpha = 0.05.

Depois dos dados:

- week 12 primary: p=0.18;
- pesquisador testa weeks 4/8/12;
- remove dois outliers sob três rules;
- testa quatro covariate sets;
- divide por sex e baseline fitness;
- reporta apenas week 8, sem outliers, adjusted model, subgroup “high fitness”, p=0.012.

A pergunta central não é:

> “0.012 é menor que 0.05?”

É:

1. esse claim era prespecified?
2. quantos caminhos analíticos existiram?
3. qual family of hypotheses deveria ser considerada?
4. o p-value foi selecionado após múltiplas tentativas?
5. protocol/SAP registram essas decisões?
6. o resultado deve ser classificado como exploratory?

---

# 33. Performance framework para auditar um estudo

Use esta sequência:

`1. Target claims → 2. Decision rules → 3. Power/sample-size assumptions → 4. Effective hypothesis family → 5. Analytical paths → 6. Prespecification evidence → 7. Multiplicity control → 8. Estimate/CI interpretation → 9. Confirmatory vs exploratory → 10. Transparent conclusion`

## 33.1 Target claims

O que o study quer provar/estimar?

## 33.2 Decision rules

Qual alpha/test/criterion?

## 33.3 Planning

Power para qual effect? Qual SESOI? Qual precision target?

## 33.4 Family

Quais outcomes/time points/subgroups/models alimentam os mesmos claims?

## 33.5 Analytical paths

Quantos caminhos possíveis existiam?

## 33.6 Prespecification

Registration/protocol/SAP mostram o quê?

## 33.7 Multiplicity control

Existe hierarchy, adjustment, alpha allocation ou classificação exploratory?

## 33.8 F0.5 interpretation

Magnitude + CI + practical threshold continuam obrigatórios.

## 33.9 Label

Confirmatory, supportive ou exploratory?

## 33.10 Conclusion

O que é suportado e o que não é?

---

# 34. Integrated audit scenario

Estudo sintético:

- 120 atletas randomizados para estratégia A ou B;
- registry anterior ao recrutamento declara:
  - primary outcome: time-trial performance em week 12;
  - three secondary outcomes em week 12;
  - alpha 0.05 bilateral;
  - target difference para planejamento: 2.0%;
  - power planejado: 80%;
- registro não contém multiplicity strategy para secondaries;
- SAP não está linkado no paper.

Paper reporta:

- primary week-12 effect = `+0.6%`, 95% CI `−0.5% a +1.7%`, p=`0.28`;
- além disso, analisa 20 outcomes em 4 time points = 80 main outcome-time tests;
- analisa 6 subgroup definitions sobre os 20 outcomes em week 12 = até 120 subgroup interaction tests;
- para vários outcomes, testa 3 covariate models e reporta o modelo com menor p;
- destaca:
  - mood em week 8, p=`0.008`;
  - subgroup “high baseline fitness” para recovery, p=`0.03`;
- chama ambos de “confirmatory evidence”;
- não apresenta lista completa dos resultados testados nem rationale de deviations.

### Auditoria esperada

**Original confirmatory target:** primary time-trial outcome em week 12.

**Primary result:** CI `−0.5% a +1.7%` fica abaixo do planning target +2.0%, mas practical threshold precisa estar claramente definido para concluir relevância; `p=0.28` não significa ausência de efeito.

**Multiplicity:** 80 outcome-time tests + grande número de subgroup interactions + model variants criam muitas oportunidades de seleção.

**Important nuance:** 3 models para uma mesma outcome-time comparison podem ser diferentes **analytical paths**, não necessariamente 3 independent scientific hypotheses. Não multiplique contagens mecanicamente sem definir family/claim.

**Prespecification:** registry sustenta que primary week12 foi planejado, mas não demonstra que mood-week8/subgroup/model selection foram confirmatórios.

**SAP:** ausência de acesso não prova por si só que nenhum SAP existiu, mas impede auditoria completa de prespecification.

**Classification:** mood/subgroup findings devem ser tratados como exploratory/post hoc a menos que evidência documental mostre prespecification e multiplicity control apropriados.

**Transparent report:** deve mostrar primary outcome independentemente de p, identificar analyses post hoc, reportar full family/result set, estimates/CIs, multiplicity strategy e deviations.

---

# 35. Critical-fail statements

Rejeite estas afirmações:

1. `Power = 80%` significa 80% de chance de H1 ser verdadeira.
2. `1 − power` é a probabilidade de este resultado não significativo ser false negative.
3. Um observed power de 25% prova que o estudo falhou por falta de power.
4. Um p>0.05 pode ser explicado definitivamente calculando observed power a partir do effect observado.
5. Cada p<0.05 entre 20 outcomes é confirmação independente se cada teste usou alpha=0.05.
6. Se o primary falhou, é equivalente escolher qualquer secondary com p<0.05 como novo primary.
7. Subgroup A significativo e subgroup B não significativo prova interaction.
8. Preregistration garante low risk of bias.
9. Registration e protocol são a mesma coisa em nível de detalhe.
10. Um SAP criado depois de ver os resultados prova prespecification.
11. Multiplicity só existe quando há muitos endpoints; time points/models/subgroups nunca contam.
12. Todo resultado exploratory deve ser descartado.
13. Bonferroni é obrigatório e ótimo em qualquer situação.
14. High power corrige confounding ou measurement bias.
15. Um estudo “bem powered” dispensa magnitude e CI.

---

# 36. Active recall

Sem consultar a aula:

1. Defina Type I error e alpha sem usar probabilidade posterior.
2. Defina Type II error e explique por que beta depende do effect size considerado.
3. Defina power em uma frase contendo `effect`, `design` e `repeated sampling`.
4. Por que “80% power” é incompleto sem dizer para qual effect?
5. Diferencie power e precision.
6. Por que observed power calculado com o effect observado é geralmente não informativo?
7. O que usar pós-estudo em vez de observed power?
8. Cite quatro fatores que alteram power.
9. Qual a função de SESOI no sample-size planning?
10. Calcule `1 − 0.95^5` e interprete corretamente.
11. Defina family of hypotheses.
12. Cite cinco fontes de multiplicity.
13. Explique diferença entre hypothesis multiplicity e analytical-path multiplicity.
14. Para que serve endpoint hierarchy?
15. O que Bonferroni ilustra?
16. Por que subgroup significant vs nonsignificant não prova diferença entre subgroups?
17. Diferencie trial registration, protocol e SAP.
18. Por que timing/versioning de SAP importa?
19. Por que preregistration não garante low bias?
20. Diferencie confirmatory de exploratory sem tratar exploration como ciência ruim.

---

# 37. Integração com F0.4 e F0.5

## F0.4

Fornece:

- sampling variability;
- SD/SE;
- efeito de n sobre precisão.

## F0.5

Fornece:

- estimates;
- CI;
- p-value;
- magnitude;
- practical thresholds.

## F0.6

Adiciona:

- comportamento repetido das decision rules;
- prospective power;
- multiplicity;
- analytical flexibility;
- prespecification;
- confirmatory/exploratory distinction.

Nenhuma camada substitui a anterior.

---

# 38. Limites deliberados

F0.6 não ensina em profundidade:

- derivação matemática de noncentral distributions;
- cálculo manual de power para todos os modelos;
- exhaustive catalog de corrections;
- FDR em profundidade;
- adaptive/sequential trial theory completa;
- equivalence/noninferiority power formal;
- Bayesian decision theory;
- meta-analysis;
- heterogeneity/I²;
- publication-bias methods;
- meta-regression.

Meta-analysis e heterogeneity pertencem à F0.7.

---

# 39. Fontes e função

## `F0-S01` — CONSORT 2025

Função:

- trial registration;
- acesso ao protocol/SAP;
- transparência de statistical methods;
- documentação de prespecified versus post hoc/deviations.

Limite:

- reporting guideline; não é risk-of-bias score nem garante validade.

## `F0-S08` — ASA 2016

Função:

- threshold não substitui reasoning;
- full reporting/transparency;
- p-value não mede effect size/importance.

## `F0-S09` — ASA Task Force 2021

Função:

- uncertainty, variability, multiplicity e replicability;
- p-values podem ser úteis quando corretamente usados.

## `F0-S10` — FDA Multiple Endpoints 2022

Função:

- por que multiple endpoints criam false-conclusion risk;
- family/hierarchy/grouping/order;
- multiplicity management em confirmatory trials.

Limite:

- regulatory drug/biologic context; princípios matemáticos transferem, requisitos regulatórios não são universalizados.

## `F0-S13` — Lakens 2022

Função:

- sample-size justification;
- a-priori power;
- desired accuracy;
- SESOI/informational goals.

## `F0-S28` — Greenland et al. 2016

Função:

- proteger contra probability reversals envolvendo p-values/power;
- integrar uncertainty e assumptions.

## `F0-S29` — Heinsberg & Weeks 2022

Função:

- observed/post hoc power é misleading/redundant para interpretar dados já observados;
- usar estimate/CI e design reasoning em vez de explicar nonsignificance por observed power.

---

# 40. Regra final

Ao auditar um estudo, não pergunte apenas:

> “teve power suficiente?”

Pergunte:

> **para qual effect e objetivo o estudo foi planejado, qual precisão realmente foi observada, qual family de claims foi testada, quantas escolhas analíticas poderiam gerar resultados selecionáveis, o que foi prespecified, como multiplicity foi tratada e quais conclusions permanecem suportadas por estimates/CI e pelo desenho?**
