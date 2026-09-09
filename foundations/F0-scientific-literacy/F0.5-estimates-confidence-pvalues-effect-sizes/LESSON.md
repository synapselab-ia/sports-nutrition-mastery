# F0.5 — Estimativas, intervalos de confiança, p-values, effect sizes e relevância prática

**Production state:** `APPROVED`

**Prerequisite P2:** F0.4 — estatística descritiva, distribuições e variação amostral.

**P0 ensinados localmente:** parâmetro, estimador, estimativa, estimativa pontual, estimativa intervalar, hipótese nula, p-value, intervalo de confiança, effect size, risk, odds, mean difference, standardized mean difference, risk difference, risk ratio, odds ratio, menor efeito de interesse/decision threshold.

**P1 ensinados localmente:** razão e reciprocidade; intuição de escala logarítmica para medidas de razão; uso conceitual de erro-padrão na incerteza.

**Core/method sources:** `F0-S06`, `F0-S08`, `F0-S09`, `F0-S12`, `F0-S13`, `F0-S27`, `F0-S28`.

## 1. Competência-alvo

Ao terminar esta unidade, você deve conseguir receber um resultado estatístico e separar, em ordem:

1. **qual parâmetro/efeito está sendo estimado?**
2. **qual é a estimativa pontual?**
3. **qual é a escala da medida de efeito?**
4. **quão precisa é a estimativa?**
5. **quais valores do efeito permanecem compatíveis com os dados e o modelo?**
6. **o que o p-value diz e, principalmente, o que ele não diz?**
7. **o efeito é grande ou pequeno na unidade original ou relativa?**
8. **o efeito ultrapassa algum limiar de importância previamente defensável?**
9. **qual é a diferença entre importância estatística e importância prática?**
10. **que conclusão permanece suportada depois de considerar desenho, bias, magnitude, precisão e contexto?**

A regra central é:

> **um resultado estatístico não deve ser reduzido a “significativo” ou “não significativo”. Interpretação exige direção, magnitude, precisão, escala, contexto e limites de inferência.**

F0.4 ensinou de onde vem a variação amostral e separou SD de SE. F0.5 usa essa base para interpretar estimativas e sua incerteza. F0.6 ensinará formalmente Type I/II error, power, multiplicidade e analytical flexibility.

---

# 2. Parâmetro, estimador e estimativa

## 2.1 Parâmetro

Um **parâmetro** é uma quantidade definida para a população ou processo-alvo.

Exemplos conceituais:

- diferença média verdadeira entre estratégias A e B;
- risco verdadeiro de um evento sob A;
- risk ratio verdadeiro entre A e B;
- efeito médio causal definido por um estimand.

O parâmetro costuma ser desconhecido.

## 2.2 Estimador

Um **estimador** é uma regra estatística usada para estimar um parâmetro a partir dos dados.

Exemplo simples:

`diferença entre as médias amostrais`

pode ser um estimador de uma diferença média populacional sob condições apropriadas.

## 2.3 Estimativa

A **estimativa** é o valor obtido quando o estimador é aplicado ao dataset observado.

Se:

- média do grupo A = `4,2`;
- média do grupo B = `2,8`;

então a estimativa pontual da diferença `A − B` é:

`4,2 − 2,8 = 1,4 unidade`.

Não confunda:

- parâmetro = alvo desconhecido;
- estimador = regra;
- estimativa = resultado observado da regra.

---

# 3. Estimativa pontual versus estimativa intervalar

## 3.1 Estimativa pontual

Uma **estimativa pontual** resume o efeito em um único número.

Exemplo:

`MD = +1,4`.

Isso informa direção e magnitude observada, mas não mostra sozinho a incerteza amostral.

## 3.2 Estimativa intervalar

Uma **estimativa intervalar** fornece um intervalo construído por um procedimento estatístico para refletir incerteza sobre o parâmetro.

O exemplo mais comum nesta unidade é o **confidence interval (CI)**.

O CI não substitui a estimativa pontual. Os dois devem ser lidos juntos:

`estimativa pontual + intervalo + contexto`

---

# 4. Do SE ao intervalo de confiança

F0.4 separou:

- **SD** = dispersão dos valores individuais;
- **SE** = variação amostral/precisão de uma estimativa.

