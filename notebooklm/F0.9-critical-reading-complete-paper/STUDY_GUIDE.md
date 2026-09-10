# F0.9 — NotebookLM Study Guide

**Package state:** `READY_FOR_STUDY`
**Manifest version:** `1`
**Use with:** the seven-source corpus defined in `MANIFEST.md`

This guide is for active study. Do not ask NotebookLM for a finished appraisal of the real paper. The value of F0.9 is the reconstruction process.

For every pass:

1. answer from memory first;
2. identify which source should resolve uncertainty;
3. inspect the approved source;
4. repair the answer in your own words;
5. repeat without consultation;
6. only then advance.

The fixed appraisal sequence is:

`1. Question/estimand → 2. Design/sampling → 3. Intervention/exposure/comparator → 4. Outcome measurement → 5. Bias/confounding/missingness → 6. Sample size/analysis plan → 7. Effect estimate/uncertainty → 8. Multiplicity/exploration → 9. Result robustness → 10. Applicability → 11. Consistency with authors’ conclusion → 12. What the paper does not establish`

The real study object is `F0-S30`, with `F0-S31` as its registry companion. `EXERCISES.md` and `ANSWER_KEY.md` must remain outside the initial notebook.

---

## Pass 1 — The paper is an argument, not an answer

Before opening the full paper, state from memory why the following are insufficient as an appraisal:

- title;
- abstract;
- journal reputation;
- design label;
- authors' conclusion.

Ask NotebookLM to compare your answer with the canonical lesson.

### Required principle

`authors' narrative → hypothesis to audit`

not:

`authors' narrative → final interpretation`.

### Recall check

Explain why an RCT can still have a result with material bias and why an observational paper cannot be dismissed solely because it is observational.

---

## Pass 2 — Article anatomy and source layers

From memory, list what each layer can contribute:

- main article;
- supplement/appendix;
- registry;
- protocol;
- statistical analysis plan;
- data/code repository.

Then ask NotebookLM to generate five examples of missing information and require you to choose the best source layer to inspect next.

### Critical trap

`not in the main text = did not exist` is invalid.

`document exists = prospectively prespecified` is also invalid.

---

## Pass 3 — Provenance before appraisal

Build a provenance note for `F0-S30` containing only facts you can locate directly:

- citation/DOI;
- full-text source;
- version/publication status;
- legal-access status;
- registry identifier;
- available external materials;
- any correction/retraction signal you can locate.

Do **not** interpret the trial yet.

### Required habit

Separate:

`identity/version/access facts`

from:

`methodological judgment`.

---

## Pass 4 — Reconstruct question and estimand

Before reading the discussion, fill this table from `F0-S30`:

| Field | Your extraction |
|---|---|
| Population | |
| Intervention/exposure | |
| Comparator | |
| Outcome | |
| Time | |
| Estimand/contrast | |
| Analysis population | |
| Target context | |

Then ask NotebookLM to challenge ambiguities rather than complete the table for you.

### Required distinction

Compare:

1. title question;
2. stated objective;
3. contrast actually estimated by the model.

If they differ, say how.

---

## Pass 5 — Design and sampling architecture

Classify `F0-S30` without using the design label as a verdict.

Extract:

- randomized/observational;
- parallel/crossover/cluster/factorial/other;
- unit of allocation;
- recruitment/sampling route;
- follow-up structure;
- analysis population;
- attrition/retention.

Then answer:

> What causal/inferential advantage does the design create in principle, and what execution problems could still weaken a result?

### Critical trap

Do not write `RCT = low risk of bias`.

---

## Pass 6 — Intervention and comparator reconstruction

Create an arm-by-arm table for `F0-S30`.

Include:

- what participants actually received;
- dose/composition;
- timing;
- duration;
- common exercise intervention;
- adherence/fidelity information;
- co-interventions;
- what differs between each pair of arms.

Then identify which pairwise comparisons isolate a narrower contrast and which comparisons combine more than one change.

NotebookLM may ask questions but should not give you the finished appraisal.

---

## Pass 7 — Outcome architecture

List all material outcome families/timepoints you can identify in `F0-S30`.

For each, classify:

- construct;
- operational measure;
- objective/subjective component;
- repeated measurement structure;
- decision relevance;
- whether a practical threshold is given.

### Required principle

`measurement precision ≠ construct validity`.

Explain one way a reliable measure could still fail to capture the broader claim being made.

---

## Pass 8 — Build the result table before reading the conclusion

For at least the main muscle-thickness and strength outcomes, create:

