# F0.5 — Exercícios de recuperação ativa e aplicação

**Total:** 100 pontos

**Condição de progressão local:** `>=80/100` **e nenhum critical fail**.

Este instrumento testa interpretação quantitativa, não reconhecimento de palavras. Responda sem consultar `ANSWER_KEY.md` na primeira tentativa.

## Critical fail — bloqueia progressão independentemente da pontuação

Qualquer um dos erros abaixo bloqueia o gate local até correção e reteste equivalente:

1. afirmar que `p < 0,05` prova que a hipótese nula é falsa ou que um efeito “é verdadeiro”;
2. afirmar que `p > 0,05` prova ausência de efeito;
3. interpretar `p = x` como probabilidade de H0 ser verdadeira ou como probabilidade de “o acaso ter produzido o resultado”;
4. interpretar um CI frequentista de 95% como “95% de probabilidade posterior de o parâmetro fixo estar dentro do intervalo”;
5. tratar “CI cruza o null” como sinônimo de inutilidade/ausência de efeito sem discutir magnitude e precisão;
6. tratar “CI não cruza o null” como prova de importância prática;
7. interpretar uma medida relativa sem procurar/considerar baseline absoluto quando ele é necessário para significado prático;
8. tratar SMD/Cohen-like labels como medida universal de importância clínica/esportiva;
9. tratar OR como RR sem reconhecer que são medidas diferentes;
10. afirmar que maior precisão ou p menor corrige systematic bias/confounding/selection/measurement problems.

---

# Parte A — Objetos estatísticos e linguagem correta — 15 pontos

## A1 — parâmetro, estimador e estimativa — 4 pontos

Um estudo quer estimar a diferença média populacional de uma mudança entre estratégias A e B. A regra de análise é `média_A − média_B`. No dataset observado, o resultado é `+1,7`.

Identifique:

1. o parâmetro;
2. o estimador;
3. a estimativa;
4. por que a estimativa não deve ser chamada automaticamente de “o efeito verdadeiro”.

## A2 — point versus interval estimate — 3 pontos

Resultado:

`MD = +1,7; 95% CI = +0,3 a +3,1`.

Explique:

1. qual é a point estimate;
2. qual é a interval estimate;
3. que informação o intervalo acrescenta que o ponto sozinho não mostra.

## A3 — frequentist CI — 4 pontos

Repare a frase abaixo para uma interpretação frequentista defensável:

> “Existe 95% de probabilidade de o verdadeiro efeito estar entre 0,3 e 3,1.”

Sua resposta deve mencionar:

- repeated sampling/procedimento;
- parâmetro fixo;
- assumptions/modelo.

## A4 — null values — 4 pontos

Preencha e justifique:

| Medida | Null value |
|---|---:|
| Mean difference | ? |
| Risk difference | ? |
| Risk ratio | ? |
| Odds ratio | ? |

---

# Parte B — Confidence intervals e p-values — 25 pontos

## B1 — seis princípios ASA — 12 pontos

Para cada afirmação, marque `CORRETA` ou `INCORRETA` e repare as incorretas em uma frase.

1. “P-values podem indicar incompatibilidade dos dados com um modelo estatístico especificado.”
2. “p=0,04 significa 4% de probabilidade de H0 ser verdadeira.”
3. “A decisão científica pode ser reduzida a p<0,05 versus p>=0,05.”
4. “Inferência adequada depende também de transparência e de como análises/resultados foram selecionados.”
5. “Um p-value menor indica necessariamente um efeito maior.”
6. “Um p-value isolado não resume adequadamente toda a evidência sobre uma hipótese/modelo.”

## B2 — p pequeno, efeito pequeno — 5 pontos

Threshold de benefício relevante: `+1,0 unidade`.

Resultado:

- estimate = `+0,20`;
- 95% CI = `+0,05 a +0,35`;
- p = `0,01`.

Responda:

1. direção;
2. magnitude;
3. precisão;
4. o que p=0,01 permite dizer;
5. importância prática sob o threshold definido.

## B3 — dois resultados “não significativos” — 8 pontos

Threshold de relevância: `±1,0 unidade`.

**Estudo X:** `estimate = 0,0; 95% CI = −5,0 a +5,0; p=0,99`.

**Estudo Y:** `estimate = 0,0; 95% CI = −0,30 a +0,30; p=0,99`.

1. Por que o rótulo “não significativo” perde a diferença mais importante entre X e Y?
2. Qual estudo é mais informativo sobre efeitos de magnitude `>=1,0`?
3. Escreva uma conclusão correta para X.
4. Escreva uma conclusão correta para Y.

---

# Parte C — Effect measures — 20 pontos

## C1 — mean difference e standardized mean difference — 6 pontos

Outcome contínuo; maior é melhor.

- média A = `6,0`;
- média B = `4,5`;
- SD usada na padronização = `3,0`.

1. Calcule `MD = A − B`.
2. Calcule `SMD = MD / SD`.
3. Explique o significado de cada medida.
4. Por que `SMD = 0,50` não autoriza automaticamente o rótulo “efeito médio e importante”?