Em muitos estimadores aproximadamente normais, um intervalo de 95% assume conceitualmente a forma:

`estimativa ± valor crítico × SE`

Para uma aproximação normal simples:

`estimativa ± 1,96 × SE`.

Isso **não** é uma fórmula universal para todo estimador e todo desenho. O valor crítico e o SE dependem do modelo, do tamanho amostral e da estrutura dos dados.

### Exemplo sintético

Suponha:

- diferença média estimada `A − B = +1,4`;
- `SE = 1,14`.

A aproximação de 95% seria:

`1,4 ± 1,96 × 1,14`

aproximadamente:

`−0,84 a +3,64`.

A estimativa pontual é `+1,4`, mas o intervalo mostra que os dados são compatíveis, sob o modelo adotado, com efeitos em uma faixa bem mais ampla.

---

# 5. O que significa um 95% confidence interval em abordagem frequentista

## 5.1 A interpretação de repeated sampling

Em uma abordagem frequentista, o nível de 95% pertence ao **procedimento de construção do intervalo**.

Se repetíssemos o processo amostral e calculássemos um CI de 95% de forma válida em cada repetição, aproximadamente 95% desses intervalos cobririam o parâmetro verdadeiro fixo no longo prazo.

Portanto, depois de observar um intervalo específico, a formulação:

> “há 95% de probabilidade de o parâmetro verdadeiro estar dentro deste intervalo”

não é a interpretação frequentista padrão.

O parâmetro é tratado como fixo; o intervalo é o objeto aleatório antes da coleta dos dados.

## 5.2 Linguagem operacional útil

Uma forma pedagógica mais segura é dizer:

> **sob o modelo e os pressupostos usados, o intervalo mostra uma faixa de valores do parâmetro que permanecem relativamente compatíveis com os dados.**

Isso evita transformar o CI em uma distribuição posterior bayesiana.

### Cuidado

“Compatível” não significa:

- igualmente provável em todos os pontos do intervalo;
- impossível fora do intervalo;
- garantidamente verdadeiro dentro do intervalo.

O CI depende de:

- desenho;
- modelo;
- erro-padrão;
- assumptions;
- seleção/análise dos dados;
- ausência de bias relevante não tratado.

F0.3 continua valendo: um CI estreito ao redor de uma estimativa enviesada pode ser uma descrição precisa do valor errado.

---

# 6. O null value depende da escala

A hipótese nula frequentemente testa “nenhuma diferença” ou “nenhuma associação”, mas o valor nulo depende da medida.

## Medidas de diferença

Exemplos:

- mean difference;
- risk difference.

Null value:

`0`.

## Medidas de razão

Exemplos:

- risk ratio;
- odds ratio.

Null value:

`1`.

Isso acontece porque:

- diferença zero = grupos iguais naquela escala;
- razão 1 = numerador e denominador iguais naquela escala.

---

# 7. O que um p-value é

Uma definição operacional coerente com a ASA é:

> **o p-value quantifica quão incompatíveis os dados observados são com um modelo estatístico especificado, usualmente incluindo uma hipótese nula, por meio da probabilidade de observar um resultado/test statistic pelo menos tão extremo quanto o observado se o modelo usado para calcular o p-value fosse válido.**

Em linguagem mais simples:

1. assuma temporariamente o modelo/hypótese usados no teste;
2. pergunte quão extremos seriam dados como os observados sob essas assumptions;
3. um p-value menor representa maior incompatibilidade dos dados com aquele modelo, nas condições do teste.

O p-value é calculado **condicionando-se às assumptions**; ele não calcula diretamente a probabilidade dessas assumptions serem verdadeiras.

---

# 8. Os seis princípios centrais da ASA

F0.5 preserva os seis princípios em forma operacional.

## Princípio 1 — incompatibilidade com modelo

P-values podem indicar o grau de incompatibilidade entre os dados e um modelo estatístico especificado.

## Princípio 2 — não é probabilidade da hipótese

Um p-value não é:

- `P(H0 verdadeira | dados)`;
- a probabilidade de que “o acaso produziu os dados”.

A direção lógica é outra: o cálculo assume o modelo para avaliar a distribuição dos dados/test statistic.

## Princípio 3 — threshold não decide ciência

