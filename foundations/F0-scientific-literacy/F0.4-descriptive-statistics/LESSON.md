# F0.4 — Estatística descritiva, distribuições e variação amostral

**Production state:** `APPROVED`

**Prerequisite P2:** F0.1 — perguntas científicas, hipóteses e operacionalização.

**Conditional prerequisite:** `P2-QB` somente se o diagnóstico quantitativo de entrada demonstrar lacuna estrutural. Antes de respostas reais, o diagnóstico permanece `UNOBSERVED`.

**P0 ensinados localmente:** observação, variável, variável categórica/numérica, centro, dispersão, distribuição, população, amostra, parâmetro, estatística, outlier, quantil.

**P1 ensinados localmente:** razões/porcentagens quando necessárias; interpretação básica de eixos; intuição de repetição de amostras; raiz quadrada em fórmulas já fornecidas.

**Core sources:** `F0-S12`, `F0-S14`, `F0-S27`.

## 1. Competência-alvo

Ao terminar esta unidade, você deve conseguir olhar para um conjunto de dados e responder:

1. **que tipo de variável estou vendo?**
2. **como os valores se distribuem?**
3. **qual medida de centro faz sentido?**
4. **qual medida de dispersão faz sentido?**
5. **há skew, limites naturais ou valores extremos que mudam a interpretação?**
6. **qual gráfico revela a estrutura sem exagerá-la ou escondê-la?**
7. **o que pertence aos indivíduos da amostra e o que pertence à incerteza de uma estimativa?**
8. **por que duas amostras da mesma população podem produzir estatísticas diferentes?**
9. **por que SD e SE respondem perguntas diferentes?**
10. **o que muda — e o que não precisa mudar — quando o tamanho da amostra aumenta?**

A regra central é:

> **descrever dados não é reduzir tudo a uma média. Uma descrição adequada preserva o tipo da variável, a forma da distribuição, o centro, a dispersão e a estrutura visual relevante.**

F0.5 usará esses objetos para ensinar estimativas, intervalos de confiança, p-values e effect sizes. F0.6 aprofundará power e multiplicidade. Aqui o foco é construir a base descritiva e a intuição de variação amostral.

---

# 2. Da pergunta científica para os dados

F0.1 ensinou que uma pergunta precisa tornar explícitos população, contraste, outcome, tempo e estimand.

F0.4 pergunta o que acontece depois que observações aparecem.

Considere um estudo hipotético que registra:

- modalidade esportiva;
- sexo registrado no protocolo;
- anos de treinamento;
- massa corporal;
- tempo em um teste de ciclismo;
- escala ordinal de percepção de esforço;
- presença/ausência de um evento.

Essas variáveis não têm a mesma estrutura. Antes de calcular qualquer resumo, precisamos saber **o que os números ou categorias representam**.

---

# 3. Observação, variável e dataset

## 3.1 Observação

Uma **observação** é uma unidade registrada no dataset: uma pessoa, uma sessão, uma equipe, uma medição ou outra unidade definida pelo desenho.

F0.2 já mostrou que unidade de observação não é necessariamente unidade de alocação. Aqui importa porque a descrição precisa respeitar a estrutura do dado.

## 3.2 Variável

Uma **variável** é uma característica que assume valores diferentes entre observações ou ocasiões.

Exemplos:

- modalidade: corrida, ciclismo, natação;
- número de sessões semanais: 2, 3, 4, 5;
- tempo de prova: 38,2 min; 40,1 min; 42,7 min;
- classificação de esforço: leve, moderado, difícil, máximo.

A primeira decisão estatística não é “qual teste usar?”. É:

> **que tipo de informação esta variável carrega?**

---

# 4. Tipos de variável

## 4.1 Categórica nominal

Categorias sem ordem natural.

Exemplos:

- modalidade esportiva;
- grupo sanguíneo;
- braço do estudo A/B/C.

Para variáveis nominais, médias aritméticas de códigos são geralmente sem sentido. Se codificarmos `corrida=1`, `ciclismo=2`, `natação=3`, a média `2,1` não representa uma modalidade intermediária real.

Resumos típicos:

- contagens;
- proporções/percentuais;
- moda, quando útil.

## 4.2 Categórica ordinal

