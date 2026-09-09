# F0.4 — Gabarito comentado

Este gabarito contém:

1. chave do `ENTRY_DIAGNOSTIC.md`;
2. respostas esperadas para `EXERCISES.md`;
3. critérios de correção e falhas críticas.

Não existe uma única redação obrigatória para questões abertas. O critério é preservar o conceito estatístico e justificar a escolha.

---

# Parte 0 — Gabarito do diagnóstico quantitativo de entrada

## D1 — Frações, decimais e porcentagens

### 1

`3/5 = 0,6 = 60%`.

### 2

`0,125 = 125/1000 = 1/8 = 12,5%`.

**2/2:** ambas as conversões completas.

**1/2:** uma conversão correta ou erro aritmético pequeno com procedimento correto.

**0/2:** não demonstra equivalência fração–decimal–porcentagem.

## D2 — Razões e mudança relativa

Inicial = 20; novo = 30.

### Razão

`30/20 = 1,5`.

### Aumento relativo

`(30−20)/20 = 10/20 = 0,5 = 50%`.

**Resposta:** razão `1,5`; aumento relativo `50%`.

## D3 — Porcentagem versus ponto percentual

De 20% para 25%:

- aumento absoluto = `5 pontos percentuais`;
- aumento relativo = `(25−20)/20 = 5/20 = 25%`.

Erro estrutural típico: responder “5%” para ambas.

## D4 — Álgebra de uma etapa

`3x = 24`

Dividir ambos os lados por 3:

`x = 8`.

## D5 — Notação científica

1. `0,00045 = 4,5 × 10⁻⁴`.
2. `3,2 × 10³ = 3200`.

## D6 — Tabela e relação x–y

1. Em `2 h`, medida = `12`.
2. Variações consecutivas:
   - 0→1: +2;
   - 1→2: 0;
   - 2→3: +3.

Maior aumento: `2 h → 3 h`, aumento de `3` unidades.

## D7 — Média versus mediana

Valores: `2, 3, 3, 4, 20`.

Média:

`(2+3+3+4+20)/5 = 32/5 = 6,4`.

Mediana = `3`.

Se 20 é um valor extremo real, a mediana representa melhor o centro dos quatro valores menores porque é muito menos deslocada pela magnitude do 20.

## D8 — Probabilidade

1. `0,35 = 35%`.
2. `70% = 0,70`.

---

# Roteamento do diagnóstico

Aplicar exatamente os critérios do `ENTRY_DIAGNOSTIC.md`.

### `READY_FOR_F0.4`

- 14–16/16;
- nenhum domínio zerado.

### `P1_REPAIR`

- 10–13/16; ou
- 14–16/16 com um ou dois domínios zerados;
- pelo menos seis domínios com `>=1/2`.

### `P2-QB_REQUIRED`

- `<=9/16`; ou
- três ou mais domínios zerados; ou
- menos de seis domínios com qualquer competência (`>=1/2`).

**Não aplicar nenhum rótulo sem respostas reais observadas.**

---

# Parte A — Recuperação ativa

Cada item vale 2 pontos.

## A1 — nominal versus ordinal

**Nominal:** categorias sem ordem natural.

**Ordinal:** categorias com ordem, mas sem garantia de intervalos iguais entre níveis.

## A2 — discreta versus contínua

**Discreta:** valores contáveis, frequentemente inteiros.

**Contínua:** valores em um continuum/intervalo de medição, ainda que o instrumento arredonde.

## A3 — média versus mediana

A média usa a magnitude de todos os valores no cálculo. A mediana depende principalmente da posição ordenada e por isso é menos sensível à magnitude de extremos.

## A4 — range versus IQR

`range = máximo − mínimo` e depende dos dois extremos.

`IQR = Q3 − Q1` e descreve a largura do meio de aproximadamente 50% dos dados.

## A5 — variância versus SD

Variância usa desvios ao quadrado, então fica em unidade². SD é a raiz da variância e volta à unidade original.

## A6 — right skew

Cauda mais longa para valores altos/direita. Média frequentemente é puxada para cima, mas `média > mediana` não é a definição universal.

## A7 — outlier

Valor extremo pode ser erro, valor raro real, subgrupo ou consequência legítima. Deve ser verificado, não apagado automaticamente.

## A8 — população versus amostra

