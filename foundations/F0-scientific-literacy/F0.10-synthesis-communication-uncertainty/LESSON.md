# F0.10 — Síntese e comunicação da incerteza

**Production state:** `APPROVED_PENDING_QA`

**Prerequisites P2:** F0.5 — estimativas, intervalos, effect sizes e relevância prática; F0.7 — síntese, heterogeneidade e missing evidence; F0.8 — risk of bias, certeza e aplicabilidade; F0.9 — leitura crítica de paper completo.

**P0 ensinados localmente:** calibrated language, claim scope, epistemic content, invariant core, evidence statement, recommendation statement, audience translation, language drift, decision threshold, conclusion-changing evidence.

**P1 ensinados localmente:** transformar uma mesma síntese em versões técnica, practitioner-facing e lay-facing sem alterar direção, magnitude, incerteza, certeza, aplicabilidade ou limites de inferência.

**Core/method sources:** `F0-S08`, `F0-S09`, `F0-S18`, `F0-S19`, `F0-S20`, além das unidades canônicas F0.5/F0.7/F0.8/F0.9.

## 1. Competência-alvo

Ao terminar esta unidade, você deve conseguir receber um resultado ou evidence body já criticamente reconstruído e comunicá-lo para públicos diferentes sem:

1. transformar um p-value em verdade binária;
2. esconder magnitude ou intervalo de confiança;
3. apagar um limiar de importância prática;
4. converter `low certainty` em “não funciona”;
5. converter `high certainty` em “efeito grande/importante”;
6. dar o mesmo peso retórico a evidências de força muito diferente só para parecer equilibrado;
7. confundir directness com ausência de bias;
8. confundir certeza da evidência com força de recomendação;
9. ampliar população, outcome, duração ou contexto além do que a evidência sustenta;
10. tornar a versão leiga mais certa que a síntese técnica.

Regra central:

> **Simplificar linguagem pode reduzir complexidade verbal; não pode reduzir a incerteza científica.**

A função de F0.10 é converter um julgamento de evidência em comunicação calibrada sem perda epistemológica.

---

# 2. O objeto que precisa sobreviver à tradução: invariant core

Antes de escrever para qualquer público, congele oito campos:

1. **Target** — população, intervenção/exposição, comparator, outcome, tempo e contexto;
2. **Direction** — para onde a estimativa aponta;
3. **Magnitude** — quão grande é o efeito na escala relevante;
4. **Precision** — qual intervalo/uncertainty acompanha a estimativa;
5. **Threshold** — qual magnitude mudaria uma decisão ou seria considerada importante;
6. **Certainty** — quanta confiança cabe no body/outcome inference;
7. **Applicability** — até onde o body corresponde ao target real;
8. **Boundaries** — o que ainda não foi estabelecido e o que mudaria a conclusão.

Esse conjunto é o **invariant core**.

Você pode trocar:

- vocabulário;
- extensão;
- ordem das frases;
- densidade estatística;
- exemplos.

Você não pode trocar silenciosamente:

- `may` por `does`;
- `small possible benefit` por `works`;
- `did not detect` por `has no effect`;
- `moderate certainty` por `proven`;
- `trained adults` por `everyone`;
- `12 weeks` por `long term`;
- `one outcome` por `overall health/performance`.

---

# 3. Evidência antes da redação

F0.9 terminou com um appraisal reconstruído. F0.10 começa daí.

Nunca faça:

`headline → simplify → communicate`.

Faça:

`reconstructed evidence → invariant core → calibrated claim → audience translation → drift audit`.

Se o appraisal ainda não resolveu qual estimand/outcome está em jogo, F0.10 não pode corrigir isso com palavras melhores.

---

# 4. Linguagem calibrada

A força verbal deve acompanhar o que a evidência permite.

## 4.1 Verbos e construções úteis

### Observação/descritivo

- `was associated with`;
- `was higher/lower in`;
- `co-occurred with`.

Não converter automaticamente em:

- `caused`;
- `improved`;
- `prevented`.

### Resultado experimental com incerteza relevante

- `the estimate favored X, but the interval was compatible with...`;
- `the trial did not detect a clear between-group difference`;
- `a small benefit remains plausible`;
- `the data are compatible with effects ranging from...`.