Categorias com ordem, mas sem garantia de que a distância entre níveis seja numericamente igual.

Exemplo:

`baixo < moderado < alto < muito alto`

A ordem contém informação. A diferença entre baixo e moderado, porém, não precisa ser a mesma que entre alto e muito alto.

## 4.3 Numérica discreta

Valores numéricos contáveis, frequentemente inteiros.

Exemplos:

- número de sessões de treino na semana;
- número de eventos adversos;
- número de repetições completas.

## 4.4 Numérica contínua

Pode assumir valores em um intervalo de uma escala de medição.

Exemplos:

- massa corporal;
- tempo;
- concentração;
- distância;
- potência.

Na prática, instrumentos arredondam valores, mas isso não transforma necessariamente a variável conceitual em discreta.

---

# 5. Escalas de mensuração: nominal, ordinal, intervalar e de razão

A classificação clássica das escalas ajuda a pensar quais operações são interpretáveis.

## 5.1 Nominal

Apenas identidade/diferença entre categorias.

## 5.2 Ordinal

Identidade + ordem.

## 5.3 Intervalar

Diferenças são interpretáveis em uma escala com intervalos comparáveis, mas o zero não representa necessariamente ausência da quantidade.

Exemplo clássico: temperatura em Celsius.

`20 °C` não é “duas vezes mais quente” que `10 °C` em sentido físico de razão.

## 5.4 Razão

Diferenças e razões podem ser interpretáveis porque existe um zero com significado de ausência da quantidade na escala relevante.

Exemplos típicos:

- duração;
- massa;
- distância.

### Cuidado

Essa tipologia é uma ferramenta de raciocínio, não uma máquina que decide toda análise automaticamente. O desenho, a distribuição, a pergunta e as propriedades do instrumento continuam importantes.

---

# 6. Distribuição: a forma dos dados

Uma **distribuição** descreve como os valores de uma variável se espalham pelo espaço possível.

Ao olhar uma distribuição, pergunte:

- onde os dados se concentram?
- quão dispersos estão?
- existem múltiplos agrupamentos?
- existe assimetria?
- há valores extremos?
- existem limites naturais, como 0–100%?

Dois datasets podem ter a mesma média e ainda serem profundamente diferentes.

Exemplo:

Dataset A:

`48, 49, 50, 50, 50, 51, 52`

Dataset B:

`35, 35, 35, 50, 65, 65, 65`

Ambos têm média 50, mas o espalhamento e a forma são diferentes.

Logo:

> **uma medida de centro sem uma medida de dispersão e sem noção da forma da distribuição é frequentemente insuficiente.**

---

# 7. Medidas de centro

## 7.1 Média aritmética

Para valores `x1, x2, ..., xn`:

`média = soma dos valores / número de valores`

Formalmente:

`x̄ = Σxi / n`

Exemplo:

`48, 49, 50, 50, 50, 51, 52`

Soma = 350.

`x̄ = 350/7 = 50`

### Propriedade importante

A média usa a magnitude de **todos** os valores. Isso a torna informativa, mas também sensível a valores extremos.

## 7.2 Mediana

A **mediana** é o valor central quando os dados são ordenados.

- se `n` é ímpar: valor do meio;
- se `n` é par: em convenção usual, média dos dois valores centrais.

Exemplo:

`32, 33, 34, 35, 36, 38, 95`

Mediana = `35`.

Média ≈ `43,3`.

O valor 95 puxa a média para cima muito mais do que altera a mediana.

### Mediana não é “sempre melhor para skew”

É frequentemente útil em distribuições fortemente assimétricas, mas a escolha depende do que se quer descrever. Média e mediana respondem a conceitos diferentes de centro.

## 7.3 Moda

A **moda** é o valor ou categoria mais frequente.

Pode ser útil para:

- categorias nominais;
- distribuições com picos claros;
- descrição de respostas mais comuns.

Pode haver:

- uma moda;
- múltiplas modas;
- nenhuma moda única útil.

---

# 8. Medidas de dispersão

## 8.1 Range / amplitude

`range = máximo − mínimo`

É simples e intuitivo, mas depende apenas de dois valores e é muito sensível a extremos.

## 8.2 Variância

A variância resume o quadrado das distâncias dos valores em relação à média.

