# F0.10 — Síntese e comunicação da incerteza

**Production state:** `APPROVED`

**Prerequisites P2:** F0.5 — estimativas, intervalos, effect sizes e relevância prática; F0.7 — síntese, heterogeneidade e missing evidence; F0.8 — risk of bias, certeza e aplicabilidade; F0.9 — leitura crítica de paper completo.

**P0 ensinados localmente:** calibrated language, claim scope, epistemic content, invariant core, evidence statement, recommendation statement, audience translation, language drift, decision threshold, conclusion-changing evidence.

**P1 ensinados localmente:** transformar uma mesma síntese em versões técnica, practitioner-facing e lay-facing sem alterar direção, magnitude, incerteza, certeza, aplicabilidade ou limites de inferência.

**Core/method sources:** `F0-S08`, `F0-S09`, `F0-S18`, `F0-S19`, `F0-S20`, além das unidades canônicas F0.5/F0.7/F0.8/F0.9.

## 1. Competência-alvo

Ao terminar esta unidade, você deve conseguir receber um resultado ou evidence body já criticamente reconstruído e comunicá-lo para públicos diferentes sem:

1. transformar p-value em verdade binária;
2. esconder magnitude ou intervalo;
3. apagar limiar de importância prática;
4. converter `low certainty` em “não funciona”;
5. converter `high certainty` em “efeito grande/importante”;
6. dar o mesmo peso retórico a evidências de força muito diferente só para parecer equilibrado;
7. confundir directness com ausência de bias;
8. confundir certeza da evidência com força de recomendação;
9. ampliar população, outcome, duração ou contexto além do suportado;
10. tornar a versão leiga mais certa que a técnica.

Regra central:

> **Simplificar linguagem pode reduzir complexidade verbal; não pode reduzir a incerteza científica.**

F0.10 converte julgamento de evidência em comunicação calibrada sem perda epistemológica.

---

## 2. Invariant core: o que deve sobreviver à tradução

Antes de escrever para qualquer público, congele oito campos:

1. **Target** — população, intervenção/exposição, comparator, outcome, tempo e contexto;
2. **Direction** — para onde a estimate aponta;
3. **Magnitude** — tamanho do efeito na escala relevante;
4. **Precision** — CI/range/uncertainty;
5. **Threshold** — magnitude que seria importante ou mudaria decisão;
6. **Certainty** — confiança no body/outcome inference;
7. **Applicability** — alinhamento ao target real;
8. **Boundaries** — o que não foi estabelecido e o que mudaria a conclusão.

Isso é o **invariant core**.

Você pode mudar vocabulário, extensão, ordem e densidade técnica. Não pode mudar silenciosamente:

- `may` → `does`;
- `small possible benefit` → `works`;
- `did not detect` → `has no effect`;
- `moderate certainty` → `proven`;
- `trained adults` → `everyone`;
- `12 weeks` → `long term`;
- `one outcome` → `overall performance/health`.

Fluxo canônico:

`reconstructed evidence → invariant core → calibrated claim → audience translation → drift audit`.

Se F0.9 ainda não resolveu qual estimand/result está em jogo, palavras melhores não resolvem o problema.

---

## 3. Linguagem calibrada

A força verbal acompanha a força do que foi reconstruído.

### Observational/descriptive

Use construções como:

- `was associated with`;
- `was higher/lower in`;
- `co-occurred with`.

Não transforme automaticamente em `caused`, `improved` ou `prevented`.

### Resultado experimental com incerteza material

Formulações úteis:

- `the estimate favored X, but the interval was compatible with...`;
- `the trial did not detect a clear between-group difference`;
- `a small benefit remains plausible`;
- `the data are compatible with effects ranging from...`.

### Body-level certainty

Quando coerente com a framework usada:

- moderate certainty → `probably`, `moderate-certainty evidence suggests...`;
- low certainty → `may`, `the evidence is uncertain about...`.

Não existe dicionário universal de verbos. Existe a exigência de que claim strength e evidence strength não entrem em conflito.

---

## 4. O p-value não controla a frase

`F0-S08` e `F0-S09` continuam válidos:

- `p<0.05` não significa “verdadeiro”;
- `p<0.05` não significa “importante”;
- `p>0.05` não significa “sem efeito”.

Comunique:

`estimate → interval → threshold → design/bias → certainty/context`.

O p-value pode ser uma saída estatística; não substitui magnitude, precisão ou contexto.

---

## 5. Três claims diferentes: não detectado, não importante e equivalente

### 5.1 Did not detect