Conclusões científicas ou decisões não devem depender apenas de atravessar um cutoff como `0,05`.

`p = 0,049` e `p = 0,051` não representam universos científicos opostos.

## Princípio 4 — inferência exige transparência

Seleção de análises, outcomes, subgrupos ou modelos com base nos resultados compromete a interpretação. F0.6 aprofundará multiplicidade e analytical flexibility.

## Princípio 5 — p não mede magnitude/importância

Um p-value não mede:

- tamanho do efeito;
- relevância prática;
- benefício real;
- importância clínica/esportiva.

## Princípio 6 — p isolado não mede “evidência” de modo suficiente

O p-value isolado não resume desenho, bias, magnitude, precisão, plausibilidade, multiplicidade, prior evidence ou aplicabilidade.

---

# 9. Erros clássicos com p-values

## Erro 1

> `p = 0,03` significa 3% de chance de H0 ser verdadeira.

**Errado.**

## Erro 2

> `p < 0,05` prova que existe efeito real.

**Errado.** Um p pequeno pode coexistir com bias, model misspecification, seleção de análise, efeito trivial ou outros problemas.

## Erro 3

> `p > 0,05` prova que não existe efeito.

**Errado.** Um p grande pode ocorrer com estimativa imprecisa, efeito pequeno, amostra limitada ou várias outras estruturas.

## Erro 4

> `p = 0,049` é cientificamente diferente de `p = 0,051`.

**Errado** como classificação substantiva automática.

## Erro 5

> Quanto menor o p, maior necessariamente o efeito.

**Errado.** p depende da relação entre magnitude, variabilidade, tamanho amostral e modelo/teste.

## Erro 6

> Se o resultado é “significativo”, ele é importante.

**Errado.** Importância exige escala, magnitude, contexto e decision threshold.

---

# 10. Por que “significant / nonsignificant” perde informação

Considere dois resultados sintéticos para a mesma escala, com menor efeito de interesse definido como `+1,0` unidade.

## Estudo A

`efeito = +0,20`

`95% CI = +0,05 a +0,35`

`p = 0,01`

O resultado pode ser estatisticamente incompatível com zero, mas o intervalo inteiro fica abaixo do limiar prático de `+1,0`.

Dentro desse contexto definido, os dados são precisos e compatíveis apenas com efeitos **menores que o limiar de interesse**.

## Estudo B

`efeito = +1,40`

`95% CI = −0,84 a +3,64`

`p ≈ 0,22`

O resultado não cruza um threshold de significância convencional, mas o CI é compatível com:

- pequeno efeito negativo;
- efeito trivial/próximo de zero;
- efeito acima do limiar `+1,0`;
- efeito potencialmente grande.

A conclusão correta não é “não funcionou”.

A conclusão é:

> **a estimativa é positiva, porém imprecisa; os dados não distinguem adequadamente entre efeitos negativos pequenos, efeitos triviais e benefícios potencialmente relevantes.**

---

# 11. Direction, magnitude e precision

Uma leitura quantitativa deve separar pelo menos três dimensões.

## Direction

Qual lado da escala favorece qual condição?

Exemplo:

- `MD > 0` pode favorecer A se maior for melhor;
- em tempo de prova, `MD < 0` pode favorecer A se menor for melhor.

A direção precisa ser definida pela variável, não pelo sinal isolado.

## Magnitude

Qual é o tamanho da diferença na escala escolhida?

Exemplo:

`+1,4 kg`, `−8 pontos percentuais`, `RR = 0,60`.

## Precision

Quão estreita é a incerteza em torno da estimativa?

CI mais estreito geralmente indica maior precisão relativa naquela escala/modelo.

Mas:

> **precisão não é validade.**

Um estudo pode ser muito preciso e sistematicamente enviesado.

---

# 12. Effect size: o que significa

**Effect size** é uma medida quantitativa da magnitude de uma diferença, associação ou efeito na escala definida.

Não existe um único “effect size”.

Exemplos:

- mean difference;
- standardized mean difference;
- risk difference;
- risk ratio;
- odds ratio.

A interpretação depende da escala e do contexto.

---

# 13. Mean difference (MD)

Para outcome contínuo:

`MD = média_A − média_B`

### Exemplo