Para uma amostra, a forma usual é:

`s² = Σ(xi − x̄)² / (n − 1)`

Por que quadrados?

- diferenças positivas e negativas não se cancelam;
- desvios maiores recebem peso maior.

Limitação didática: a unidade fica ao quadrado. Se a variável é em `kg`, a variância fica em `kg²`.

## 8.3 Desvio-padrão (SD)

O **desvio-padrão** é a raiz quadrada da variância:

`s = √s²`

Isso devolve a dispersão à unidade original.

Se o tempo é medido em minutos, o SD também é em minutos.

### O que SD descreve

SD descreve a **dispersão dos valores individuais em torno da média**.

Ele não é, por definição, a incerteza da média.

Esse contraste será decisivo quando chegarmos ao SE.

## 8.4 Quantis

Um **quantil** é um ponto que divide a distribuição ordenada segundo uma proporção.

Exemplos:

- percentil 25 = `Q1`;
- percentil 50 = mediana = `Q2`;
- percentil 75 = `Q3`.

### IQR

`IQR = Q3 − Q1`

O IQR descreve a largura do meio de aproximadamente 50% dos dados.

É menos influenciado por valores extremos do que o range e frequentemente acompanha a mediana em distribuições assimétricas.

### Convenções de quantil

Softwares podem usar regras de interpolação ligeiramente diferentes para amostras pequenas. Em exercícios, a convenção deve ser especificada quando isso puder alterar o resultado.

---

# 9. Simetria, skew e valores extremos

## 9.1 Distribuição aproximadamente simétrica

Uma distribuição é aproximadamente simétrica quando os lados em torno do centro têm formas semelhantes.

Em uma distribuição simétrica unimodal, média e mediana costumam ficar próximas.

## 9.2 Right skew / assimetria positiva

Existe uma cauda mais longa para valores altos.

Exemplo hipotético:

`32, 33, 34, 35, 36, 38, 95`

A média fica acima da mediana neste exemplo.

Mas evite a regra absoluta:

> “right skew significa sempre média > mediana”.

Isso é uma tendência comum em distribuições típicas, não uma definição matemática universal.

## 9.3 Left skew / assimetria negativa

A cauda se prolonga mais para valores baixos.

## 9.4 Outlier

Um **outlier** é um valor que se destaca do restante dos dados segundo algum critério visual, estatístico ou contextual.

Outlier não é sinônimo de erro.

Pode ser:

- erro de digitação;
- falha de instrumento;
- observação biologicamente possível e rara;
- subpopulação diferente;
- consequência legítima do processo estudado.

A atitude correta é:

`detectar → verificar origem → justificar tratamento → documentar`

Nunca:

`valor inconveniente → apagar`.

---

# 10. Qual resumo usar?

Não existe tabela universal, mas um bom ponto de partida é:

## Distribuição aproximadamente simétrica sem extremos dominantes

Frequentemente:

- média;
- SD.

## Distribuição fortemente assimétrica ou com extremos relevantes

Frequentemente:

- mediana;
- IQR;
- quantis adicionais;
- gráfico da distribuição.

## Variável categórica

Frequentemente:

- contagem;
- proporção/percentual;
- moda quando informativa.

### Regra mais importante

> **o resumo deve representar a estrutura real dos dados e responder à pergunta descritiva; não deve ser escolhido apenas porque é tradicional.**

---

# 11. Visualização de dados

Um gráfico é uma ferramenta analítica, não decoração.

## 11.1 Dot plot / strip plot

Útil para amostras pequenas/moderadas porque mostra valores individuais.

Pode revelar:

- clusters;
- gaps;
- outliers;
- sobreposição entre grupos.

## 11.2 Histograma

Agrupa uma variável numérica em intervalos (`bins`) e mostra a distribuição de frequências.

Útil para:

- skew;
- múltiplos picos;
- dispersão;
- caudas.

A aparência depende da largura/posição dos bins. Por isso, um único histograma não é uma verdade visual absoluta.

## 11.3 Boxplot

Resume:

- mediana;
- quartis;
- IQR;
- pontos potencialmente extremos segundo uma regra de whiskers.

É compacto, mas esconde alguns detalhes que um dot plot ou violin/density plot pode revelar.

## 11.4 Bar chart