| Outcome/timepoint | Contrast | Effect measure | Point estimate | CI/SE | p-value | Analysis population | Prespecification status | Practical threshold | Caveat |
|---|---|---|---|---|---|---|---|---|---|

If a direct between-group estimate/CI is not clearly reported in the source, write `NOT CLEARLY REPORTED` rather than reconstructing one from imagination.

### Gate

Do not advance until you can distinguish:

- change over time;
- group main effect;
- group×time interaction;
- pairwise treatment contrast.

---

## Pass 9 — Within-group change versus treatment effect

Ask NotebookLM to generate three generic repeated-measures examples.

For each, classify whether the result supports:

- improvement over time;
- difference between groups;
- differential change between groups;
- none of the above.

Then return to `F0-S30` and identify which reported quantities answer which questions.

### Critical repair

`Group A improved significantly and Group B did not` does **not** prove A outperformed B.

A direct between-group comparison is required.

---

## Pass 10 — Magnitude, CI and practical threshold

Using F0.5 reasoning, interpret each material result in this order:

`Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning → Unsupported claims`

Do not start with the p-value.

### Exercise

For one result from the paper:

1. state the point estimate;
2. state the CI if available;
3. describe the compatible range;
4. identify whether a practical threshold was prespecified/provided;
5. state what the result does **not** allow you to conclude.

---

## Pass 11 — Nonsignificance is not equivalence

Before consulting sources, explain the difference among:

- failure to reject a null;
- evidence compatible with a small/trivial effect;
- formal equivalence;
- non-inferiority.

Ask NotebookLM to create a case where `p>0.05` but the CI still contains both meaningful benefit and meaningful harm.

Then inspect `F0-S30` and ask whether the reporting provides what would be required for a formal equivalence claim.

### Critical trap

`no statistically significant group difference = groups are equivalent` is invalid.

---

## Pass 12 — Sample size, precision and power

Create a three-column distinction:

| Object | When defined/used | What it answers |
|---|---|---|
| Prospective sample-size/power planning | | |
| Observed estimate + CI | | |
| Observed/post-hoc power | | |

Use `F0-S29` to repair your answer.

Then locate the paper's sample-size/power discussion and classify each calculation by function.

### Required principle

After data are observed, interpretation should return to:

`estimate + CI + practical threshold + design/bias`.

A post-study power/sensitivity calculation does not provide posterior evidence that the intervention does or does not work.

---

## Pass 13 — Registration, protocol, SAP and the clock

Use `F0-S30` and `F0-S31` to build a timeline without asking NotebookLM for the conclusion.

Record:

- study start;
- primary/study completion;
- first registry submission/posting;
- publication timing;
- any protocol/SAP timestamps you can verify.

Then classify each public record as:

- demonstrably prospective;
- retrospective;
- timing unclear.

### Required principle

`timestamp → evidentiary value for prespecification`.

The existence of a document alone does not establish prospectivity.

---

## Pass 14 — Multiplicity and claim-family mapping

From the paper, map the available claim family:

- outcomes;
- timepoints;
- arms/contrasts;
- pairwise comparisons;
- transformations/models;
- sensitivity analyses;
- any subgroup/exploratory analyses.

Then classify highlighted findings as:

- prospectively confirmatory;
- prospectively secondary;
- exploratory;
- post hoc;
- unclear.

Do not accuse selective reporting merely because multiple outcomes exist. State what evidence would be needed to strengthen that inference.

---

## Pass 15 — Result-specific risk of bias

Use `F0-S07` plus the canonical lesson.

Pick one concrete outcome/result from `F0-S30` and audit:

1. randomization process;
2. deviations from intended interventions;
3. missing outcome data;
4. outcome measurement;
5. selection of reported result.

For each concern write:

`mechanism → result affected → plausible direction/impact → evidence or uncertainty`.

### Critical trap

Do not produce a numerical score such as `8/10 quality`.

Do not transfer one result's judgment automatically to every outcome.

---

## Pass 16 — Reporting visibility versus validity

Use `F0-S01` as a navigation guide.

Ask:

- Which CONSORT items help you locate participant flow, outcomes, analysis populations, missing data, trial registration and protocol/SAP information?
- Which of those items can only tell you whether information is visible?
- Which validity judgments still require separate reasoning?

### Repair

Rewrite:

> “The paper reports CONSORT items well, therefore it is low risk of bias.”

Your replacement must preserve both transparency and independent appraisal.

---

## Pass 17 — Robustness versus result-shopping

