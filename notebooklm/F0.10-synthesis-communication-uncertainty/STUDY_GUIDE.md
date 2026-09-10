# F0.10 — NotebookLM Study Guide

**Package state:** `READY_FOR_STUDY`
**Manifest version:** `1`
**Use with:** the exact six-source corpus defined in `MANIFEST.md`

This guide trains **compression without epistemic loss**. Do not treat communication as a final cosmetic step. The learner must first reconstruct the evidence judgment, freeze the invariant core, then translate it for different audiences without changing what the evidence supports.

For every pass:

1. answer from memory before consulting NotebookLM;
2. ask NotebookLM to challenge the answer using only the approved corpus;
3. repair the answer in your own words;
4. repeat the repaired version without looking;
5. proceed only when the scientific content—not just the wording—is stable.

The canonical workflow is:

`reconstructed evidence → invariant core → calibrated claim → audience translation → drift audit → update conditions`

The eight-field invariant core is:

`Target → Direction → Magnitude → Precision → Threshold → Certainty → Applicability → Boundaries/update conditions`

Do not open F0.10 `EXERCISES.md` or `ANSWER_KEY.md` during first-pass study.

---

## Pass 1 — What F0.10 actually does

Without sources, explain the difference between:

- critical appraisal;
- evidence synthesis;
- communication of uncertainty;
- recommendation.

Then verify against the canonical lesson and GRADE overview.

### Required conclusion

F0.10 begins **after** a defensible evidence judgment exists. Better wording cannot repair an undefined estimand, bad synthesis or unresolved bias problem.

### Recall check

Complete from memory:

`reconstructed evidence → ______ → ______ → ______ → ______ → ______`

---

## Pass 2 — Freeze the invariant core

Recite all eight fields from memory.

Then build an invariant core for this fresh synthetic result:

- trained adults;
- fictional intervention R versus placebo;
- 8-week standardized performance test;
- lower score is better;
- `MD -9 s`;
- `95% CI -27 to +9 s`;
- practical-benefit threshold `-20 s`;
- moderate certainty, limited mainly by imprecision;
- evidence is direct for this target.

Do not write audience-facing prose yet.

### Required output

A compact eight-row table with no interpretation drift.

---

## Pass 3 — Point estimate, interval and threshold travel together

Using G1 above, answer:

1. direction of the point estimate;
2. whether the CI crosses the null;
3. whether the CI crosses the meaningful-benefit threshold;
4. what important possibilities remain compatible;
5. what a p-value alone would fail to tell you.

Then ask NotebookLM to critique any sentence that omits one of the three quantitative anchors when it is material.

### Critical trap

`not statistically significant = unimportant` is invalid.

---

## Pass 4 — Three distinct claims

Generate or use three synthetic scenarios to distinguish:

1. **did not detect a clear effect**;
2. **compatible with no meaningful effect above a stated threshold**;
3. **formal equivalence/non-inferiority conclusion**.

For each, state what evidence/design feature is required.

### Required repair

Repair:

> “The superiority test was nonsignificant, therefore the treatments are equivalent.”

Your repair must mention the compatible effect range and the need for an appropriate equivalence/non-inferiority framework and margin.

---

## Pass 5 — ASA six-principle boundary

Before consulting F0-S08, write what a p-value can and cannot establish.

Then verify the six ASA principles.

### Required distinctions

You must be able to explain why:

- `p < 0.05` is not `P(H1|data)`;
- `p > 0.05` is not proof of no effect;
- statistical significance is not effect magnitude;
- a single threshold should not determine the scientific conclusion.

### Micro-task

Rewrite a fictional sentence containing “significant, therefore clinically important” without deleting the numeric effect information.

---

## Pass 6 — Do not overcorrect on p-values

Use F0-S09 as a contrast source.

Explain why both of these are defective:

- “p<0.05 settles the question.”
- “p-values are useless and should never appear.”