**População:** conjunto-alvo sobre o qual a pergunta pretende falar.

**Amostra:** unidades efetivamente observadas.

## A9 — parâmetro versus estatística

**Parâmetro:** característica da população.

**Estatística:** quantidade calculada da amostra.

## A10 — sample versus sampling distribution

**Sample distribution:** distribuição dos valores individuais em uma amostra.

**Sampling distribution:** distribuição de uma estatística em muitas amostras hipotéticas repetidas.

---

# Parte B — Quatro datasets, quatro decisões

Cada cenário vale 5 pontos. Respostas alternativas recebem crédito se a justificativa for estatisticamente coerente.

## B1 — aproximadamente simétrico

`48, 49, 50, 50, 50, 51, 52`

- variável: numérica contínua;
- centro: média = 50 é natural;
- dispersão: SD; pode acompanhar range/quantis;
- gráfico: dot plot ou histograma simples;
- justificativa: distribuição compacta/aproximadamente simétrica e sem extremo dominante.

A mediana também é 50, mas resposta completa deve justificar por que média + SD funciona bem aqui.

## B2 — cauda longa à direita

`32, 33, 34, 35, 36, 38, 95`

- variável: numérica contínua;
- centro preferencial: mediana = 35;
- dispersão: IQR/quantis; range pode ser mostrado como informação adicional, mas é dominado pelo extremo;
- gráfico: dot plot, boxplot e/ou histograma;
- justificativa: forte right skew com valor 95 real.

Resposta inadequada: “apagar 95 porque é outlier”.

## B3 — modalidade

- variável: categórica nominal;
- centro: moda = corrida, se for necessário um resumo de categoria mais frequente;
- estrutura: contagens e proporções;
- gráfico: bar chart;
- justificativa: categorias não têm ordem quantitativa.

Não calcular média dos códigos de modalidade.

## B4 — percepção ordinal

- variável: categórica ordinal;
- centro: mediana/categoria mediana ou moda podem ser defendidas conforme objetivo;
- estrutura: contagens/proporções por nível, preservando ordem;
- gráfico: bar chart ordenado;
- justificativa: existe ordem, mas não se presume distância igual entre níveis.

Full credit não exige calcular uma mediana numérica de códigos arbitrários.

---

# Parte C — Cálculos descritivos

## C1 — dataset `70, 72, 74, 76, 78`

### Média

`(70+72+74+76+78)/5 = 370/5 = 74`.

### Mediana

`74`.

### Range

`78−70 = 8`.

### Variância amostral

Desvios em relação a 74:

`-4, -2, 0, 2, 4`.

Quadrados:

`16, 4, 0, 4, 16`.

Soma = 40.

`s² = 40/(5−1) = 10`.

### SD amostral

`s = √10 ≈ 3,16`.

**Pontuação sugerida:**

- média 2;
- mediana 1;
- range 1;
- variância com denominador correto 3;
- SD 3.

## C2 — quartis/IQR

Valores:

`2, 4, 6, 8, 10, 12, 14, 16, 18`.

Mediana = `10`.

Metade inferior, excluindo mediana:

`2, 4, 6, 8`.

`Q1 = (4+6)/2 = 5`.

Metade superior:

`12, 14, 16, 18`.

`Q3 = (14+16)/2 = 15`.

`IQR = 15−5 = 10`.

## C3 — valor extremo

Dataset A:

`10, 11, 12, 13, 14`

Média = 12; mediana = 12.

Dataset B:

`10, 11, 12, 13, 50`

Média = `96/5 = 19,2`; mediana = 12.

A média aumenta fortemente; a mediana não muda. A mediana é mais resistente à magnitude do extremo.

---

# Parte D — Auditoria de visualização

## D1 — eixo truncado

Diferença real:

`50,4 − 50,0 = 0,4`.

O eixo `49,8–50,5` amplia visualmente uma diferença pequena em relação à escala absoluta.

Resposta boa:

- manter os valores explícitos;
- mostrar eixo claramente;
- considerar dot/interval plot ou distribuição individual;
- se eixo truncado for usado para detalhes, deixar isso inequívoco e não descrever a diferença pela aparência da altura da barra.

## D2 — médias iguais, distribuições diferentes

Ambas têm média 50, mas:

- A é muito concentrado;
- B é muito disperso e possui agrupamentos nos extremos.