Identify analyses in `F0-S30` that could plausibly be described as sensitivity, secondary or robustness-related.

For each, ask:

- Was the purpose stated before or after results?
- Is the alternative analysis scientifically defensible?
- Does it test an assumption or merely search for a preferable result?
- Does the substantive conclusion change?

### Required distinction

`robustness = stability under defensible assumptions`

not:

`robustness = one alternative model still has p<0.05`.

---

## Pass 18 — Applicability audit

Choose a target context different from the study sample, such as trained competitive athletes.

Compare `F0-S30` to that target across:

`Population → Intervention/exposure → Comparator → Outcome → Time → Setting → Decision context`.

For every mismatch, explain a plausible mechanism by which it could matter. Do not downgrade applicability for demographic difference by reflex.

### Required principle

`internal validity ≠ applicability`.

A result may be internally credible yet narrow in transfer.

---

## Pass 19 — One paper versus a body of evidence

Use `F0-S18` only as a contrast source.

Explain why you can appraise from `F0-S30`:

- result-specific bias;
- precision;
- applicability;
- proportionality of the authors' claims;

but cannot assign from this one paper alone:

- certainty of the entire evidence body;
- universal recommendation strength.

### Critical repair

`good RCT = high-certainty evidence overall` is an invalid shortcut.

---

## Pass 20 — Authors' conclusion audit

Only now read the discussion/conclusion carefully.

For every material claim, classify it as:

- directly supported;
- supported with caveat;
- exploratory/plausible;
- overextended;
- unsupported by the measured data.

Require a reason linked to:

- estimand;
- direct result;
- CI/precision;
- prespecification/multiplicity;
- bias;
- applicability.

Do not classify by tone or whether you personally agree with the nutrition claim.

---

## Pass 21 — What the paper does not establish

Complete at least five versions of:

> **This paper can inform ______, but does not establish ______.**

Possible categories to inspect—but not answers to copy—include:

- population scope;
- intervention component/dose/source;
- outcome scope;
- duration;
- equivalence;
- mechanism;
- body-level certainty;
- recommendation strength.

Each boundary must be tied to something actually absent or outside the measured estimand.

---

## Pass 22 — Full blind integration

Without opening `EXERCISES.md` or `ANSWER_KEY.md`, produce a complete appraisal of `F0-S30` with `F0-S31` and methodological supports.

Use exactly this structure:

### A. Provenance/version note

### B. Research question / estimand

### C. Design and sampling

### D. Intervention/exposure/comparator reconstruction

### E. Outcome measurement

### F. Material result table

### G. Bias/confounding/missingness

### H. Sample size / analysis plan / power

### I. Multiplicity / prespecification timeline

### J. Robustness

### K. Applicability

### L. Strongest defensible inference

### M. Authors' conclusion audit

### N. What the paper does not establish

Then finish by reciting the **12-step F0.9 sequence from memory**.

### Self-audit before independent assessment

Reject your own response if it does any of the following:

- relies on abstract/title only;
- treats RCT as the appraisal;
- uses CONSORT completion as validity;
- leads with p-values rather than estimates/uncertainty;
- treats within-group change as a treatment effect;
- treats nonsignificance as equivalence;
- invokes observed power to rescue interpretation;
- assumes registration was prospective without checking dates;
- ignores multiplicity;
- gives one global quality/RoB score;
- mistakes open data for valid design;
- assigns GRADE certainty to the whole field from one paper;
- repeats the authors' conclusion without reconstructing the result;
- fails to state explicit non-established claims.

---

# NotebookLM prompt template

Use this when beginning a session:

> Act as a strict Socratic examiner for F0.9. Use only the seven approved sources in the manifest. Do not reveal or reconstruct the project's hidden `ANSWER_KEY.md`. Require me to extract facts from the full paper and registry myself. When I make a claim, ask which source supports it and whether it is a factual extraction or an appraisal judgment. Enforce the twelve-step F0.9 sequence. Prioritize estimand, direct effect estimates and confidence intervals over significance labels. Reject within-group-as-treatment-effect, p>0.05-as-equivalence, observed-power rescue, checklist-as-validity, untimestamped prespecification claims, global quality scores and single-paper GRADE certainty. If information is unavailable, make me say `UNCLEAR / NOT REPORTED` rather than inventing it.

---

# Completion rule

Do not open the independent `EXERCISES.md` or `ANSWER_KEY.md` until you can complete Pass 22 without assistance that supplies the appraisal conclusions.

Finishing these passes is preparation for assessment. It does not automatically change any learner/mastery state in the GitHub repository.