## C2 — risco, RD, RR e OR — 9 pontos

Evento sintético:

- A: `12/100`;
- B: `20/100`.

Calcule:

1. risk_A;
2. risk_B;
3. `RD = risk_A − risk_B` em proporção e pontos percentuais;
4. `RR = risk_A / risk_B`;
5. odds_A;
6. odds_B;
7. OR;
8. interprete RR em linguagem clara;
9. explique por que OR e RR não devem ser tratados como a mesma coisa.

## C3 — mesmo RR, impacto absoluto diferente — 5 pontos

Dois cenários têm `RR = 0,50`.

**Cenário 1:** B = 20%, A = 10%.

**Cenário 2:** B = 2%, A = 1%.

1. Calcule RD em pontos percentuais nos dois cenários.
2. Explique por que dizer apenas “redução de 50%” é incompleto.
3. Qual informação de baseline deve acompanhar a medida relativa?

---

# Parte D — Thresholds, compatibilidade e relevância prática — 20 pontos

Para D1–D3, considere:

- benefício relevante: `>= +1,0`;
- zona trivial: `−1,0 a +1,0`;
- dano relevante: `<= −1,0`.

## D1 — intervalo inteiramente acima do threshold — 5 pontos

`estimate = +1,8; 95% CI = +1,2 a +2,4`.

Interprete:

- direction;
- magnitude;
- precision;
- relação com o null;
- relação com o threshold de benefício.

Não use linguagem de probabilidade posterior.

## D2 — intervalo estreito dentro da zona trivial — 5 pontos

`estimate = −0,10; 95% CI = −0,40 a +0,20`.

Explique por que este resultado pode ser informativo mesmo que um teste contra zero produza p alto.

## D3 — intervalo largo cruza múltiplas zonas — 6 pontos

`estimate = +1,4; 95% CI = −0,84 a +3,64`.

1. Quais tipos de efeito permanecem compatíveis com os dados/modelo?
2. O que seria errado concluir a partir de “CI cruza zero”?
3. O que seria errado concluir apenas pela point estimate `+1,4`?

## D4 — threshold não é propriedade automática do dado — 4 pontos

Explique quatro razões pelas quais o smallest effect of interest/decision threshold deve ser justificado pelo contexto e não escolhido automaticamente depois de olhar o resultado.

---

# Parte E — Performance task integrada — 20 pontos

Em cada item, use obrigatoriamente os seis blocos:

1. `Target/measure:`
2. `Direction:`
3. `Magnitude:`
4. `Precision/CI:`
5. `Statistical output:`
6. `Practical meaning + unsupported claims:`

## E1 — linha de forest plot — 10 pontos

Imagine a seguinte linha de um forest plot para um outcome em que **maior é melhor**:

```text
                 favorece B          null          favorece A
--------------------|-----------------0-----------------|--------------------
                                      ●──────────────
                                  -0,84      +1,40         +3,64
```

Dados numéricos canônicos da linha:

- measure = mean difference `A − B`;
- point estimate = `+1,40`;
- 95% CI = `−0,84 a +3,64`;
- p ≈ `0,22`;
- threshold de benefício relevante = `+2,0` unidades.

Produza os seis blocos obrigatórios.

Sua conclusão deve distinguir:

- direção observada;
- magnitude;
- imprecisão;
- null/statistical output;
- efeitos triviais versus relevantes;
- o que não pode ser declarado.

## E2 — pequena tabela de trial sintético — 10 pontos

Evento binário; **menor risco é melhor**.

| Grupo | Eventos | Total | Risk |
|---|---:|---:|---:|
| A | 12 | 100 | 12% |
| B | 20 | 100 | 20% |

Resultado fornecido:

- `RR = 0,60`;
- `95% CI do RR ≈ 0,31 a 1,16`;
- `p ≈ 0,13`;
- `RD pontual = −8 pontos percentuais`;
- threshold prático: redução absoluta de pelo menos `5 pontos percentuais` seria relevante.

Produza os seis blocos obrigatórios.

Sua resposta deve:

- interpretar `RR=0,60` sem chamá-lo de OR;
- usar o baseline absoluto;
- reconhecer que o CI do RR inclui 1;
- não converter p=0,13 em probabilidade de ausência;
- discutir que a point estimate absoluta ultrapassa o threshold, mas a incerteza impede concluir benefício relevante com segurança apenas desse resultado;
- separar resultado estatístico de validade causal/desenho, que não está especificado completamente aqui.

---

# Regra de correção

## `>=90/100`

Interpretação quantitativa estável; linguagem de incerteza e practical threshold bem integrada.

## `80–89/100`

Suficiente para o gate local se não houver critical fail.

## `70–79/100`

`TARGETED_REMEDIATION`: revisar os primeiros conceitos quebrados e fazer reteste equivalente.

## `<70/100`

Revisão mais ampla de F0.5; se erros incluírem SD/SE ou sampling distribution, retornar antes a F0.4.

**Produção desta avaliação não altera learner state. Somente respostas reais corrigidas podem produzir evidência de progressão.**
