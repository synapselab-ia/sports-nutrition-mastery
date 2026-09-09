# F0.4 — Exercícios de recuperação ativa e aplicação

**Use depois de estudar `LESSON.md` e somente após resolver o `ENTRY_DIAGNOSTIC.md` quando ele for aplicado.**

Não consulte `ANSWER_KEY.md` na primeira tentativa.

## Estrutura e pontuação

- Parte A — recuperação ativa: 20 pontos
- Parte B — escolha de resumos para quatro datasets: 20 pontos
- Parte C — cálculos descritivos: 20 pontos
- Parte D — auditoria de visualização: 15 pontos
- Parte E — sampling variation, SD e SE: 15 pontos
- Parte F — integração: 10 pontos

**Total:** 100 pontos.

### Gate local de competência

- `>=80/100`: desempenho suficiente para seguir, desde que nenhuma falha crítica ocorra;
- `70–79`: corrigir as partes frágeis e refazer itens equivalentes;
- `<70`: revisar F0.4 e repetir avaliação equivalente.

### Falhas críticas, independentemente da nota

- afirmar que `SE` descreve a dispersão dos indivíduos como se fosse `SD`;
- afirmar que aumentar `n`, por si só, torna os indivíduos menos variáveis e necessariamente reduz o `SD`;
- confundir sample distribution com sampling distribution mesmo após o cenário explicitar que uma é composta por indivíduos e a outra por estatísticas de amostras repetidas;
- apagar outlier automaticamente apenas porque é extremo, sem verificar origem/contexto;
- interpretar magnitude de diferença apenas pelo tamanho visual de barras em eixo truncado, ignorando os valores/escala;
- tratar descrição gráfica/associação como prova de causalidade.

Produção deste material não altera estado de aprendizagem. Somente desempenho observado e corrigido pode sustentar progressão.

---

# Parte A — Recuperação ativa — 20 pontos

Cada item vale 2 pontos.

1. Diferencie variável categórica nominal de categórica ordinal.
2. Diferencie variável numérica discreta de contínua.
3. O que a média usa que a mediana não usa da mesma forma?
4. Diferencie range de IQR.
5. Por que a variância e o SD têm unidades diferentes?
6. O que significa right skew em linguagem visual?
7. Por que um outlier não deve ser tratado automaticamente como erro?
8. Diferencie população de amostra.
9. Diferencie parâmetro de estatística.
10. Diferencie sample distribution de sampling distribution.

---

# Parte B — Quatro datasets, quatro decisões — 20 pontos

Para cada cenário, indique:

1. tipo principal da variável;
2. resumo de centro mais apropriado entre média, mediana ou moda;
3. medida de dispersão/estrutura que deve acompanhar o centro;
4. um gráfico apropriado;
5. justificativa curta.

Cada cenário vale 5 pontos.

## B1 — valores aproximadamente simétricos

Altura de salto hipotética (cm):

`48, 49, 50, 50, 50, 51, 52`

## B2 — cauda longa à direita

Tempo hipotético para completar uma tarefa (min):

`32, 33, 34, 35, 36, 38, 95`

O valor `95` foi verificado e é real.

## B3 — categorias sem ordem

Modalidade principal de 40 participantes:

- corrida: 18
- ciclismo: 14
- natação: 8

## B4 — escala ordinal

Resposta de percepção categórica:

- baixa: 3
- moderada: 8
- alta: 12
- muito alta: 7

---

# Parte C — Cálculos descritivos — 20 pontos

## C1 — média, mediana, range, variância e SD — 10 pontos

Considere:

`70, 72, 74, 76, 78`

Calcule:

1. média;
2. mediana;
3. range;
4. variância **amostral** usando denominador `n−1`;
5. SD amostral.

Mostre as etapas principais.

## C2 — quartis e IQR — 6 pontos

Considere os valores ordenados:

`2, 4, 6, 8, 10, 12, 14, 16, 18`

Para este exercício, use a convenção:

- mediana = valor central;
- exclua a mediana ao formar metade inferior/superior;
- `Q1` = mediana da metade inferior;
- `Q3` = mediana da metade superior.

Calcule:

1. mediana;
2. Q1;
3. Q3;
4. IQR.

## C3 — média versus mediana sob valor extremo — 4 pontos