Aumento médio sintético em uma variável de desempenho:

- A = `4,2 unidades`;
- B = `2,8 unidades`.

`MD = +1,4 unidade`.

Vantagem:

- permanece na unidade original;
- costuma ser diretamente interpretável quando a escala tem significado claro.

Limitação:

- não é comparável de forma direta entre outcomes medidos em escalas diferentes.

---

# 14. Standardized mean difference (SMD)

Quando estudos medem um construto semelhante em escalas diferentes, uma diferença padronizada pode ser usada.

Conceitualmente:

`SMD = diferença entre médias / medida de SD usada para padronização`.

O resultado fica em unidades de desvio-padrão.

Exemplo:

`SMD = 0,50`

significa que a diferença média equivale a aproximadamente meia unidade da dispersão usada na padronização.

### Erro crítico

Não transforme automaticamente:

- `0,2 = pequeno`;
- `0,5 = médio`;
- `0,8 = grande`

em relevância prática universal.

Essas convenções podem ser referências descritivas em alguns contextos, mas **não substituem** conhecimento da escala, variabilidade, população, outcome e decisão.

Um SMD maior não é intrinsecamente “clinicamente” ou “esportivamente” importante.

---

# 15. Outcomes binários: risco

Considere um evento que pode ocorrer ou não.

`risk = número com evento / número total`

Exemplo sintético:

- A: `12/100 = 0,12 = 12%`;
- B: `20/100 = 0,20 = 20%`.

---

# 16. Risk difference (RD)

`RD = risk_A − risk_B`

No exemplo:

`0,12 − 0,20 = −0,08`.

Ou:

`−8 pontos percentuais`.

RD é uma medida **absoluta**.

Ela responde:

> quantos pontos percentuais o risco difere entre os grupos?

---

# 17. Risk ratio (RR)

`RR = risk_A / risk_B`

No exemplo:

`0,12 / 0,20 = 0,60`.

Interpretação:

- risco em A = 60% do risco em B;
- equivalente a redução relativa de 40%, se a direção/contexto justificarem essa linguagem.

RR é uma medida **relativa**.

Null value:

`RR = 1`.

---

# 18. Odds e odds ratio (OR)

## 18.1 Odds

Se o risco é `p`:

`odds = p / (1 − p)`.

Para A:

`0,12 / 0,88 ≈ 0,136`.

Para B:

`0,20 / 0,80 = 0,25`.

## 18.2 Odds ratio

`OR = odds_A / odds_B`.

No exemplo:

`OR ≈ 0,136 / 0,25 ≈ 0,55`.

### RR não é OR

No mesmo dataset:

- `RR = 0,60`;
- `OR ≈ 0,55`.

Quando eventos são raros, OR e RR podem ser numericamente próximos. Quando eventos são comuns, podem divergir bastante.

Portanto, nunca interprete OR como se fosse automaticamente RR.

---

# 19. Por que efeito relativo precisa de baseline absoluto

Considere dois cenários com o mesmo `RR = 0,50`.

## Cenário 1

- B: 20%;
- A: 10%.

RD = `−10 pontos percentuais`.

## Cenário 2

- B: 2%;
- A: 1%.

RD = `−1 ponto percentual`.

O efeito relativo é o mesmo, mas o impacto absoluto é muito diferente.

Logo:

> **medidas relativas sem baseline podem exagerar ou ocultar a importância prática. Sempre procure também uma escala absoluta quando possível.**

---

# 20. Escala logarítmica para medidas de razão — P1

Razões têm assimetria aritmética na escala original:

- metade = `0,5`;
- dobro = `2,0`.

Esses valores são recíprocos em torno de `1`, mas não estão igualmente distantes de 1 na escala linear.

Aplicando log:

- `log(0,5) = −log(2)`;
- `log(1) = 0`.

Por isso, medidas como RR e OR são frequentemente analisadas ou mostradas em escala logarítmica em forest plots.

Você não precisa calcular logs manualmente nesta unidade. Precisa entender:

- null = 1 na escala de razão;
- reciprocidade fica simétrica na escala log;
- leitura visual de forest plots com razões deve respeitar a escala.

---

# 21. Menor efeito de interesse / decision threshold