Adequado principalmente para categorias e suas contagens/proporções.

Não confunda com histograma:

- bar chart: categorias separadas;
- histograma: intervalos de uma variável numérica contínua/discreta ordenada.

## 11.5 Scatterplot

Mostra pares `(x, y)` para duas variáveis numéricas.

Pode revelar:

- direção de associação;
- curvatura;
- clusters;
- heteroscedasticidade visual;
- pontos extremos.

Não transforma associação em causalidade; F0.3 continua valendo.

---

# 12. Como gráficos enganam

## 12.1 Eixo truncado

Suponha duas médias:

- grupo A = 50,0;
- grupo B = 50,4.

Se o eixo y vai de `0 a 60`, a diferença parece pequena.

Se vai de `49,8 a 50,5`, a diferença pode parecer enorme.

A diferença numérica continua sendo `0,4`.

Eixo truncado não é automaticamente proibido, mas precisa ser claramente mostrado e interpretado com a escala real.

## 12.2 Áreas e volumes desproporcionais

Representar quantidade por figuras cujo **comprimento e área** aumentam simultaneamente pode exagerar diferenças.

## 12.3 Omissão de variabilidade

Mostrar apenas uma barra de média pode esconder:

- dispersão ampla;
- bimodalidade;
- outliers;
- sobreposição entre grupos.

## 12.4 Escalas incompatíveis entre painéis

Comparar dois gráficos com eixos diferentes como se tivessem a mesma escala pode criar uma impressão falsa de contraste.

## 12.5 Seleção de janela

Escolher apenas um intervalo temporal conveniente pode exagerar tendência ou esconder reversão.

Pergunta de auditoria:

> **o que eu concluiria se visse os valores individuais, o eixo completo e a janela temporal mais ampla?**

---

# 13. População, amostra, parâmetro e estatística

## 13.1 População

A **população** é o conjunto de unidades sobre o qual a pergunta estatística pretende falar.

Ela precisa ser definida pela pergunta científica, não como “todo mundo”.

## 13.2 Amostra

A **amostra** é o conjunto efetivamente observado.

## 13.3 Parâmetro

Um **parâmetro** é uma característica da população-alvo, como a média populacional.

Em geral, é desconhecido.

## 13.4 Estatística

Uma **estatística** é uma quantidade calculada da amostra, como:

- média amostral;
- mediana amostral;
- SD amostral;
- proporção amostral.

Usamos estatísticas para descrever a amostra e, em etapas posteriores, aprenderemos a usá-las para inferir parâmetros.

---

# 14. Sampling variation: amostras variam

Imagine uma população muito grande de atletas com uma distribuição fixa de determinada medida.

Agora repita mentalmente:

1. sorteie 20 pessoas;
2. calcule a média;
3. devolva-as à população conceitualmente;
4. sorteie outras 20;
5. calcule outra média;
6. repita milhares de vezes.

As médias não serão idênticas.

Isso é **sampling variation**: estatísticas mudam de amostra para amostra por causa da seleção aleatória/variabilidade do processo amostral.

Sampling variation não significa que alguém “cometeu erro”. É uma consequência esperada de observar uma parte da população em vez da população inteira.

---

# 15. Sample distribution versus sampling distribution

Essa distinção é um dos pontos mais importantes da F0.4.

## 15.1 Sample distribution

É a distribuição dos **valores individuais dentro de uma amostra**.

Exemplo:

20 tempos de corrida de 20 atletas.

Pergunta:

> quão diferentes são os atletas observados?

Medidas úteis:

- SD;
- IQR;
- range;
- histograma.

## 15.2 Sampling distribution

É a distribuição de uma **estatística calculada em muitas amostras hipotéticas repetidas**.

Exemplo:

- média da amostra 1;
- média da amostra 2;
- média da amostra 3;
- ...

Pergunta:

> quanto a média amostral varia de amostra para amostra?

Essa distribuição não é formada pelos indivíduos originais; é formada por **estatísticas**.

---

# 16. Standard deviation versus standard error

## 16.1 SD

SD descreve principalmente o espalhamento dos **valores individuais** na amostra e estima a variabilidade individual na população sob o modelo amostral.

Pergunta respondida:

> quão dispersos estão os indivíduos?