Resultado:

`MD = -8 s [95% CI -45,+29]`.

O intervalo inclui benefício e pouca diferença/efeito oposto.

Defensável:

> O estudo não detectou uma diferença clara; benefício e pouca ou nenhuma diferença permanecem compatíveis com os dados.

### 5.2 Evidence compatible with no important effect

Threshold de benefício importante = `-30 s`.

Resultado:

`MD = -4 s [95% CI -18,+10]`.

O CI exclui um benefício de 30 s ou maior na direção favorável.

Defensável:

> Sob esse threshold, os dados são compatíveis com ausência de benefício grande/importante; efeitos pequenos ainda permanecem possíveis.

Isso é mais informativo que dizer apenas `p>0.05`.

### 5.3 Formal equivalence

Formal equivalence/non-inferiority exige desenho/análise e margem apropriados, idealmente prespecified.

`nonsignificant superiority test ≠ equivalence trial`.

---

## 6. Estimate + CI + threshold devem viajar juntos

Exemplo:

`MD = -22 s [95% CI -51,+7]`, threshold importante `-30 s`.

Dizer apenas “efeito médio de 22 s” apaga precisão. Dizer apenas “não significativo” apaga magnitude e as possibilidades ainda compatíveis.

Síntese adequada:

> A estimate favoreceu a intervenção em 22 s, mas o IC95% vai de 51 s de benefício a 7 s de piora; portanto, tanto um benefício acima do threshold de 30 s quanto pouca diferença permanecem compatíveis com os dados.

Essa é a continuidade direta de F0.5.

---

## 7. Certainty não é magnitude

GRADE separa:

1. qual efeito/faixa parece existir;
2. quanta confiança temos de que o efeito verdadeiro está nessa faixa ou lado de um threshold.

Logo:

- `high certainty + trivial effect` é possível;
- `low certainty + large point estimate` é possível;
- low certainty não significa no effect;
- high certainty não significa large/important effect.

Exemplo:

`+0.15 [0.12,0.18]`, threshold `+1.0`, high certainty.

A conclusão correta é alta confiança de que o efeito é pequeno/trivial em relação ao threshold, não “efeito importante”.

---

## 8. Incerteza tem mecanismos diferentes

### Imprecision

CI amplo, poucos eventos/information size, crossing de thresholds relevantes.

> “A magnitude permanece incerta porque a faixa compatível é ampla.”

### Risk of bias

Processos de desenho/condução/análise podem deslocar sistematicamente a estimate.

> “Mesmo uma estimate precisa pode estar sistematicamente distorcida por...”

### Inconsistency

Estudos diretos estimam efeitos materialmente diferentes sem explicação suficiente.

> “A variação entre estudos reduz confiança em uma única magnitude média.”

### Indirectness

Evidence PICO/context difere do target.

> “A evidência é menos direta para atletas altamente treinados porque...”

### Missing/dissemination evidence

Estudos/resultados podem estar ausentes de forma relacionada ao achado.

> “A confiança é limitada pela possibilidade de evidência não observada ou seletivamente reportada.”

Não colapse todos esses mecanismos em “mais estudos são necessários”.

---

## 9. Direct evidence ≠ unbiased evidence

Um estudo pode corresponder perfeitamente a population/intervention/comparator/outcome/time e ainda ter:

- differential attrition;
- unblinded subjective measurement;
- selective analysis.

Ele pode ser **direct but biased**.

O inverso também é possível: internal validity forte e applicability estreita.

`internal validity / RoB ≠ directness / applicability`.

---

## 10. Conflito entre estudos: não conte papers

Se há:

- uma meta-analysis de RCTs diretos;
- um grande RCT recente;
- um observational cohort;
- um acute mechanistic study;

não conclua “2 contra 2”.

Pondere:

1. fit à pergunta;
2. design e bias;
3. estimand/outcome compatibility;
4. magnitude e precisão;
5. directness/applicability;
6. synthesis context;
7. body-level certainty;
8. atualidade quando material.

**False balance** ocorre quando fontes de capacidade inferencial muito desigual recebem peso retórico equivalente só porque discordam.

Evitar false balance também não significa aplicar evidence pyramid mecanicamente. A pergunta permanece:

> **Qual fonte é mais informativa para qual claim?**

Um mechanistic experiment pode ser excelente para mecanismo e insuficiente para performance crônica. Um RCT high-risk pode ser menos informativo para determinado claim que outra evidência cuidadosamente desenhada.

---

## 11. Síntese de conflito em quatro passos

Use:

`claim → source fit → weighted evidence → residual uncertainty`.

### 1. Claim

Defina exatamente população, contraste, outcome e tempo.

### 2. Source fit

Pergunte para cada fonte:

- mesma população?
- mesma intervention/comparator?
- mesmo outcome?
- mesmo time horizon?
- design adequado ao claim?

### 3. Weighted evidence

Considere:

- precision/relevance;
- RoB;
- heterogeneity;
- compatibility;
- directness.

### 4. Residual uncertainty

Uma frase útil pode ser:

> A evidência mais direta e forte concentra-se perto de efeitos pequenos, enquanto os maiores efeitos aparecem em estudos menos precisos ou menos diretamente aplicáveis; benefícios grandes são menos sustentados, embora alguma incerteza permaneça.

---

## 12. Evidence statement ≠ recommendation

**Evidence statement:** o que a evidência indica sobre um outcome específico?

**Recommendation statement:** o que alguém deveria fazer?

Recomendação pode exigir ainda:

- benefits e harms múltiplos;
- valores/preferências;
- custo/recursos;
- feasibility;
- acceptability;
- equity;
- contexto decisório.

`certainty of one outcome ≠ recommendation strength`.

Alta certeza de um efeito pequeno não cria automaticamente recomendação forte.

---

## 13. Tradução por audiência sem drift

### Technical

Pode incluir effect measure, point estimate, CI, threshold, RoB/certainty language, directness, limitations e target exato.

### Practitioner-facing

Reduza jargão, mas preserve:

- quem foi estudado;
- tamanho provável do efeito;
- amplitude da incerteza;
- grau de confiança;
- applicability;
- o que não foi estabelecido.

### Lay-facing

Pode traduzir CI como faixa de efeitos compatíveis e certainty como grau de confiança em linguagem comum.

Mas não pode converter:

> “A evidência sugere benefício pequeno, com certeza moderada.”

em:

> “Funciona.”

Nem:

> “Não detectamos benefício claro.”

em:

> “Não funciona.”

---

## 14. Drift audit

Depois de produzir várias versões, compare-as:

1. a população ficou mais ampla?
2. direção mudou?
3. magnitude desapareceu?
4. interval virou certeza?
5. threshold sumiu?
6. `may/probably` virou verbo categórico?
7. bias foi apagado?
8. applicability foi generalizada?
9. evidence statement virou recommendation?
10. versão simplificada parece mais confiante que a técnica?

Se sim, houve **language drift**.

---

## 15. O que mudaria a conclusão?

Toda boa síntese explicita update conditions.

Exemplos:

- RCT direto grande com CI estreito inteiramente além do threshold;
- body direto com CI estreito excluindo o threshold;
- reanalysis que resolve missingness material;
- novos estudos na população-alvo que reduzem indirectness;
- credible missing-evidence signal que altera o body;
- mudança defensável do threshold;
- harms relevantes que alteram recommendation mesmo sem mudar efficacy.

“Mais estudos são necessários” é insuficiente sem dizer **qual resultado** mudaria a conclusão e em que direção.

---

## 16. Worked example A — não detectado ≠ inexistente

- target: trained adults;
- outcome: performance time, lower better;
- `MD = -12 s`;
- `95% CI = -44 a +20 s`;
- practical-benefit threshold = `-30 s`;
- low RoB;
- direct evidence;
- body certainty: moderate, limitada principalmente por imprecision.

### Technical

> A estimate favorece a intervenção em 12 s, mas o IC95% de -44 a +20 s cruza tanto o null quanto o limiar de benefício importante de -30 s. Os dados não demonstram benefício claro nem excluem benefício material; a incerteza é principalmente de precisão.

### Practitioner-facing

> O melhor palpite é uma melhora pequena, mas os dados ainda permitem tanto uma melhora relevante quanto quase nenhuma diferença. Não é correto concluir nem que “funciona claramente” nem que “não funciona”.

### Lay-facing

> O resultado apontou para uma pequena melhora, mas a margem de incerteza ainda é grande: o efeito real pode ser relevante ou praticamente nulo. Ainda não há base para uma conclusão definitiva.

O invariant core permanece o mesmo.

---

## 17. Worked example B — high certainty, trivial effect

- pooled effect `+0.15`;
- 95% CI `+0.12 a +0.18`;
- threshold importante `+1.0`;
- high certainty.

Adequado:

> Há alta confiança de que o efeito é pequeno/trivial em relação ao threshold definido.

Inadequado:

> Há alta certeza, então o efeito é importante.

---