### Body com certeza moderada

- `the intervention probably...` quando esse verbo é coerente com a framework usada e o target de certainty;
- `moderate-certainty evidence suggests/probably indicates...`.

### Body com baixa certeza

- `the intervention may...`;
- `the evidence is uncertain about...`;
- `the estimate suggests..., but confidence is limited by...`.

A escolha exata do verbo não é uma tabela universal. O princípio é consistência entre **claim strength** e **evidence strength**.

---

# 5. O p-value não controla a frase

F0-S08 e F0-S09 continuam válidos aqui.

Não escreva:

- `p<0.05, therefore true`;
- `p<0.05, therefore important`;
- `p>0.05, therefore no effect`.

Escreva o resultado em termos de:

`estimate → interval → threshold → design/bias → certainty/context`.

Um p-value pode ser uma peça da saída estatística. Ele não substitui esses objetos.

---

# 6. Três claims diferentes: ausência de detecção, ausência prática e equivalência

Essas frases parecem próximas, mas não são intercambiáveis.

## 6.1 “Não detectamos evidência clara de diferença”

Exemplo:

`MD = -8 s [95% CI -45, +29]`.

Se `0` é o null, o intervalo inclui benefício e dano/efeito oposto.

Uma frase defensável:

> O estudo não detectou uma diferença clara; os dados ainda são compatíveis com benefício e com pouca ou nenhuma diferença.

## 6.2 “A evidência é compatível com ausência de efeito importante”

Agora suponha um threshold de benefício importante em `-30 s` e resultado:

`MD = -4 s [95% CI -18, +10]`.

O intervalo exclui benefício maior que `30 s` nessa direção.

Uma conclusão mais forte pode ser defensável:

> Sob o threshold de 30 s, os dados são compatíveis com ausência de benefício grande/importante; efeitos pequenos ainda permanecem possíveis.

Isso é diferente de `p>0.05`.

## 6.3 Equivalence formal

Para afirmar formal equivalence/non-inferiority, é necessário um desenho/analysis framework apropriado e margens prespecificadas adequadamente.

`nonsignificant superiority test ≠ equivalence trial`.

---

# 7. Point estimate, interval e threshold devem viajar juntos

Considere:

`MD = -22 s [95% CI -51, +7]`

Threshold de benefício importante:

`-30 s`.

Uma comunicação que diz apenas:

> “O efeito médio foi de 22 s.”

perde precisão.

Uma que diz apenas:

> “Não foi significativo.”

perde magnitude e compatibilidade.

Uma melhor síntese é:

> A estimativa média favoreceu a intervenção em 22 s, mas o intervalo de 95% foi de 51 s de benefício a 7 s de piora; portanto, tanto um benefício acima do limiar de 30 s quanto pouca diferença permanecem compatíveis com os dados.

Esse é o núcleo de F0.5 preservado em F0.10.

---

# 8. Certainty não é magnitude

GRADE separa duas perguntas:

1. **Qual efeito/intervalo parece existir?**
2. **Quanta confiança temos de que o efeito verdadeiro está na faixa relevante?**

Portanto:

- `high certainty + trivial effect` é possível;
- `low certainty + large point estimate` é possível;
- `low certainty` não significa `no effect`;
- `high certainty` não significa `large benefit`.

Exemplo:

> High-certainty evidence may indicate that an intervention changes an outcome by only a trivial amount.

Isso é epistemicamente diferente de:

> The intervention has a large effect.

---

# 9. Incerteza não é uma coisa só

Ao comunicar incerteza, identifique sua origem.

## 9.1 Imprecision

Problema:

- CI amplo;
- poucos eventos;
- baixo N/information size;
- threshold crossing relevante.

Comunicação:

> “A magnitude permanece incerta porque o intervalo é amplo.”

## 9.2 Risk of bias

Problema:

- mecanismos podem deslocar sistematicamente a estimate.

Comunicação:

> “Mesmo uma estimativa precisa pode estar sistematicamente distorcida por...”

Não diga “o CI é amplo por bias” se o problema é outra coisa.

## 9.3 Inconsistency

Problema:

- estudos estimam efeitos materialmente diferentes sem explicação suficiente.

Comunicação:

> “O efeito varia entre estudos, reduzindo confiança em uma única magnitude média.”

## 9.4 Indirectness

Problema:

- evidence PICO/context não corresponde bem ao target.

Comunicação:

> “A evidência é menos direta para atletas altamente treinados porque a maioria dos estudos foi feita em...”

## 9.5 Missing/dissemination evidence

Problema:

- resultados/estudos podem estar ausentes de forma relacionada aos achados.

Comunicação:

> “A confiança é limitada pela possibilidade de evidência não observada/selecionada.”

Não reduza tudo a “mais estudos são necessários”.

---

# 10. Direct evidence ≠ unbiased evidence

Uma comparação pode ser diretamente alinhada ao target e ainda ser enviesada.

Exemplo:

- população correta;
- intervenção correta;
- comparator correto;
- outcome correto;
- duração correta;

mas:

- differential attrition;
- unblinded subjective outcome;
- selective analysis.

Isso é **direct but potentially biased**.

O inverso também é possível: um estudo pode ser internamente forte e ainda ser indirect para o target.

Mantenha os eixos separados:

`internal validity / RoB` ≠ `directness / applicability`.

---

# 11. Conflito entre estudos: não conte papers

Considere quatro fontes:

- uma meta-analysis de seis RCTs diretos;
- um RCT grande e recente;
- um observational cohort grande;
- um pequeno mechanistic study.

Não faça:

> “Dois estudos são positivos e dois negativos, então está 50/50.”

A síntese deve ponderar:

1. fit à pergunta;
2. design e bias;
3. estimand/outcome compatibility;
4. magnitude e precisão;
5. directness/applicability;
6. synthesis context;
7. body-level certainty;
8. atualidade quando material.

**False balance** ocorre quando fontes com capacidade inferencial muito desigual recebem peso retórico equivalente só porque discordam.

---

# 12. Hierarquia mecânica também é erro

Evitar false balance não significa usar uma pirâmide automática.

Um RCT pequeno e high risk não derrota automaticamente um cohort observacional cuidadosamente desenhado para uma pergunta que randomização não responde bem.

Um mechanistic experiment pode ser excelente para mecanismo e insuficiente para performance crônica.

A pergunta correta permanece:

> **Qual fonte é mais informativa para qual claim?**

---

# 13. Síntese de conflito em quatro passos

Use:

`claim → source fit → weighted evidence → residual uncertainty`.

## Passo 1 — Defina o claim

Exemplo:

> “Intervention X melhora performance de endurance em atletas treinados após 8–12 semanas.”

## Passo 2 — Classifique o fit

Para cada fonte:

- mesma população?
- mesma intervention/comparator?
- mesmo outcome?
- mesma time horizon?
- design adequado ao claim?

## Passo 3 — Pondere o corpo

Pergunte:

- quais estimates dominam pela precisão/relevância?
- quais têm maior risk of bias?
- há heterogeneity explicável?
- os resultados diretos são consistentes?

## Passo 4 — Escreva a incerteza residual

Exemplo:

> “A evidência mais direta e metodologicamente forte concentra-se perto de efeitos pequenos, enquanto os maiores efeitos aparecem em estudos menos precisos ou menos diretamente aplicáveis; portanto, benefícios grandes são menos suportados que benefícios pequenos, embora alguma incerteza permaneça.”

---

# 14. Evidence statement ≠ recommendation

Uma **evidence statement** responde:

> O que a evidência indica sobre um outcome específico?

Uma **recommendation statement** responde:

> O que alguém deve fazer?

A segunda pode exigir ainda:

- benefits e harms múltiplos;
- valores/preferências;
- custo/recursos;
- feasibility;
- acceptability;
- equity;
- contexto decisório.

Logo:

`certainty of one outcome ≠ recommendation strength`.

Mesmo uma evidência de alta certeza sobre um efeito pequeno não cria automaticamente recomendação forte.

---

# 15. Audience translation sem drift

## 15.1 Technical synthesis

Pode incluir:

- effect measure;
- point estimate;
- CI;
- threshold;
- risk-of-bias/certainty language;
- directness;
- limitations;
- exact target.