A pergunta “existe qualquer efeito não zero?” muitas vezes é menos útil que:

> **qual magnitude seria grande o suficiente para importar para a pergunta científica ou decisão?**

Um **smallest effect of interest (SESOI)** ou **decision threshold** é um limiar definido para distinguir efeitos que seriam substantivamente relevantes de efeitos pequenos demais para mudar interpretação/decisão.

### Características importantes

- não existe valor universal;
- deve ser justificado pela escala e contexto;
- idealmente é definido antes de olhar o resultado principal;
- pode ser assimétrico para benefício e dano;
- pode refletir custo, risco, viabilidade ou significado fisiológico/prático.

Ele não é “verdade estatística”. É parte explícita da pergunta/decisão.

---

# 22. Ler CI em relação a thresholds

Suponha:

- benefício relevante: `>= +1,0`;
- efeito trivial: entre `−1,0` e `+1,0`;
- dano relevante: `<= −1,0`.

## Caso A

`estimate = +1,8`

`95% CI = +1,2 a +2,4`

Sob o modelo, todos os valores do intervalo estão acima do threshold de benefício.

## Caso B

`estimate = +0,2`

`95% CI = +0,05 a +0,35`

Intervalo estreito e acima de zero, mas totalmente abaixo do threshold `+1,0`.

Possível interpretação: evidência precisa de um efeito pequeno naquela escala, não de um benefício praticamente importante.

## Caso C

`estimate = +1,4`

`95% CI = −0,84 a +3,64`

Intervalo cruza:

- valores negativos pequenos;
- zero;
- zona trivial;
- threshold de benefício;
- efeitos grandes.

Possível interpretação: **impreciso para decidir importância prática**.

## Caso D

`estimate = −0,1`

`95% CI = −0,4 a +0,2`

Se os thresholds relevantes forem ±1,0, o intervalo inteiro exclui efeitos relevantes em ambas as direções.

Esse é um caso em que um resultado próximo de zero pode ser **informativo**, porque a precisão é suficiente para excluir efeitos considerados importantes sob o threshold definido.

---

# 23. “Não significativo” versus “evidência de ausência relevante”

Compare:

## Estudo X

`estimate = 0,0`

`95% CI = −5 a +5`

## Estudo Y

`estimate = 0,0`

`95% CI = −0,3 a +0,3`

Ambos podem ter p-values altos contra H0=0.

Mas não são igualmente informativos.

Se ±1,0 é o limite de importância:

- X continua compatível com efeitos relevantes de benefício e dano;
- Y exclui, sob o modelo, efeitos maiores que ±0,3 e portanto fornece informação muito mais forte contra efeitos de magnitude relevante.

Assim:

> **p > 0,05 sozinho não distingue “não sabemos” de “estimativa suficientemente precisa para excluir efeitos importantes”.**

---

# 24. Statistical importance versus practical importance

## Statistical output

Inclui:

- estimate;
- SE;
- CI;
- p-value;
- test/model details.

## Practical importance

Depende de:

- magnitude na escala relevante;
- baseline;
- smallest effect of interest;
- custo/benefício;
- risco;
- aplicabilidade;
- duração;
- viabilidade;
- qualidade causal da evidência.

Um p-value não contém essas informações.

---

# 25. O p-value muda com n

Considere a mesma magnitude aproximada com diferentes níveis de precisão.

Com n maior:

- o SE frequentemente diminui;
- o test statistic pode aumentar em magnitude;
- o p-value pode ficar menor.

Logo, um efeito minúsculo pode gerar p muito pequeno em uma amostra enorme.

E um efeito potencialmente relevante pode gerar p alto em uma amostra pequena/imprecisa.

Isso não significa que tamanho amostral é irrelevante. Significa que:

> **p-value combina efeito e incerteza; ele não é uma escala pura de magnitude.**

Power formal fica para F0.6.

---

# 26. Forest plot: como ler uma linha

Uma linha de forest plot costuma mostrar:

- estimativa pontual;
- CI;
- null value;
- escala da medida.

## Medida de diferença

Null = `0`.

## Medida de razão

Null = `1`.

### Exemplo sintético — diferença média

`MD = +1,4`

`95% CI = −0,84 a +3,64`

Threshold de benefício relevante = `+1,0`.

