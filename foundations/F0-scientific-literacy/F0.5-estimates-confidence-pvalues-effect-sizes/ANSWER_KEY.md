# F0.5 — Gabarito comentado

Este arquivo deve ser consultado **somente depois da primeira tentativa independente** de `EXERCISES.md`.

**Total:** 100 pontos.

**Gate local:** `>=80/100` + nenhum `critical fail`.

---

# Parte A — Objetos estatísticos e linguagem correta — 15 pontos

## A1 — parâmetro, estimador e estimativa — 4 pontos

1. **Parâmetro:** a diferença média populacional alvo entre A e B, na população/estimand definidos.
2. **Estimador:** a regra `média_A − média_B` aplicada à amostra.
3. **Estimativa:** `+1,7` no dataset observado.
4. A estimativa não é automaticamente o “efeito verdadeiro” porque muda com sampling variation e pode ainda ser afetada por bias/model assumptions/desenho.

**Pontuação:** 1 ponto por item.

## A2 — point versus interval estimate — 3 pontos

- point estimate = `+1,7`;
- interval estimate = `+0,3 a +3,1`;
- o intervalo acrescenta informação sobre incerteza/precisão e mostra que múltiplos valores do parâmetro permanecem compatíveis com os dados/modelo, em vez de apresentar +1,7 como valor conhecido exatamente.

**Pontuação:** 1 por componente.

## A3 — frequentist CI — 4 pontos

Resposta-modelo:

> Um CI frequentista de 95% é produzido por um procedimento que, sob repeated sampling e assumptions válidas, cobriria o parâmetro verdadeiro fixo em aproximadamente 95% das aplicações repetidas. O 95% caracteriza o procedimento de construção, não uma probabilidade posterior de o parâmetro fixo estar dentro deste intervalo observado.

**Pontuação:**

- repeated sampling/cobertura do procedimento — 2;
- parâmetro fixo — 1;
- dependence on model/assumptions — 1.

**Critical fail:** afirmar explicitamente `P(parâmetro dentro do CI observado)=0,95` como interpretação frequentista.

## A4 — null values — 4 pontos

| Medida | Null value | Razão |
|---|---:|---|
| Mean difference | `0` | zero diferença |
| Risk difference | `0` | zero diferença absoluta |
| Risk ratio | `1` | riscos iguais |
| Odds ratio | `1` | odds iguais |

1 ponto cada.

---

# Parte B — Confidence intervals e p-values — 25 pontos

## B1 — seis princípios ASA — 12 pontos

### 1. CORRETA

P-values podem expressar incompatibilidade dos dados com um modelo estatístico especificado.

### 2. INCORRETA

`p=0,04` não é 4% de probabilidade de H0 ser verdadeira. O cálculo condiciona ao modelo/H0 para avaliar quão extremo é o resultado/test statistic.

### 3. INCORRETA

Conclusão científica não deve depender apenas de ultrapassar um threshold como 0,05; é necessário considerar desenho, magnitude, precisão, transparência e contexto.

### 4. CORRETA

Selective reporting e escolhas analíticas condicionadas aos resultados prejudicam inferência.

### 5. INCORRETA

P-value não mede magnitude; depende da combinação entre efeito, variabilidade, n e modelo/teste.

### 6. CORRETA

P-value isolado não resume toda a evidência/model assumptions.

**Pontuação:** 2 por item: 1 pela classificação + 1 por explicação/reparo correto.

**Critical fail:** itens 2, 3 ou 5 reparados de forma que ainda atribua probabilidade à hipótese ou magnitude ao p-value.

## B2 — p pequeno, efeito pequeno — 5 pontos

- **Direction:** positiva;
- **Magnitude:** `+0,20` unidade;
- **Precision:** relativamente alta/CI estreito `+0,05 a +0,35`;
- **p=0,01:** dados mostram incompatibilidade relativamente maior com o null/modelo especificado; não prova verdade/importância;
- **Practical importance:** CI inteiro está abaixo do threshold `+1,0`, portanto, sob esse threshold e assumptions, o resultado é compatível com efeito positivo pequeno, não com benefício considerado relevante.

1 ponto por item.

## B3 — dois resultados “não significativos” — 8 pontos