## 15.2 Practitioner-facing synthesis

Pode reduzir jargon, mas deve preservar:

- quem foi estudado;
- tamanho provável do efeito;
- amplitude da incerteza;
- grau de confiança;
- aplicabilidade;
- o que não está estabelecido.

## 15.3 Lay-facing synthesis

Pode traduzir CI para faixa plausível/compatível e certainty para linguagem comum.

Mas não pode trocar:

> “A evidência sugere um benefício pequeno, com incerteza moderada.”

por:

> “Funciona.”

Nem:

> “Não detectamos benefício claro.”

por:

> “Não funciona.”

---

# 16. Drift audit

Depois de produzir três versões, compare frase por frase.

Pergunte:

1. a população ficou mais ampla?
2. a direção mudou?
3. a magnitude desapareceu?
4. o intervalo virou certeza?
5. o threshold sumiu?
6. `may/probably` virou verbo categórico?
7. bias foi apagado?
8. applicability foi generalizada?
9. evidence statement virou recommendation?
10. uma versão leiga parece mais confiante que a técnica?

Se sim, houve **language drift**.

---

# 17. “O que mudaria minha conclusão?”

Toda boa síntese termina com update conditions.

Pergunte:

> Qual nova evidência ou mudança de assumptions faria esta conclusão mudar materialmente?

Exemplos:

- um RCT direto grande com CI estreito excluindo o threshold atual;
- reanalysis que resolve um problema material de missingness;
- confirmação de um prespecified subgroup effect;
- novos estudos na população-alvo reduzindo indirectness;
- evidência de publication/non-reporting bias que altera o body;
- mudança defensável do threshold de decisão;
- evidência de harms relevantes que muda a recomendação mesmo sem alterar efficacy.

Isso transforma a conclusão em uma posição atualizável, não dogmática.

---

# 18. Worked example A — não detectado ≠ inexistente

Outcome: performance time; menor = melhor.

- target: trained adults;
- MD = `-12 s`;
- 95% CI = `-44 a +20 s`;
- practical-benefit threshold = `-30 s`;
- low risk of bias;
- direct evidence;
- body certainty: moderate, limitada principalmente por imprecision.

## Technical

> A estimativa favorece a intervenção em 12 s, mas o IC95% de -44 a +20 s cruza tanto o null quanto o limiar de benefício importante de -30 s. Assim, os dados não demonstram benefício claro nem excluem um benefício material; a incerteza é principalmente de precisão.

## Practitioner-facing

> O melhor palpite é uma melhora pequena, mas o estudo ainda é compatível tanto com uma melhora relevante quanto com quase nenhuma diferença. Por isso, não é correto concluir nem que “funciona claramente” nem que “não funciona”.

## Lay-facing

> O resultado apontou para uma pequena melhora, mas a margem de incerteza é grande: o efeito real pode ser relevante ou pode ser praticamente nulo. Ainda não há base para uma conclusão definitiva.

O conteúdo epistemológico é o mesmo nas três versões.

---

# 19. Worked example B — high certainty, trivial effect

- pooled effect = `+0.15 unidade`;
- 95% CI = `+0.12 a +0.18`;
- threshold de importância = `+1.0`;
- high certainty.

Conclusão adequada:

> Há alta confiança de que o efeito é pequeno/trivial em relação ao threshold definido.

Conclusão inadequada:

> Há alta certeza, então o efeito é importante.

`certainty` descreve confiança sobre a faixa do efeito; não transforma sua magnitude.

---

# 20. Worked example C — conflito sem falsa equivalência

Claim: Intervention Q melhora um performance score crônico.

Evidence:

- systematic review de RCTs diretos: pooled `+0.4 [0.0,+0.8]`;
- grande RCT novo: `+0.2 [-0.1,+0.5]`;
- cohort observacional: `+1.8 [+1.3,+2.3]`, self-selection e residual confounding plausível;
- acute mechanistic experiment: biomarker aumenta 35%, sem performance endpoint.

Threshold importante = `+1.0`.

Uma síntese ruim:

> “A literatura é muito dividida: dois estudos positivos e dois inconclusivos.”