Leitura correta:

**Direction:** point estimate favorece A se valores maiores forem melhores.

**Magnitude:** melhor estimativa = +1,4 unidade.

**Precision:** intervalo largo, incluindo valores de pequena desvantagem até grande benefício.

**Statistical output:** CI inclui 0 e o p-value correspondente pode ser >0,05.

**Practical importance:** intervalo inclui efeitos triviais e efeitos acima do threshold; importância permanece incerta.

**Unsupported:** não é válido concluir “A não funciona” nem “A funciona de forma importante”.

---

# 27. Trial table: leitura integrada

Considere um estudo sintético com outcome contínuo em que maior é melhor.

| Grupo | n | Mudança média | SD |
|---|---:|---:|---:|
| A | 40 | +4,2 | 5,0 |
| B | 40 | +2,8 | 5,2 |

Resultado modelado:

- `MD A−B = +1,4`;
- `95% CI = −0,84 a +3,64`;
- `p ≈ 0,22`;
- threshold de benefício relevante prespecificado = `+2,0` unidades.

### Interpretação por blocos

**1. Direction**

Point estimate favorece A.

**2. Magnitude**

A diferença média observada é +1,4 unidade.

**3. Precision**

Baixa/moderada: intervalo de aproximadamente −0,84 a +3,64.

**4. Statistical output**

O CI inclui o null 0; p ≈0,22 não mostra forte incompatibilidade com um modelo de diferença zero.

**5. Practical importance**

O CI inclui:

- pequena diferença desfavorável;
- zero/trivial;
- benefícios acima do threshold +2.

Logo a importância prática permanece incerta.

**6. Unsupported**

Não está suportado afirmar:

- ausência de efeito;
- benefício relevante comprovado;
- equivalência;
- causalidade além do que o desenho permite;
- que p=0,22 seja “22% de chance de não haver efeito”.

---

# 28. Confidence interval não é Bayesian credible interval

Em um **Bayesian credible interval**, sob um modelo bayesiano especificado e uma prior, pode-se formular probabilidade posterior sobre o parâmetro.

Em um **frequentist confidence interval**, o nível de confiança descreve a cobertura de longo prazo do procedimento sob assumptions.

F0.5 não ensina inferência bayesiana formal. A distinção existe apenas para bloquear o erro:

> “95% CI = 95% de probabilidade posterior do parâmetro estar aqui”.

---

# 29. CI não é “teste de significância desenhado como intervalo” apenas

CI e testes têm relação matemática, mas o intervalo oferece mais informação porque mostra:

- magnitude;
- direção;
- precisão;
- valores compatíveis em múltiplas hipóteses;
- relação com thresholds práticos.

Reduzir um CI a:

> “cruza zero: não significativo / não cruza: significativo”

joga fora grande parte da informação.

---

# 30. SMD e relevância prática

Imagine dois estudos:

- Estudo A: `SMD = 0,50`, mas a escala tem grande variabilidade entre indivíduos e o desfecho é pouco relevante para decisão;
- Estudo B: `SMD = 0,20`, mas uma pequena mudança na escala original é decisiva para o contexto.

A classificação por número padronizado não resolve a importância prática.

Pergunte:

- qual SD foi usada na padronização?
- qual é a escala original?
- qual população?
- qual threshold de interesse?
- o outcome importa?
- a medida é confiável?

---

# 31. Absolute versus relative effect: sempre faça a dupla leitura

Para outcome binário, procure responder:

1. qual o risco em cada grupo?
2. qual a diferença absoluta?
3. qual a razão relativa?
4. qual o baseline?
5. qual o CI de cada medida quando disponível?
6. qual magnitude seria relevante?

Um headline como:

> “redução de 50%”

é incompleto sem dizer:

- 20% → 10%?
- 2% → 1%?
- 0,2% → 0,1%?

---

# 32. Compatibilidade de múltiplos efeitos

Uma estimativa não escolhe um único “verdadeiro valor” com certeza.

Um CI amplo pode permanecer compatível com várias histórias substantivas.

Exemplo:

`MD = +1,4; 95% CI = −0,84 a +3,64`.

Dependendo do threshold:

- pequena desvantagem ainda é compatível;
- efeito próximo de zero é compatível;
- benefício moderado é compatível;
- benefício grande também pode ser compatível.