1. O rótulo esconde a diferença de precisão: X é extremamente impreciso; Y é estreito.
2. Y é mais informativo sobre efeitos `>=1,0`, porque o CI `−0,30 a +0,30` os exclui sob o modelo.
3. X: “a estimativa está perto de zero, mas o CI é tão amplo que efeitos relevantes em benefício e dano permanecem compatíveis; o estudo é pouco informativo para excluir magnitude relevante.”
4. Y: “a estimativa está perto de zero e o CI estreito fica dentro da zona ±1,0; sob o threshold e assumptions, efeitos de magnitude relevante estão excluídos.”

**Pontuação:** 2 por item.

**Critical fail:** “ambos provam ausência de efeito porque p=0,99”.

---

# Parte C — Effect measures — 20 pontos

## C1 — MD e SMD — 6 pontos

1. `MD = 6,0 − 4,5 = +1,5` — 1 ponto.
2. `SMD = 1,5 / 3,0 = +0,50` — 1 ponto.
3. MD: diferença na unidade original; SMD: diferença em unidades da SD usada para padronização — 2 pontos.
4. `0,50` não é universalmente “médio/importante”: relevância depende da escala original, SD, população, outcome e threshold decisório — 2 pontos.

**Critical fail:** tratar 0,50 como importância universal apenas por convenção de rótulo.

## C2 — risco, RD, RR e OR — 9 pontos

A:

`risk_A = 12/100 = 0,12 = 12%`.

B:

`risk_B = 20/100 = 0,20 = 20%`.

### RD

`RD = 0,12 − 0,20 = −0,08`.

Equivale a:

`−8 pontos percentuais`.

### RR

`RR = 0,12/0,20 = 0,60`.

### Odds

A:

`odds_A = 0,12/0,88 ≈ 0,136`.

B:

`odds_B = 0,20/0,80 = 0,25`.

### OR

`OR ≈ 0,136/0,25 ≈ 0,545 ≈ 0,55`.

### Interpretação do RR

O risco em A é 60% do risco em B; equivalentemente, a point estimate corresponde a 40% menor risco relativo em A, sem afirmar ainda causalidade ou certeza.

### RR versus OR

São medidas matematicamente diferentes. OR compara odds; RR compara riscos. Podem ser próximos quando eventos são raros, mas divergem quando eventos são mais comuns.

**Pontuação:** 1 ponto por cada um dos nove pedidos.

**Critical fail:** OR chamado de RR ou vice-versa sem reconhecer distinção.

## C3 — mesmo RR, impacto absoluto diferente — 5 pontos

Cenário 1:

`RD = 10% − 20% = −10 pontos percentuais`.

Cenário 2:

`RD = 1% − 2% = −1 ponto percentual`.

O RR é 0,50 nos dois, mas o efeito absoluto difere dez vezes.

Dizer apenas “redução de 50%” é incompleto porque esconde baseline e absolute difference.

Acompanhar com riscos absolutos em cada grupo e/ou RD.

**Pontuação:**

- RD1 — 1;
- RD2 — 1;
- explicação da diferença — 2;
- baseline/absolute reporting — 1.

**Critical fail:** interpretar os dois cenários como mesmo impacto prático apenas porque RR é igual.

---

# Parte D — Thresholds, compatibilidade e relevância prática — 20 pontos

## D1 — intervalo acima do threshold — 5 pontos

- direction: positiva/benefício;
- magnitude: point estimate +1,8;
- precision: CI +1,2 a +2,4, relativamente estreito no contexto;
- null: 0 está fora do CI;
- threshold: o CI inteiro está acima de +1,0, então sob o modelo e threshold os valores compatíveis no intervalo são todos de benefício relevante.

1 ponto cada.

Não dizer “95% de chance de benefício relevante”.

## D2 — intervalo estreito dentro da zona trivial — 5 pontos

Resposta esperada:

- point estimate próxima de zero;
- CI `−0,40 a +0,20` é estreito;
- todo o intervalo está dentro de `−1 a +1`;
- portanto, sob threshold/model assumptions, efeitos de magnitude relevante estão excluídos;
- p alto não transforma o resultado em “sem informação”; a informação vem da magnitude e precisão.

1 ponto por componente.

## D3 — intervalo largo cruza múltiplas zonas — 6 pontos

