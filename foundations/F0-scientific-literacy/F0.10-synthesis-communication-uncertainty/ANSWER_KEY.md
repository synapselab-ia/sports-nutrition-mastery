# F0.10 — Commented answer key

**Use only after completing `EXERCISES.md`.**

This key gives scoring anchors, not mandatory wording. Equivalent answers earn credit when they preserve the same epistemic content.

---

# Section A — 20 points

## A1 — Repair the binary claim — 5 points

Full-credit example:

> The study did not detect a clear difference (`MD -9 s`, 95% CI `-41 to +23 s`); the interval remains compatible with a potentially meaningful benefit, little/no difference and some worsening, so `p=0.41` does not establish that the intervention has no effect.

### Scoring

- 2 pt: rejects `p>0.05 = no effect`;
- 1 pt: states point estimate/direction;
- 1 pt: preserves CI/compatible effects;
- 1 pt: explains that magnitude/precision were discarded by the original claim.

Critical fail if the repaired sentence still says “does not work” solely from p-value.

## A2 — High certainty is not large effect — 5 points

Expected reasoning:

- `+0.18 [+0.14,+0.22]` is tightly estimated;
- the whole interval is far below the `+1.0` importance threshold;
- therefore high certainty can support a **trivial/small** effect;
- trivial magnitude does not imply low certainty.

Possible repairs:

1. “High certainty indicates high confidence that the effect lies in a small/trivial range relative to the +1.0 threshold.”
2. “The effect appears trivial, but precisely estimated; certainty and magnitude are different dimensions.”

### Scoring

- 2 pt: certainty ≠ magnitude;
- 1 pt: uses threshold;
- 1 pt: uses CI/precision;
- 1 pt: both repairs are coherent.

## A3 — Directness versus bias — 5 points

Expected:

- target matching addresses directness/applicability;
- differential attrition can distort who remains observed;
- unblinded subjective outcome measurement can systematically distort the result;
- therefore evidence can be highly direct yet high/some-concerns RoB.

### Scoring

- 2 pt: separates directness from internal validity;
- 2 pt: explains at least one bias mechanism;
- 1 pt: avoids global study-quality scoring.

## A4 — Evidence statement versus recommendation — 5 points

Full-credit example:

> Moderate-certainty evidence suggests a small benefit for the specified outcome in the studied population.

> This does not by itself justify a strong recommendation because recommendation strength also depends on other outcomes, harms, values/preferences, resources, feasibility, acceptability and decision context.

### Scoring

- 2 pt: calibrated evidence statement;
- 3 pt: recommendation boundary with at least three additional decision dimensions.

---

# Section B — 20 points

## B1 — 5 points

`MD -12 [-44,+20]`, threshold `-30`.

Correct interpretation:

- point estimate favors intervention;
- CI crosses `0`;
- CI crosses `-30` threshold;
- CI extends to positive values, so some worsening is compatible;
- data do not establish either important benefit or absence of benefit.

Model sentence:

> The estimate favors the intervention by 12 s, but the 95% CI spans from a 44-s benefit to a 20-s worsening, crossing both the null and the 30-s benefit threshold; meaningful benefit, little/no difference and some worsening remain compatible with the data.

## B2 — 5 points

`MD -4 [-18,+10]`.

Yes: relative to the predefined `-30 s` threshold, the interval excludes a benefit of 30 s or larger in the favorable direction under the stated model/assumptions.

No: this does not prove exact zero effect. Small benefits and small worsening remain compatible.

### Full-credit distinction

`evidence compatible with no important benefit >=30 s` ≠ `effect exactly zero`.

## B3 — 5 points

Expected:

- a nonsignificant superiority test does not establish equivalence;
- equivalence requires an explicit equivalence framework/margins and analysis designed to test whether effects lie within them;
- `p=0.62` alone does not provide that.

## B4 — 5 points

Study 2 constrains the effect better relative to `-30 s`:

- Study 1 CI `[-90,+40]` includes large important benefit and worsening;
- Study 2 CI `[-15,+1]` excludes the `-30 s` important-benefit threshold;
- therefore Study 2 is much more informative about ruling out a >=30-s benefit, regardless of binary significance labels.

---

# Section C — 20 points

## C1 — False-balance audit — 8 points

Expected answer:

`2 vs 2` treats source count as information weight. The four sources answer different questions with different validity/directness.

At minimum discuss four of:

1. target-question fit;
2. design appropriate to claim;
3. risk of bias;
4. effect magnitude;
5. precision/CI;
6. directness/applicability;
7. synthesis context;
8. outcome compatibility;
9. time horizon;
10. whether a mechanistic result actually estimates the target outcome.

The direct RCT and systematic review should usually carry greater weight for the chronic intervention-effect claim than the confounded observational association or acute biomarker result, without turning that into a universal design hierarchy.

### Scoring

- 3 pt: explains why vote counting is invalid;
- 4 pt: four relevant weighting properties;
- 1 pt: avoids a mechanical hierarchy.

## C2 — Name the uncertainty mechanism — 8 points

1. **Imprecision** — CI crosses materially different decision regions.
2. **Inconsistency** — direct studies yield materially different effects without credible explanation.
3. **Indirectness** — evidence population differs materially from target with plausible effect modification/transfer concern.
4. **Bias** — differential missingness related to true outcomes can systematically distort the estimate.

2 points each: label + mechanism.

## C3 — Update conditions — 4 points

Examples:

- strengthen: a large low-risk direct RCT with CI entirely beyond the `-30 s` benefit threshold;
- weaken large-benefit hypothesis: a large low-risk direct body with CI tightly inside the trivial/small range and excluding `-30 s`;
- strengthen concern: credible evidence that missing unpublished trials systematically favor smaller/null effects;
- alter applicability: new direct trials in the exact target population showing materially different effects.

2 points per concrete, directionally interpretable update condition.

“More studies” alone = 0 for that condition.

---

# Section D — Fixed evidence package — 40 points

## D1 — Invariant core — 10 points

Expected extraction:

### 1. Target

Trained adult endurance athletes; daily Intervention X; 8–12 weeks; matched placebo/no X; 20-km time-trial performance; seconds to completion, lower better.

### 2. Direction

Most direct randomized point estimates favor X slightly, but not uniformly beyond a meaningful threshold.

### 3. Magnitude pattern

- systematic review: `-20 s`;
- large newer low-risk RCT: `-12 s`;
- small high-risk RCT: `-75 s`;
- larger favorable observational association: `-48 s` but different population/outcome and residual confounding;
- acute biomarker result does not estimate chronic performance.

### 4. Precision

- meta-analysis `[-42,+2]` includes important benefit and little/no benefit;
- large RCT `[-27,+3]` excludes `-30 s` threshold but permits small benefit/no difference;
- small RCT `[-140,-10]` is wide and high risk.

### 5. Threshold

Important benefit = `-30 s`.

- meta-analysis crosses threshold;
- large direct RCT excludes threshold;
- high-risk small RCT exceeds threshold but has low inferential reliability.

### 6. Certainty

Supplied body-level judgment = **MODERATE** for the target outcome.

### 7. Applicability

Direct randomized evidence is mostly close to the trained endurance target. Observational cohort is recreational runners/10-km, so more indirect. Acute mechanism is temporally/outcome indirect for chronic performance.

### 8. Boundaries/update conditions

- large benefit is not strongly established;
- small benefit remains plausible;
- no formal recommendation;
- conclusion could change with larger direct low-risk evidence whose CI clearly lies beyond or clearly excludes the `-30 s` threshold, or evidence that materially changes bias/missing-evidence judgments.

### Weighting explanation

The observational source is down-weighted because self-selection/residual confounding and target mismatch limit causal/applicability inference. The mechanistic source is not a co-equal estimator because it measures an acute biomarker, not chronic performance. The small RCT's large effect is down-weighted by high attrition, selective-analysis concerns and imprecision.

### Scoring

- 8 fields: 1 pt each;
- correct differential weighting: 2 pt.

## D2 — Technical synthesis — 10 points

Model answer (~150 words):

> In trained adult endurance athletes, the most direct randomized evidence suggests at most a small average improvement in 20-km time-trial performance with Intervention X over 8–12 weeks, but uncertainty remains around the predefined 30-s threshold for practical benefit. A six-trial meta-analysis estimated `MD -20 s` (95% CI `-42 to +2`), while a newer low-risk RCT estimated `-12 s` (`-27 to +3`), with the latter excluding a >=30-s benefit. A small high-risk RCT reported a much larger effect (`-75 s`, `-140 to -10`) but is less persuasive because of differential attrition, selective-analysis concerns and imprecision. A favorable observational association is vulnerable to residual confounding and indirectness, and the acute biomarker study does not estimate chronic performance. Overall certainty for the target outcome is moderate: a small benefit remains plausible, whereas a large benefit is less well supported. This evidence statement alone does not establish a recommendation.