O trabalho científico é **não esconder essa pluralidade atrás de um rótulo binário**.

---

# 33. O que não pode ser inferido de CI/p-value

Mesmo um resultado com CI estreito e p pequeno não resolve automaticamente:

- confounding;
- selection bias;
- measurement bias;
- missingness;
- model misspecification;
- applicability;
- outcome importance;
- causal estimand inadequado;
- multiplicidade/selective reporting.

F0.3 continua upstream de F0.5.

---

# 34. Interpretação em seis blocos

Para qualquer resultado quantitativo de F0.5, use esta sequência:

`1. Target/measure → 2. Direction → 3. Magnitude → 4. Precision/CI → 5. Statistical output → 6. Practical meaning + unsupported claims`

Versão expandida:

1. **Target/measure:** qual parâmetro e escala?
2. **Direction:** qual lado favorece qual condição?
3. **Magnitude:** quanto?
4. **Precision:** qual intervalo e quão amplo?
5. **Statistical output:** p-value/null/model sem transformar threshold em verdade;
6. **Practical meaning:** threshold/baseline/contexto e o que continua não estabelecido.

---

# 35. Worked example — p pequeno, efeito trivial

Outcome sintético em escala onde `+1,0` é o menor efeito considerado relevante.

Resultado:

- estimate `+0,20`;
- 95% CI `+0,05 a +0,35`;
- p `0,01`.

### Leitura

**Direction:** positiva.

**Magnitude:** +0,20.

**Precision:** relativamente alta; intervalo estreito.

**Statistical output:** dados relativamente incompatíveis com null 0 sob o modelo especificado.

**Practical meaning:** intervalo inteiro abaixo de +1,0; sob esse threshold, efeitos relevantes estão excluídos na direção positiva.

**Conclusion:** existe evidência de uma diferença pequena, não de uma diferença praticamente relevante.

---

# 36. Worked example — p alto, informação ainda útil

Threshold de relevância: ±1,0.

Resultado:

- estimate `−0,10`;
- 95% CI `−0,40 a +0,20`;
- p alto contra null 0.

### Leitura

O intervalo é estreito e fica inteiramente dentro da zona considerada trivial.

Conclusão:

> **os dados são compatíveis apenas com diferenças pequenas dentro da faixa considerada trivial sob o threshold adotado, nas assumptions do modelo.**

Isso é diferente de simplesmente dizer “não significativo”.

---

# 37. Worked example — p alto e baixa informação

Threshold de relevância: ±1,0.

Resultado:

- estimate `0,0`;
- 95% CI `−4,0 a +4,0`;
- p alto.

Conclusão:

> **o estudo é impreciso; permanece compatível com efeitos relevantes em ambas as direções.**

Logo, “não significativo” não distingue o exemplo da seção 36 deste exemplo.

---

# 38. Transparência e selective reporting — ponte mínima para F0.6

O p-value pressupõe um processo de análise especificado.

Se o pesquisador:

- testa muitos outcomes;
- escolhe apenas um time point favorável;
- experimenta vários modelos;
- publica só o menor p;

então a leitura simples do p-value fica comprometida.

F0.5 precisa apenas reconhecer a ameaça.

F0.6 ensinará:

- family of hypotheses;
- Type I/II error;
- multiplicity;
- adjustment;
- preregistration;
- analytical flexibility.

---

# 39. Checklist anti-erro

Antes de concluir qualquer resultado, rejeite automaticamente estas frases:

1. `p < 0,05`, portanto H0 é falsa.
2. `p > 0,05`, portanto não existe efeito.
3. `p = 0,03`, portanto existe 97% de chance de efeito real.
4. CI de 95% significa 95% de probabilidade posterior do parâmetro estar no intervalo.
5. CI cruza zero, portanto o tratamento é inútil.
6. CI não cruza zero, portanto o efeito é importante.
7. SMD de 0,8 é universalmente “grande e importante”.
8. RR de 0,5 significa grande benefício sem precisar conhecer o baseline.
9. OR pode ser lido como RR em qualquer frequência de evento.
10. mais precisão resolve bias causal.

---

# 40. Perguntas de recuperação ativa

Sem consultar a aula, responda:

1. Diferencie parâmetro, estimador e estimativa.
2. O que significa 95% em um CI frequentista?
3. Por que `95% CI = 95% de probabilidade do parâmetro estar aqui` é uma interpretação incorreta no frequentismo?
4. Defina p-value em termos de modelo e dados.
5. Liste os seis princípios ASA em suas próprias palavras.
6. Por que p pequeno não implica efeito grande?
7. Por que p grande não prova ausência de efeito?
8. Diferencie MD e SMD.
9. Defina RD, RR e OR.
10. Explique por que o mesmo RR pode corresponder a impactos absolutos muito diferentes.
11. O que é smallest effect of interest?
12. Como um CI pode ser usado em relação a um threshold prático sem virar uma decisão binária automática?
13. Diferencie “evidência de ausência relevante” de “ausência de evidência”.
14. Por que um CI estreito não corrige confounding?
15. Quais seis blocos você deve relatar ao interpretar uma linha de forest plot?

---

# 41. Integração com F0.1–F0.4

## F0.1

Define a pergunta, outcome e estimand.

Sem isso, effect size pode estar medindo a coisa errada.

## F0.2

Define como o contraste foi criado.

Sem isso, a estimativa pode não responder à pergunta desejada.

## F0.3

Analisa systematic bias e causal validity.

Sem isso, precisão pode estar cercando um valor enviesado.

## F0.4

Define distribuição, SD, SE e sampling variation.

Sem isso, CI/p-value viram fórmulas sem objeto estatístico claro.

## F0.5

Integra:

`estimativa + incerteza + magnitude + threshold + contexto`.

---

# 42. Limites deliberados desta unidade

F0.5 **não** ensina formalmente:

- Type I/II error operating characteristics;
- cálculo de power;
- post hoc power;
- multiplicity adjustment;
- family-wise error;
- false discovery rate;
- sequential testing;
- subgroup multiplicity;
- equivalence/non-inferiority testing formal;
- Bayesian estimation;
- meta-analysis completa;
- model-based robust/clustered SE;
- causal identification além de F0.3.

Esses tópicos pertencem a F0.6 ou módulos posteriores.

---

# 43. Fontes metodológicas e função

## `F0-S06` — Cochrane Handbook Chapter 6

Função:

- mean difference;
- standardized mean difference;
- risk difference;
- risk ratio;
- odds ratio;
- diferença versus razão;
- interpretação de effect measures.

Limite: escrito para evidence synthesis e inclui detalhes além de F0.5.

## `F0-S08` — ASA Statement on p-values

Função:

- seis princípios centrais;
- bloqueio de interpretações erradas de p-values;
- p-value como parte, não substituto, de raciocínio científico.

## `F0-S09` — ASA Task Force 2021

Função:

- reforçar que p-values/testes podem ser úteis quando corretamente aplicados;
- evitar tanto ritual `p<0,05` quanto abandono simplista de métodos estatísticos;
- colocar incerteza, variabilidade, multiplicidade e replicabilidade no contexto correto.

## `F0-S12` — NIST/SEMATECH

Função:

- base frequentista de sampling, SE, confidence intervals e interpretação de parâmetros.

Limite: contexto geral/engenharia e apresentação tradicional em alguns pontos.

## `F0-S13` — Lakens 2022

Função:

- conectar informativeness, precision e inferential goals;
- introduzir smallest effect of interest/decision-relevant effect sem antecipar power formal.

## `F0-S27` — Altman & Bland

Função:

- preservar `SD ≠ SE` e a ponte F0.4 → F0.5.

## `F0-S28` — Greenland et al. 2016

Função:

- catálogo metodológico de misinterpretations de p-values, CIs e power;
- reforçar interpretação de CI como repeated-sampling procedure e bloquear probabilidades indevidas sobre hipóteses/parâmetros;
- enfatizar magnitude + confidence limits em vez de classificação binária.

---

# 44. Regra final

Ao ler um resultado, nunca termine em:

`significant / not significant`.

Termine em:

> **qual efeito foi estimado, em qual escala, com qual magnitude e precisão, quais valores ainda são compatíveis com os dados/modelo, como isso se compara ao threshold prático e quais inferências continuam não sustentadas pelo desenho e pela evidência.**