1. Permanecem compatíveis: pequena desvantagem, zero/efeito trivial, benefício acima de +1 e benefício grande — 2 pontos.
2. Errado concluir “não há efeito” apenas porque CI cruza zero — 2 pontos.
3. Errado concluir “há benefício relevante” apenas porque point estimate é +1,4; CI mostra imprecisão e inclui outras histórias — 2 pontos.

## D4 — threshold depende do contexto — 4 pontos

Aceitar qualquer quatro justificativas defensáveis, uma por ponto:

- significado da escala/outcome;
- custo;
- risco/harms;
- viabilidade;
- população;
- baseline;
- duração;
- decisão em questão;
- conhecimento prévio;
- comparação com alternativas;
- idealmente prespecificação para evitar escolha pós-resultado.

---

# Parte E — Performance task integrada — 20 pontos

## E1 — linha de forest plot — 10 pontos

Resposta-modelo:

### Target/measure

Mean difference `A−B` para outcome em que maior é melhor; null = 0.

### Direction

Point estimate `+1,40` favorece A.

### Magnitude

Diferença média estimada = `+1,40 unidade`.

### Precision/CI

`95% CI = −0,84 a +3,64`: intervalo amplo, cobrindo pequena desvantagem até benefício grande.

### Statistical output

CI inclui 0; `p≈0,22` indica que os dados não mostram forte incompatibilidade com um modelo de diferença zero. Isso não é 22% de chance de ausência nem prova de H0.

### Practical meaning + unsupported claims

Threshold relevante = +2,0. A point estimate não chega ao threshold, mas o CI inclui valores >+2 e também efeitos triviais/negativos. Logo, o estudo é impreciso para estabelecer benefício prático. Não sustenta “A não funciona”, “A tem benefício relevante comprovado” ou causalidade além do desenho.

**Pontuação:**

- Target/measure — 1;
- Direction — 1;
- Magnitude — 1;
- Precision — 2;
- Statistical output — 2;
- Practical/unsupported — 3.

## E2 — trial binário — 10 pontos

Resposta-modelo:

### Target/measure

Risk ratio A/B, complementado por riscos absolutos e RD; null do RR = 1.

### Direction

RR `0,60` aponta para menor risco em A na point estimate.

### Magnitude

A=12%, B=20%; RR=0,60; RD pontual=`−8 pp`. O risco de A é 60% do risco de B, equivalente a redução relativa pontual de 40%.

### Precision/CI

`95% CI RR ≈0,31 a 1,16` é amplo e inclui 1; portanto inclui desde redução relativa importante até pequeno aumento relativo.

### Statistical output

`p≈0,13` não mostra forte incompatibilidade com null RR=1, mas não é 13% de chance de não haver efeito e não prova ausência.

### Practical meaning + unsupported claims

A RD pontual de −8 pp ultrapassa o threshold de −5 pp, mas a incerteza do efeito relativo é ampla e inclui null; sem CI apropriado da RD e sem mais precisão não é defensável declarar benefício absoluto relevante estabelecido. O desenho/risco de bias também não foi fornecido, então causalidade não pode ser inferida apenas da tabela.

**Pontuação:** mesma distribuição 1/1/1/2/2/3.

**Critical fail:** usar `p=0,13` para provar ausência, tratar RR como OR, ou ignorar baseline absoluto.

---

# Rubrica global

## 90–100

Raciocínio quantitativo estável. Distingue inferência frequentista, magnitude, precisão e practical threshold sem dicotomizar.

## 80–89

Suficiente para o gate local se não houver critical fail. Pequenas imprecisões de linguagem podem ser remediadas localmente.

## 70–79

`TARGETED_REMEDIATION`. Mapear o erro à primeira dependência quebrada:

- CI frequentista → seções 4–5;
- p-value → seções 7–10;
- effect measure → seções 13–20;
- practical threshold → seções 21–24;
- SD/SE/sampling variation → retornar a F0.4.

## <70

Revisão ampla da F0.5 e reteste equivalente.

---

# Learner-state rule

Este gabarito registra somente o padrão de correção.

Não existe tentativa observada neste arquivo.

Portanto, sua criação **não altera** `UNSEEN`, `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` ou `MASTERED`.
