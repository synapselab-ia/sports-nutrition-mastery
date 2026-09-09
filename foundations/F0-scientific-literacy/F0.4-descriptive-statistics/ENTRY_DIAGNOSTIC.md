# F0.4 — Diagnóstico quantitativo de entrada

**Status:** `READY — UNOBSERVED`

**Finalidade:** verificar se a numeracia básica necessária para aprender F0.4 está disponível sem criar uma falsa impressão de domínio estatístico.

**Importante:** este arquivo define o instrumento e o roteamento. Ele **não** registra que o estudante possui qualquer lacuna. O estado permanece `UNOBSERVED` até respostas reais serem produzidas e corrigidas.

## 1. Como fazer

- Faça sem calculadora na primeira tentativa, exceto se uma questão explicitamente pedir.
- Não consulte a aula F0.4, o gabarito ou uma IA durante a tentativa.
- Mostre a conta quando houver cálculo.
- Tempo sugerido: 15–20 minutos.
- Pontuação total: **16 pontos**, distribuídos em oito domínios de 2 pontos.

O diagnóstico não é uma prova de F0.4. Ele testa apenas a ponte quantitativa anterior à unidade.

---

# D1 — Frações, decimais e porcentagens — 2 pontos

1. Converta `3/5` para decimal e porcentagem.
2. Converta `0,125` para fração simplificada e porcentagem.

---

# D2 — Razões e mudança relativa — 2 pontos

Um valor aumenta de `20` para `30`.

1. Qual é a razão `novo / inicial`?
2. Qual foi o aumento relativo em porcentagem?

---

# D3 — Porcentagem versus ponto percentual — 2 pontos

A proporção de participantes que atingiu um critério passa de `20%` para `25%`.

1. Quantos **pontos percentuais** houve de aumento?
2. Qual foi o **aumento relativo percentual** em relação ao valor inicial?

---

# D4 — Álgebra de uma etapa — 2 pontos

Resolva:

`3x = 24`

Depois, em uma frase, diga qual operação você realizou para isolar `x`.

---

# D5 — Notação científica — 2 pontos

1. Escreva `0,00045` em notação científica.
2. Escreva `3,2 × 10³` em forma decimal comum.

---

# D6 — Leitura de tabela e relação x–y — 2 pontos

Considere:

| Tempo (h) | Medida |
|---:|---:|
| 0 | 10 |
| 1 | 12 |
| 2 | 12 |
| 3 | 15 |

1. Qual é a medida em `x = 2 h`?
2. Entre quais tempos consecutivos ocorreu o maior aumento da medida, e de quanto foi esse aumento?

---

# D7 — Média versus mediana — 2 pontos

Considere os valores:

`2, 3, 3, 4, 20`

1. Calcule a média.
2. Calcule a mediana e diga qual das duas medidas representa melhor o centro dos quatro valores menores quando o `20` é tratado como um valor extremo real, não como erro de digitação.

---

# D8 — Probabilidade em 0–1 e 0–100% — 2 pontos

1. Uma probabilidade de `0,35` corresponde a quantos por cento?
2. Uma probabilidade de `70%` corresponde a qual valor na escala `0–1`?

---

# 2. Regra de pontuação por domínio

Cada domínio recebe:

- `2/2` — ambas as respostas/etapas essenciais corretas;
- `1/2` — raciocínio parcialmente correto, com um erro aritmético ou uma das duas partes correta;
- `0/2` — conceito/operacão principal não demonstrado.

O gabarito comentado e os critérios específicos estão em `ANSWER_KEY.md` da F0.4. Não abra antes da primeira tentativa.

---

# 3. Roteamento quantitativo

O objetivo do roteamento é distinguir **lacunas isoladas** de uma **dependência estrutural**.

## `READY_FOR_F0.4`

Critérios:

- `14–16/16`; e
- nenhum domínio com `0/2`.

Interpretação: a ponte quantitativa está suficientemente estável para a F0.4. Pequenos erros ocasionais podem ser corrigidos dentro da aula.

## `P1_REPAIR`

Critérios típicos:

- `10–13/16`; **ou**
- `14–16/16` com um ou dois domínios zerados;
- pelo menos seis dos oito domínios demonstram alguma competência (`>=1/2`).

Interpretação: existem lacunas localizadas. Elas devem ser reparadas com microexplicação e novo item equivalente antes ou durante a F0.4. Um `P1_REPAIR` não significa fracasso geral em matemática.

## `P2-QB_REQUIRED`

Promover a ponte quantitativa para pré-requisito estrutural quando ocorrer qualquer um destes padrões:

- `<=9/16`; ou
- três ou mais domínios com `0/2`; ou
- menos de seis dos oito domínios demonstram qualquer competência (`>=1/2`).

Interpretação: a maioria das operações necessárias não está suficientemente estável para que erros aritméticos sejam tratados como detalhes locais. Antes da validação de F0.4, completar um `P2-QB` focado nos domínios quebrados e repetir uma forma equivalente do diagnóstico.

### Regra de segurança

Não inferir `P1_REPAIR` nem `P2-QB_REQUIRED` pela impressão de dificuldade, histórico escolar ou autodeclaração. O roteamento exige **respostas observadas**.

---

# 4. O que este diagnóstico não testa

Ele não testa:

- variância ou desvio-padrão;
- distribuição amostral;
- erro-padrão;
- intervalo de confiança;
- p-value;
- power;
- regressão;
- cálculo diferencial/integral.

Esses conteúdos não devem ser usados para transformar o diagnóstico de entrada em uma prova escondida de estatística.

---

# 5. Registro de estado

Antes de respostas reais:

`F0.4 quantitative diagnostic = UNOBSERVED`

Depois de uma tentativa corrigida, o resultado pode ser registrado como:

- `READY_FOR_F0.4`;
- `P1_REPAIR` com domínios específicos;
- `P2-QB_REQUIRED` com domínios específicos.

O diagnóstico, sozinho, não altera F0.1–F0.3 e não autoriza `MASTERED` em nenhuma competência.