Uma síntese melhor:

> “As fontes mais diretas para performance crônica estimam efeitos pequenos e abaixo do threshold de +1.0, enquanto o maior efeito vem de evidência observacional mais vulnerável a confounding; o estudo mecanístico apoia plausibilidade, não magnitude de performance. O peso do conjunto favorece, no máximo, um efeito pequeno, com os grandes benefícios menos sustentados.”

---

# 21. Template canônico F0.10

Antes de qualquer audiência, preencha:

## A. Target

`Population / intervention-exposure / comparator / outcome / time / setting-context`

## B. Evidence direction and magnitude

`effect measure + point estimate`

## C. Precision

`CI/range + what material possibilities remain`

## D. Practical threshold

`threshold + whether CI crosses it`

## E. Main uncertainty sources

`bias / imprecision / inconsistency / indirectness / missing evidence`

## F. Certainty

`body/outcome certainty + rationale`

## G. Applicability

`where it transports / where it becomes indirect`

## H. Evidence statement

`one calibrated sentence`

## I. Recommendation boundary

`what this evidence statement does NOT decide by itself`

## J. Update conditions

`what would materially change the conclusion`

Só depois produza versões por audiência.

---

# 22. Performance-package rule

A avaliação usa um único pacote sintético de evidência para obrigar três comunicações:

1. technical;
2. practitioner-facing;
3. lay-facing.

A correção não premia “tom bonito”. Ela verifica se as três versões conservam o mesmo invariant core.

O pacote inclui evidências com pesos inferenciais diferentes de propósito. Contar papers em vez de ponderá-los é erro estrutural.

---

# 23. Critical fails

Uma resposta falha estruturalmente se:

1. usa `p<0.05` como prova de verdade/importância;
2. usa `p>0.05` como prova de ausência/equivalência;
3. omite CI/threshold material para tornar a mensagem mais simples;
4. converte low certainty em “sem efeito”;
5. converte high certainty em “efeito grande/importante”;
6. trata direct evidence como necessariamente unbiased;
7. dá igual peso retórico a fontes fracas e fortes apenas por balance;
8. confunde body certainty com recommendation strength;
9. amplia população/outcome/time/context sem justificativa;
10. usa linguagem causal além do desenho;
11. deixa practitioner/lay version mais certa que a technical version;
12. esconde uma fonte material de uncertainty;
13. resume conflito por votação de papers;
14. usa “mais estudos são necessários” sem dizer qual informação mudaria a conclusão;
15. transforma um mechanistic result em demonstrated performance/clinical benefit sem bridge evidence.

---

# 24. Active recall

Sem consultar:

1. recite os oito campos do invariant core;
2. explique `did not detect` versus `no meaningful effect` versus formal equivalence;
3. diga por que estimate + CI + threshold devem viajar juntos;
4. dê um exemplo de high-certainty trivial effect;
5. dê um exemplo de low-certainty large point estimate;
6. diferencie bias, imprecision, inconsistency e indirectness;
7. explique por que directness não garante low RoB;
8. explique false balance sem recorrer a evidence pyramid automática;
9. diferencie evidence statement de recommendation;
10. cite cinco perguntas do drift audit;
11. reescreva uma conclusão técnica em linguagem leiga sem aumentar certeza;
12. diga o que faria uma conclusão científica ser atualizável em vez de dogmática.

---

# 25. Limites deliberados

F0.10 não ensina:

- comunicação de risco clínico individual personalizada;
- prescrição nutricional;
- guideline development completo;
- formal Evidence-to-Decision panel methods;
- science journalism/marketing;
- rhetoric/persuasion detached from evidence;
- meta-analysis avançada;
- Bayesian decision theory avançada.

O objetivo é mais fundamental: **a mesma verdade provisória deve continuar sendo a mesma verdade provisória em qualquer audiência.**

---

# 26. Regra final

Antes de publicar uma síntese, pergunte:

> **Se eu remover o jargão, a população, magnitude, intervalo, threshold, certainty, applicability e limites continuam intactos — ou minha simplificação transformou incerteza em certeza?**

Se a resposta for a segunda opção, a comunicação falhou mesmo que seja clara e convincente.