Barra de média apaga dispersão/forma.

Gráfico adequado:

- dot plot;
- strip plot;
- boxplot acompanhado de dados individuais;
- histograma, dependendo do contexto.

Procurar dispersão, multimodalidade/clusters, gaps e extremos.

## D3 — bar chart versus histograma

- modalidade esportiva → **bar chart**, porque é categórica nominal;
- tempo de prova → **histograma**, porque é variável numérica e queremos distribuição por intervalos.

---

# Parte E — Sampling variation, SD e SE

## E1

**SD:** dispersão dos valores individuais em torno da média e estimativa da variabilidade individual sob o modelo amostral.

**SE:** desvio-padrão da sampling distribution de uma estatística; para a média, descreve quanto médias amostrais tenderiam a variar entre amostras repetidas.

Não são sinônimos porque descrevem objetos diferentes:

- SD → indivíduos;
- SE → estimativa/estatística.

## E2

`n=25`, `SD=10`:

`SE = 10/√25 = 10/5 = 2`.

`n=100`, `SD=10`:

`SE = 10/√100 = 10/10 = 1`.

## E3

De 25 para 100, `n` quadruplica.

Como `SE ∝ 1/√n`, o SE cai aproximadamente pela metade, se SD permanecer semelhante.

O SD não precisa cair pela metade porque ele descreve dispersão individual, não precisão da média.

## E4

- distribuição dos 100 valores individuais → **sample distribution**;
- distribuição de 10.000 médias de 10.000 amostras → **sampling distribution of the mean**.

---

# Parte F — Integração

## F1 — pacote descritivo para right skew

Resposta exemplar:

- centro: mediana;
- dispersão: IQR + quantis adicionais;
- gráfico: dot plot/histograma/boxplot, idealmente mostrando valores individuais quando viável;
- extremos: verificar origem, manter se válidos, documentar qualquer exclusão/correção;
- média + SE seria inadequada para descrever indivíduos porque SE descreve precisão da média e pode esconder grande dispersão/skew individual.

Média pode ser apresentada como informação adicional se a pergunta exigir, mas não deve substituir a descrição da forma.

## F2 — amostra maior

Estudo 1: n=25, SD≈12.

Estudo 2: n=400, SD≈12.

1. SDs semelhantes sugerem dispersão individual semelhante nas amostras.
2. Estudo 2 terá menor SE da média.

Se calcular:

- E1: `SE ≈ 12/5 = 2,4`;
- E2: `SE ≈ 12/20 = 0,6`.

3. Maior n não elimina bias de seleção, mensuração, confounding ou outros mecanismos sistemáticos.
4. Range depende dos extremos observados; com mais pessoas há mais oportunidade de observar valores mais extremos, portanto o range pode aumentar mesmo com mesma distribuição populacional.

---

# Rubrica global

## 90–100

Escolhe resumos pela distribuição/pergunta, calcula corretamente, lê visualizações criticamente, distingue sample/sampling distributions e explica SD versus SE sem depender de slogans.

## 80–89

Competência suficiente. Pequenas falhas aritméticas podem ocorrer, mas a estrutura conceitual permanece correta.

## 70–79

Compreensão parcial. Requer correção dirigida antes de F0.5, especialmente se houver confusão em variabilidade, gráficos ou sampling variation.

## <70

A base descritiva ainda não está estável. Revisar e refazer forma equivalente.

---

# Falhas críticas

Mesmo com nota total alta, não considerar F0.4 aplicado se o estudante:

- usa SE como medida de dispersão individual;
- afirma que aumentar n necessariamente reduz SD;
- confunde reiteradamente indivíduos com estatísticas em sample versus sampling distribution;
- remove outlier automaticamente sem investigar validade;
- interpreta magnitude somente pela aparência de eixo truncado;
- transforma gráfico descritivo/associação em prova de causalidade.

Esses erros atingem diretamente `K4`, `K5`, `K6` e `K8` e contaminariam F0.5–F0.6.

---

# Estado de aprendizagem

A existência deste gabarito não registra desempenho.

Antes de tentativa observada:

- F0.4 diagnostic = `UNOBSERVED`;
- F0.4 learner state = `UNSEEN`.

Nenhuma atualização deve ser feita apenas porque os materiais foram produzidos.