## 16.2 SE

O **standard error** de uma estatística é o desvio-padrão de sua sampling distribution.

Para a média, sob condições usuais de observações independentes:

`SE(x̄) ≈ s / √n`

Pergunta respondida:

> quão variável seria esta estimativa se repetíssemos o processo de amostragem muitas vezes?

## 16.3 Exemplo

Se:

- `SD = 10`;
- `n = 25`;

então:

`SE = 10 / √25 = 2`.

Se mantivermos aproximadamente o mesmo SD e aumentarmos para `n = 100`:

`SE = 10 / √100 = 1`.

O número de indivíduos ficou quatro vezes maior e o SE caiu pela metade.

### O que não aconteceu

Não existe motivo para concluir que o SD dos indivíduos caiu de 10 para 5 apenas porque `n` aumentou.

> **mais observações tendem a tornar a média mais precisamente estimada; não tornam automaticamente os indivíduos menos diferentes entre si.**

---

# 17. O efeito de aumentar a amostra

Mantendo o mesmo processo populacional e variabilidade individual:

## Pode acontecer

- média amostral ficar mais estável entre repetições;
- SE da média diminuir aproximadamente como `1/√n`;
- extremos e detalhes da distribuição serem observados com mais resolução;
- estimativas de quantis e SD se tornarem mais estáveis.

## Não precisa acontecer

- SD diminuir;
- range diminuir — na verdade, com mais observações, extremos mais distantes podem aparecer;
- distribuição individual ficar mais estreita;
- bias desaparecer.

F0.3 já ensinou: aumentar `n` não corrige sistematicamente confounding, seleção ou erro de mensuração.

---

# 18. Transformações: mudar a escala para enxergar/representar melhor

Uma **transformação** aplica uma função a cada valor antes de descrever/modelar os dados.

Exemplo conceitual:

`y → log(y)`

Transformações logarítmicas podem ser úteis quando:

- valores são positivos;
- a escala é multiplicativa;
- existe forte right skew;
- razões são mais naturais que diferenças absolutas.

Mas transformar não é “consertar dados ruins”.

A transformação:

- muda a escala;
- muda a interpretação de diferenças;
- pode alterar simetria visual;
- não apaga bias de desenho;
- não deve ser escolhida apenas para produzir aparência conveniente.

F0.4 não exige matemática avançada de transformações. O objetivo é reconhecer que a escala de análise pode ser uma decisão científica/estatística relevante.

---

# 19. Worked example 1 — centro e dispersão

Dataset:

`70, 72, 74, 76, 78`

## Média

`(70+72+74+76+78)/5 = 74`

## Mediana

`74`

## Range

`78 − 70 = 8`

## Variância amostral

Desvios da média:

`-4, -2, 0, 2, 4`

Quadrados:

`16, 4, 0, 4, 16`

Soma = `40`.

`s² = 40/(5−1) = 10`

## SD

`s = √10 ≈ 3,16`

Interpretação:

- centro em torno de 74;
- valores relativamente próximos;
- SD está na mesma unidade do dado;
- variância está na unidade ao quadrado.

---

# 20. Worked example 2 — skew muda o resumo

Dataset:

`32, 33, 34, 35, 36, 38, 95`

- média ≈ `43,3`;
- mediana = `35`;
- range = `63`.

O valor 95 domina fortemente a média e o range.

Se 95 for um erro de digitação, corrigir o erro é obrigatório.

Se 95 for uma observação real, removê-la apenas para “normalizar” o resultado seria inadequado.

Uma apresentação útil poderia incluir:

- mediana + IQR;
- valores individuais/dot plot;
- justificativa sobre o valor extremo.

---

# 21. Worked example 3 — mesma média, histórias diferentes

Grupo A:

`48, 49, 50, 50, 50, 51, 52`

Média = 50; SD ≈ 1,29.

Grupo B:

`35, 35, 35, 50, 65, 65, 65`

Média = 50, mas a dispersão é muito maior e a distribuição tem estrutura completamente diferente.

Uma tabela com apenas:

`A: média 50`

`B: média 50`

apagaria informação essencial.

---

# 22. Algoritmo de descrição de um dataset

Antes de produzir uma tabela ou gráfico, use esta sequência:

1. **Qual é a unidade de observação?**
2. **Qual é o tipo da variável?**
3. **Existem limites naturais ou códigos especiais?**
4. **Como é a distribuição?**
5. **Há valores extremos e eles são plausíveis?**
6. **Qual medida de centro representa a pergunta?**
7. **Qual medida de dispersão acompanha esse centro?**
8. **Qual gráfico mostra a estrutura sem ocultar indivíduos importantes?**
9. **Estou descrevendo indivíduos ou a precisão de uma estimativa?**
10. **Se falo de uma amostra, estou confundindo sample distribution com sampling distribution?**

---

# 23. Erros comuns que você deve conseguir rejeitar

## Erro 1

> “A média é sempre a melhor medida de centro.”

Falso. Skew, extremos, escala e pergunta podem tornar mediana/quantis mais informativos.

## Erro 2

> “Outlier é dado errado.”

Falso. É um sinal para investigação.

## Erro 3

> “SE descreve quão diferentes são os participantes.”

Falso. Isso é função descritiva de medidas como SD/IQR. SE descreve sampling variability de uma estimativa.

## Erro 4

> “Se n quadruplica, o SD cai pela metade.”

Falso. Sob variabilidade individual semelhante, é o SE da média que cai aproximadamente pela metade.

## Erro 5

> “Uma barra mais alta em eixo truncado significa grande efeito.”

Falso. A magnitude deve ser lida nos valores e na escala, não na impressão visual.

## Erro 6

> “Histograma e bar chart são a mesma coisa.”

Falso. Um representa intervalos de variável numérica; o outro categorias.

## Erro 7

> “A sampling distribution é o histograma dos indivíduos da amostra.”

Falso. É a distribuição de uma estatística em amostras repetidas hipotéticas.

---

# 24. Recuperação ativa durante a aula

Sem olhar para cima, responda:

1. Qual a diferença entre variável nominal e ordinal?
2. Por que códigos numéricos de categorias não tornam a variável quantitativa?
3. Quando a mediana pode ser mais informativa que a média?
4. Qual é a diferença entre range e IQR?
5. Por que SD volta para a unidade original enquanto variância não?
6. Por que outlier não deve ser apagado automaticamente?
7. Diferencie histograma e bar chart.
8. O que um eixo truncado pode fazer com a percepção visual?
9. Diferencie população e amostra.
10. Diferencie parâmetro e estatística.
11. Diferencie sample distribution e sampling distribution.
12. O que SD descreve?
13. O que SE descreve?
14. Se `SD=12` e `n=36`, qual é aproximadamente o `SE` da média?
15. Se o SD populacional se mantém parecido e `n` passa de 25 para 100, o que tende a acontecer com o SE?
16. Por que aumentar n não elimina bias sistemático?

---

# 25. Limites desta unidade

F0.4 **não** autoriza ainda:

- interpretar um intervalo de confiança em profundidade;
- concluir com base em `p < 0,05`;
- calcular/interpretar effect size como conteúdo central;
- discutir power formalmente;
- resolver multiplicidade;
- escolher modelos inferenciais complexos.

Esses temas pertencem a F0.5–F0.6.

O objetivo aqui é mais fundamental:

> **ser capaz de ver os dados antes de tentar inferir além deles.**

---

# 26. Checklist de saída da F0.4

Você está pronto para a avaliação local quando consegue, sem consultar a aula:

- classificar variáveis comuns;
- escolher média/SD versus mediana/IQR com justificativa;
- calcular média, mediana, range, variância amostral e SD em datasets pequenos;
- explicar quantis e IQR;
- reconhecer skew e valores extremos sem regras automáticas;
- escolher gráfico adequado;
- detectar pelo menos três formas de visualização enganosa;
- diferenciar população/amostra e parâmetro/estatística;
- explicar sampling variation;
- diferenciar sample distribution de sampling distribution;
- explicar SD versus SE em linguagem própria;
- prever que quadruplicar n reduz o SE da média aproximadamente pela metade quando SD se mantém semelhante;
- explicar por que o SD individual não precisa diminuir com n;
- reconhecer transformações como mudança de escala, não como correção universal.

A validação real ocorre em `EXERCISES.md`. Produção desta aula não altera o estado de aprendizagem.