### Scoring

- 2 pt: target/scope;
- 2 pt: direct estimates + CI/threshold;
- 1 pt: moderate certainty;
- 2 pt: correct down-weighting of large discordant effects;
- 1 pt: mechanism ≠ performance;
- 1 pt: recommendation boundary;
- 1 pt: residual uncertainty.

## D3 — Practitioner-facing synthesis — 8 points

Model answer:

> Para atletas adultos já treinados em endurance, os estudos randomizados mais fortes apontam para uma melhora pequena, não para um ganho grande e garantido. A revisão combinada ainda permite tanto um benefício acima de 30 s quanto pouca diferença, enquanto o maior RCT recente torna um ganho de 30 s ou mais menos provável. Os resultados muito maiores vêm de um estudo pequeno com problemas de viés e de um estudo observacional menos comparável ao alvo. O estudo de biomarcador mostra mecanismo possível, não melhora crônica de performance. A confiança geral é moderada: benefício pequeno continua possível, mas benefício grande é menos sustentado. Isso não é, sozinho, uma recomendação de uso.

### Scoring

- 2 pt: target and direction;
- 2 pt: uncertainty/threshold survives;
- 1 pt: moderate certainty;
- 1 pt: weighting preserved;
- 1 pt: mechanism boundary;
- 1 pt: no recommendation drift.

## D4 — Lay-facing synthesis — 8 points

Model answer:

> Em adultos já treinados para endurance, a melhor evidência aponta para, no máximo, uma melhora pequena com a Intervenção X. Ainda existe incerteza: alguns resultados permitem uma melhora relevante, mas o maior estudo recente não sustenta um ganho de 30 segundos ou mais. Os resultados mais impressionantes vieram de estudos menos confiáveis para essa pergunta, e uma mudança em biomarcador não prova melhora de desempenho ao longo de semanas. A confiança no conjunto é moderada. Portanto, um benefício pequeno ainda é possível, mas um grande benefício não está bem demonstrado — e isso, por si só, não diz se alguém deveria usar a intervenção.

### Scoring

- 2 pt: target retained;
- 2 pt: uncertainty/threshold retained in plain language;
- 1 pt: moderate confidence retained;
- 1 pt: weak-source weighting retained;
- 1 pt: mechanistic boundary retained;
- 1 pt: no advice/recommendation.

## D5 — Language-drift audit — 4 points

Any four of these must remain invariant in substance:

- trained adult endurance target;
- 8–12-week chronic-performance question;
- strongest evidence favors small effects;
- `-30 s` threshold matters;
- meta-analysis still crosses the threshold/null region;
- large RCT excludes >=30-s benefit while allowing small effect;
- certainty = moderate;
- large effect from small RCT is down-weighted for RoB/imprecision;
- observational source is not co-equal causal evidence;
- acute biomarker ≠ chronic performance;
- no formal recommendation;
- small benefit remains plausible; large benefit less supported.

Full credit requires an explicit comparison across D2–D4 and correction of any drift found.

---

# Critical-fail adjudication

A learner cannot pass if any critical fail in `EXERCISES.md` remains materially present after the final response.

Especially important in D:

- saying “Intervention X works” in lay language when technical language is moderate/uncertain = fail;
- saying “does not work” because a direct CI crosses zero = fail;
- presenting the observational `-48 s` as equal to the randomized estimates = fail;
- using acute biomarker improvement as proof of chronic performance = fail;
- issuing advice/recommendation from the supplied evidence package = fail.

---

# Remediation routing

If the learner fails primarily because of:

- binary p-value reasoning → return to F0.5;
- CI/threshold loss → F0.5;
- study-count synthesis / heterogeneity confusion → F0.7;
- certainty/magnitude/recommendation collapse → F0.8;
- paper-level inference/design mismatch → F0.9;
- audience language drift with otherwise correct appraisal → repeat F0.10 translation/drift passes.

---

# Mastery note

A score of `>=80/100 + no critical fail` satisfies the **local F0.10 assessment gate only when performance is actually observed and scored**.

Creating this answer key does not mark the learner `STUDIED`, `APPLIED`, `INTEGRATED` or `MASTERED`.