## 18. Worked example C — conflito sem falsa equivalência

Claim: Intervention Q melhora um performance score crônico.

Evidence:

- systematic review de RCTs diretos: `+0.4 [0.0,+0.8]`;
- grande RCT novo: `+0.2 [-0.1,+0.5]`;
- cohort observacional: `+1.8 [+1.3,+2.3]`, com self-selection/residual confounding;
- acute mechanistic experiment: biomarker +35%, sem performance endpoint;
- threshold importante `+1.0`.

Ruim:

> “A literatura está dividida: dois positivos e dois inconclusivos.”

Melhor:

> As fontes mais diretas para performance crônica estimam efeitos pequenos e abaixo do threshold de +1.0; o maior efeito vem de evidência observacional mais vulnerável a confounding, e o mechanistic study apoia plausibilidade, não magnitude de performance. O peso do conjunto favorece, no máximo, efeito pequeno; benefícios grandes estão menos sustentados.

---

## 19. Template canônico F0.10

Antes de qualquer audiência, preencha:

### A. Target
`Population / intervention-exposure / comparator / outcome / time / setting-context`

### B. Direction and magnitude
`effect measure + point estimate`

### C. Precision
`CI/range + material possibilities remaining`

### D. Practical threshold
`threshold + whether uncertainty crosses it`

### E. Main uncertainty source(s)
`bias / imprecision / inconsistency / indirectness / missing evidence`

### F. Certainty
`body/outcome certainty + rationale`

### G. Applicability
`where it transports / where it becomes indirect`

### H. Evidence statement
`one calibrated sentence`

### I. Recommendation boundary
`what the evidence statement does not decide`

### J. Update conditions
`what would materially change the conclusion`

Só depois produza versões por audiência.

---

## 20. Performance-package rule

A avaliação usa um único pacote sintético para obrigar três comunicações:

1. technical;
2. practitioner-facing;
3. lay-facing.

A correção não premia “tom bonito”. Verifica se as três versões conservam o mesmo invariant core.

O pacote inclui fontes com pesos inferenciais diferentes de propósito. Contar papers em vez de ponderá-los é erro estrutural.

---

## 21. Critical fails

Falha estrutural se a resposta:

1. usa `p<0.05` como verdade/importância;
2. usa `p>0.05` como ausência/equivalência;
3. omite CI/threshold material para simplificar;
4. converte low certainty em “sem efeito”;
5. converte high certainty em “efeito grande/importante”;
6. trata direct evidence como automaticamente unbiased;
7. dá equal rhetorical weight a fontes fracas/fortes só por balance;
8. confunde body certainty com recommendation strength;
9. amplia população/outcome/time/context sem suporte;
10. fortalece causal language além do desenho;
11. deixa practitioner/lay version mais certa que technical;
12. esconde fonte material de uncertainty;
13. resume conflito por votação de papers;
14. usa “mais estudos” sem especificar update condition;
15. transforma mechanistic result em demonstrated chronic performance/clinical benefit sem bridge evidence.

---

## 22. Active recall

Sem consultar:

1. recite os oito campos do invariant core;
2. explique `did not detect` vs `no meaningful effect` vs formal equivalence;
3. diga por que estimate + CI + threshold devem viajar juntos;
4. dê exemplo de high-certainty trivial effect;
5. dê exemplo de low-certainty large point estimate;
6. diferencie bias, imprecision, inconsistency e indirectness;
7. explique por que directness não garante low RoB;
8. explique false balance sem evidence pyramid automática;
9. diferencie evidence statement de recommendation;
10. cite cinco perguntas do drift audit;
11. traduza uma conclusão técnica para linguagem leiga sem aumentar certeza;
12. diga que evidência faria uma conclusão mudar materialmente.

---

## 23. Limites deliberados

F0.10 não ensina:

- comunicação de risco clínico individual personalizada;
- prescrição nutricional;
- guideline development completo;
- formal Evidence-to-Decision panel methods;
- journalism/marketing;
- persuasion detached from evidence;
- meta-analysis avançada;
- Bayesian decision theory avançada.

O objetivo é mais fundamental:

> **A mesma verdade provisória deve continuar sendo a mesma verdade provisória em qualquer audiência.**

---

## 24. Regra final

Antes de publicar uma síntese, pergunte:

> **Se eu remover o jargão, população, magnitude, intervalo, threshold, certainty, applicability e limites continuam intactos — ou a simplificação transformou incerteza em certeza?**

Se transformou, a comunicação falhou mesmo que pareça clara e convincente.