Then describe a better reporting stack:

`effect estimate + uncertainty + multiplicity/context + design/bias + practical threshold + scientific interpretation`

### Recall check

What does F0-S09 add that prevents F0-S08 from being mislearned as “ban p-values”?

---

## Pass 7 — Certainty is not magnitude

Use F0-S19.

Study this fresh example:

- `MD -3 s`;
- `95% CI -11 to +5 s`;
- meaningful-benefit threshold `-20 s`;
- high certainty for the body/outcome.

Explain why “high certainty” can support a conclusion that a **large benefit is unlikely** rather than a conclusion that the intervention has a large effect.

Then construct the opposite case:

- large point estimate;
- wide CI;
- low certainty.

### Critical trap

`certainty adjective ≠ effect-size adjective`.

---

## Pass 8 — Range/threshold-aware certainty

Ask NotebookLM to explain F0-S19’s range/threshold framing.

Then classify three CIs relative to a threshold:

- entirely beyond the benefit threshold;
- crosses threshold but not null;
- crosses threshold and null.

Do not assign GRADE categories mechanically from the CI alone; discuss what the interval tells you and what other certainty domains may still matter.

### Required conclusion

A certainty judgment cannot be reduced to “CI crosses zero: yes/no.”

---

## Pass 9 — Uncertainty has different causes

Without sources, define:

- imprecision;
- risk of bias;
- inconsistency;
- indirectness;
- missing/dissemination evidence.

Then create one sentence for each that communicates the mechanism correctly.

### Required contrast

Do not say “the CI is wide because of bias” when the evidence only shows imprecision.

Do not say “the evidence is indirect because the study is biased.”

---

## Pass 10 — Directness versus internal validity

Use F0-S20 and the lesson.

Create two synthetic studies:

### Study A

Perfect target-PICO match, but high risk of differential attrition and selective outcome analysis.

### Study B

Low-risk randomized trial with precise objective outcomes, but conducted in a substantially different population and intervention context.

For each, label separately:

- internal validity/RoB concern;
- directness/applicability concern.

### Required principle

`direct ≠ unbiased` and `low RoB ≠ directly applicable`.

---

## Pass 11 — PICO scope cannot expand during translation

Use F0-S20.

Start with a target restricted to:

- trained adults;
- one fictional intervention;
- one performance outcome;
- 8 weeks.

Translate a technical statement into lay language without turning it into:

- “athletes” if the evidence was narrower;
- “everyone”;
- “overall performance”;
- “long-term benefit.”

### Drift detector

If a reader could reasonably infer a broader population/outcome/time horizon from the simplified version, the translation failed.

---

## Pass 12 — Conflict is not vote counting

Use fresh scenario G3 from the manifest:

- direct meta-analysis: `+0.3 [0.0,+0.6]`;
- large direct RCT: `+0.2 [-0.1,+0.5]`;
- observational cohort: `+1.4 [+1.0,+1.8]` with residual confounding;
- acute mechanistic biomarker: `+40%`;
- practical threshold `+0.8`.

First write the bad “2 versus 2” synthesis.

Then replace it using:

`claim → source fit → weighted evidence → residual uncertainty`.

### Required conclusion

The larger observational estimate and acute mechanistic signal cannot automatically outweigh the more direct chronic performance evidence.

---

## Pass 13 — Avoid the opposite error: mechanical hierarchy

Construct a case where:

- one tiny randomized trial is high risk and badly measured;
- one large observational study is carefully designed for a different but relevant causal question;
- one mechanistic study answers mechanism only.

Ask:

> Which source is most informative for which claim?

### Required principle

Avoiding false balance does not mean `RCT always wins`.

Evidence weighting is claim-specific.

---

## Pass 14 — Mechanism is not outcome proof

Create a fictional acute experiment where a biomarker changes substantially but chronic performance is not measured.

Write:

1. one defensible mechanistic statement;
2. one overextended performance statement;
3. the corrected performance-boundary statement.