Compare:

Dataset A: `10, 11, 12, 13, 14`

Dataset B: `10, 11, 12, 13, 50`

Sem calcular SD:

1. diga o que acontece com média e mediana quando `14` é substituído por `50`;
2. explique qual das duas medidas é mais resistente a esse valor extremo.

---

# Parte D — Auditoria de visualização — 15 pontos

Cada item vale 5 pontos.

## D1 — eixo truncado

Um gráfico compara duas médias:

- grupo A = `50,0`;
- grupo B = `50,4`.

O eixo y começa em `49,8` e termina em `50,5`, fazendo a barra B parecer várias vezes maior.

1. Qual é a diferença numérica real?
2. O que há de potencialmente enganoso na apresentação?
3. Como você reportaria/visualizaria de forma mais informativa?

## D2 — barras escondendo distribuição

Dois grupos têm média 50. O artigo mostra apenas duas barras de mesma altura.

Depois você recebe os dados:

- A: `48, 49, 50, 50, 50, 51, 52`
- B: `35, 35, 35, 50, 65, 65, 65`

Explique:

1. por que as barras de média escondem informação;
2. qual gráfico adicional você usaria;
3. qual característica você procuraria nele.

## D3 — bar chart versus histograma

Um pesquisador tem:

- modalidade esportiva (corrida/ciclismo/natação);
- tempo de prova em minutos.

Escolha entre bar chart e histograma para cada variável e explique por quê.

---

# Parte E — Sampling variation, SD e SE — 15 pontos

## E1 — SD versus SE — 5 pontos

Explique em linguagem própria:

1. o que `SD` descreve;
2. o que `SE` descreve;
3. por que não devem ser usados como sinônimos.

## E2 — cálculo de SE — 4 pontos

Uma amostra tem:

- `n = 25`;
- `SD = 10`.

Use:

`SE = SD/√n`

Calcule o SE da média.

Depois, mantendo `SD = 10`, calcule o SE se `n = 100`.

## E3 — quadruplicar n — 3 pontos

Suponha que a variabilidade individual permaneça aproximadamente a mesma.

Se `n` passa de `25` para `100`:

1. o que tende a acontecer com o SE da média?
2. o SD precisa cair pela metade? Justifique.

## E4 — duas distribuições diferentes — 3 pontos

Diferencie:

- a distribuição dos 100 valores individuais observados em uma amostra;
- a distribuição de 10.000 médias obtidas de 10.000 amostras hipotéticas de tamanho 100.

Nomeie cada uma.

---

# Parte F — Integração — 10 pontos

## F1 — escolha completa de descrição — 5 pontos

Um estudo registra uma variável numérica positiva com forte right skew e alguns valores altos reais. O objetivo é descrever a amostra, não fazer inferência causal.

Proponha um pacote descritivo contendo:

- medida de centro;
- medida de dispersão;
- pelo menos um gráfico;
- tratamento dos valores extremos;
- uma frase explicando por que somente média + SE seria uma descrição ruim dos indivíduos.

## F2 — o que muda com amostra maior — 5 pontos

Dois estudos são amostras independentes da mesma população e medem a mesma variável com procedimento semelhante.

- Estudo 1: `n=25`, SD aproximadamente 12.
- Estudo 2: `n=400`, SD aproximadamente 12.

Sem usar confidence interval ou p-value, explique:

1. o que a semelhança dos SDs sugere sobre a dispersão individual;
2. qual estudo terá menor SE da média;
3. por que isso não prova que o estudo maior é livre de bias;
4. por que o range do estudo maior pode até ser maior, mesmo sem aumento da variabilidade populacional.

---

# Autoauditoria antes do gabarito

Antes de abrir `ANSWER_KEY.md`, confira se você:

- escolheu o resumo pela estrutura dos dados, não por hábito;
- não chamou todo valor extremo de erro;
- separou média/mediana de dispersão;
- separou SD de SE;
- separou sample distribution de sampling distribution;
- não concluiu que mais participantes tornam os indivíduos menos variáveis;
- leu valores e escalas em vez de confiar na aparência de barras;
- escolheu gráfico compatível com o tipo da variável;
- não importou p-values, confidence intervals ou power para resolver uma questão que é descritiva.