### Recall check

Finish:

`mechanistic plausibility ≠ demonstrated ________`

---

## Pass 15 — Evidence statement versus recommendation

Use F0-S18 and the lesson.

Given a high-certainty evidence statement for a small effect, list additional inputs that may be required before a recommendation is made:

- benefits/harms across outcomes;
- values/preferences;
- resources/cost;
- feasibility;
- acceptability;
- equity;
- decision context.

### Required repair

Repair:

> “The evidence is high certainty, so this should be strongly recommended.”

Do not weaken the certainty statement; separate it from the recommendation process.

---

## Pass 16 — Technical synthesis

Build a technical synthesis for G1.

It must preserve:

- target;
- point estimate;
- CI;
- threshold;
- main uncertainty source;
- certainty;
- applicability;
- inferential boundary.

Maximum 150 words.

Then ask NotebookLM to identify any field omitted or any causal/certainty overstatement.

---

## Pass 17 — Practitioner-facing translation

Translate the same G1 synthesis for a practitioner.

Reduce notation/jargon where helpful, but preserve:

- who the evidence concerns;
- whether effect is likely small/uncertain;
- whether meaningful benefit remains plausible;
- confidence level and main limitation;
- target scope.

### Drift rule

You may compress `95% CI -27 to +9 s` into an accurate verbal range if the exact number would obstruct communication, but you may not delete the substantive uncertainty.

---

## Pass 18 — Lay-facing translation

Translate G1 again for a general reader.

Maximum 90 words.

Avoid:

- “works”;
- “doesn’t work”;
- “proved”;
- “no difference”;
- “safe/effective for everyone.”

unless the evidence truly supports those claims, which G1 does not.

### Required comparison

Place technical, practitioner and lay versions side by side and identify where the same eight-field core appears in each.

---

## Pass 19 — Drift audit under pressure

Ask NotebookLM to deliberately corrupt one translation by introducing four drift errors selected from:

- broader population;
- stronger causal verb;
- omitted CI/range;
- deleted threshold;
- certainty upgraded;
- bias limitation deleted;
- recommendation inserted;
- chronic outcome substituted for acute outcome.

Find and repair all four.

### Mastery signal

You should be able to detect drift even when the rewritten sentence sounds smoother and more persuasive.

---

## Pass 20 — Update conditions and final integration

Take a fresh synthetic evidence package not used above.

Complete, in order:

1. reconstructed evidence summary;
2. eight-field invariant core;
3. one calibrated technical claim;
4. practitioner version;
5. lay version;
6. drift audit;
7. explicit update conditions.

Your update conditions must say **what specific new result, precision change, target-population evidence, bias resolution or threshold change would alter the conclusion**.

Then close NotebookLM and recite from memory:

- the canonical workflow;
- all eight invariant-core fields;
- the three distinct claims around nonsignificance/equivalence;
- five distinct uncertainty mechanisms;
- why directness is not validity;
- why evidence certainty is not recommendation strength;
- the rule for false balance;
- at least five drift-audit questions.

---

# Independent assessment gate

After completing the study passes:

1. close NotebookLM;
2. complete `foundations/F0-scientific-literacy/F0.10-synthesis-communication-uncertainty/EXERCISES.md` independently;
3. do not consult `ANSWER_KEY.md` during the attempt;
4. compare with `ANSWER_KEY.md` only after the attempt is complete;
5. record actual learner performance only when it truly exists.

Package completion alone does not change any learner state.

The F0.4 quantitative diagnostic remains `UNOBSERVED` until actual learner responses exist.

The cumulative F0 exit assessment remains deferred until the F0.10 study package is complete; this guide does not itself execute that assessment.

---

# Non-negotiable final rule

Before sending any evidence synthesis to any audience, ask:

> **Did I simplify the language, or did I simplify away the uncertainty?**

Only the first is acceptable.
