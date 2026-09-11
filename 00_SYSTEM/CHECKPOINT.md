# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-11
**Canonical branch:** `main`
**Project state:** `F0_EXIT_ASSESSMENT_READY`

## Canonical project state

- repository is public;
- GitHub remains canonical; NotebookLM is a controlled study layer;
- production and learner validation are separate;
- no private health data, secrets or non-redistributable third-party full text may be persisted;
- scientific/methodological claims that are living/versioned must be rechecked when materially relevant;
- learner status changes require observed evidence, never content-production inference.

## F0 production status

`F0 — Scientific Literacy and Quantitative Reasoning`

All ten instructional units are approved and all ten NotebookLM packages are ready:

| Module | Unit | NotebookLM |
|---|---|---|
| F0.1 Scientific questions/hypotheses/operationalization | APPROVED | READY_FOR_STUDY |
| F0.2 Study designs and inference boundaries | APPROVED | READY_FOR_STUDY |
| F0.3 Bias/confounding/causal reasoning/validity | APPROVED | READY_FOR_STUDY |
| F0.4 Descriptive statistics/distributions/sampling variation | APPROVED | READY_FOR_STUDY |
| F0.5 Estimates/CIs/p-values/effect sizes/practical relevance | APPROVED | READY_FOR_STUDY |
| F0.6 Power/Type I-II/multiplicity/analytical flexibility | APPROVED | READY_FOR_STUDY |
| F0.7 Systematic reviews/meta-analysis/heterogeneity | APPROVED | READY_FOR_STUDY |
| F0.8 Risk of bias/certainty/applicability | APPROVED | READY_FOR_STUDY |
| F0.9 Critical reading of a complete paper | APPROVED | READY_FOR_STUDY |
| F0.10 Synthesis/communication of uncertainty | APPROVED | READY_FOR_STUDY |

F0.4 additionally has a quantitative entry diagnostic. Its state remains `UNOBSERVED`.

Key canonical reasoning chains remain:

- F0.1: `question → target population → contrast → outcome → time → estimand`;
- F0.3: `target causal question/estimand → causal structure → distortion mechanism → adjustment/conditioning → repairability/data limitation → calibrated conclusion`;
- F0.5: `Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`;
- F0.9: `Question/estimand → Design/sampling → Intervention/exposure/comparator → Outcome measurement → Bias/confounding/missingness → Sample size/analysis plan → Effect estimate/uncertainty → Multiplicity/exploration → Result robustness → Applicability → Consistency with authors’ conclusion → What the paper does not establish`;
- F0.10: `reconstructed evidence → invariant core → calibrated claim → audience translation → drift audit → update conditions`.

Persistent safeguards:

- association ≠ causation;
- randomized ≠ automatically low risk of bias;
- reporting completeness ≠ validity/certainty;
- risk of bias is result-specific/domain-based, not a total quality score;
- `p<0.05` ≠ truth/importance;
- `p>0.05` ≠ no effect/equivalence;
- frequentist CI ≠ posterior probability interval;
- completed-study interpretation uses estimate + CI + practical threshold + design/bias, not observed power;
- multiplicity includes outcomes, timepoints, subgroups, models and data-dependent paths;
- prespecification improves auditability but does not guarantee validity;
- systematic review ≠ meta-analysis and pooling is compatibility-dependent;
- inverse-variance weight is precision, not quality/certainty;
- I² is not a quality or sameness score;
- certainty is body/outcome/question specific and not effect magnitude;
- internal validity and applicability are separate;
- one-paper appraisal ≠ body-level GRADE certainty;
- certainty of one outcome ≠ recommendation strength;
- audience simplification cannot increase certainty or broaden target scope.

## F0-A22 — cumulative Exit Assessment v1

`F0-A22` is complete.

Approved packet:

`foundations/F0-scientific-literacy/F0-exit-assessment/`

Verified files on `main`:

- `ASSESSMENT.md` — cumulative 100-point learner-facing assessment;
- `ANSWER_KEY.md` — point-by-point scoring, acceptable alternatives, critical-fail triggers and remediation mapping;
- `QA_REPORT.md` — `PASS — READY_FOR_ADMINISTRATION`.

### Structure

The approved blueprint structure is preserved exactly:

- Section A — question/design/causal structure: `20`;
- Section B — quantitative interpretation: `25`;
- Section C — systematic review/certainty: `20`;
- Section D — full-paper critical appraisal: `25`;
- Section E — communication of uncertainty: `10`;
- total: `100`.

Exit gate remains:

- total `>=85/100`;
- every section `>=70%`;
- no `CRITICAL_FAIL`;
- Section D must show a defensible integrated appraisal chain;
- Section E must preserve epistemic content when language is simplified.

`75–84` with no critical fail = `NEAR_PASS / TARGETED_REMEDIATION`.

Below `75` = broader remediation mapped to earliest broken dependency.

A first strong pass may support `APPLIED`/`INTEGRATED`; it does not automatically authorize `MASTERED`, which requires robust/repeated performance over time.

### Fresh transfer design

- Sections A–C and E use new synthetic scenarios/numbers rather than copying module assessments;
- Section C contains a five-study synthetic forest/evidence-synthesis package with visible heterogeneity;
- Section D uses a different real paper from the F0.9 training paper;
- answer-key scoring rewards reasoning rather than one memorized wording;
- checklist-only Section D remains capped at 60% of that section.

### Section D source

`F0-S32` — Jagłowska K, Folwarski M, Chroboczek M, Potrykus M, Kaczmarczyk M, Skonieczna-Żydecka K, Kaczor JJ. *Multistrain Probiotic Supplementation Combined with a Standardized Diet Did Not Significantly Affect Exercise Performance or Inflammatory Responses in Male Endurance Runners: A Randomized Controlled Trial.* Nutrients. 2026;18(15):2484. doi:10.3390/nu18152484.

- published 1 August 2026;
- human randomized double-blind parallel placebo-controlled exercise/nutrition trial;
- trained male endurance runners;
- standardized diet;
- quantitative 95% CIs and explicit multiplicity handling;
- preliminary/exploratory design with missed recruitment target and per-protocol/complete-case analysis;
- public registration occurred retrospectively;
- full text is legally accessible through PMC and marked CC BY;
- no third-party full text/figure/table was copied into GitHub.

`F0-S33` — ClinicalTrials.gov `NCT07411482` is the registry/timeline companion.

The paper contains an internal reporting inconsistency: main methods/limitations identify retrospective registration after enrolment, while the institutional statement uses prospective/prior-enrolment language. Exit scoring follows the explicit reported dates/timeline and rewards detection of the inconsistency rather than accepting either label mechanically.

`SOURCE_INDEX.md` was advanced to `Last researched: 2026-09-11` and now registers `F0-S32`/`F0-S33` without removing prior sources.

## Current learner position

**Learning position:** `UNSEEN`.

Repository learner artifacts confirm:

- learner initial domain remains `UNKNOWN` and must be measured rather than inferred;
- `study/MASTERY_MATRIX.md` still records F0 Scientific literacy = `UNSEEN`;
- no F0.1–F0.10 module has observed evidence sufficient for `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED`;
- F0.4 quantitative diagnostic = `UNOBSERVED`;
- `study/STUDY_HISTORY.md` contains only its template; no study session has yet been persisted;
- `study/ERROR_LEDGER.md` must only receive actual observed learner errors.

The Exit Assessment is **ready but must not yet be scored/administered as if prerequisites were learned** merely because production is complete.

## Operational constraints for learner validation

- initial NotebookLM corpora must not include module answer keys or prerequisite diagnostics;
- answer keys may be used for scoring only after independent response;
- learner-state changes require observed performance;
- F0.4 diagnostic must be administered before treating quantitative prerequisites as demonstrated;
- remediation/retests must use new numbers/scenarios/papers when transfer is being tested;
- actual persistent errors should be logged with cause/correction/retest plan;
- passing the exit gate permits progression but does not confer professional credentialing or clinical authority.

## NEXT_ACTION

`F0-A23` — Create the canonical learner-facing **F0 Study-to-Exit Runbook** at `study/F0_STUDY_RUNBOOK.md` using the already approved F0.1–F0.10 NotebookLM packages, `MASTERY_PROTOCOL.md`, F0.4 `ENTRY_DIAGNOSTIC.md`, module assessments and the new F0 Exit Assessment. The runbook must define the actual learning/validation sequence from current `UNSEEN` state to exit readiness without fabricating study activity: how to instantiate each NotebookLM corpus from its manifest; first-pass study order; active-recall checks; when module exercises are taken independently; how observed results update `STUDY_HISTORY.md`, `ERROR_LEDGER.md` and `MASTERY_MATRIX.md`; exactly where the F0.4 quantitative diagnostic occurs and how failure promotes the quantitative bridge to a structural prerequisite; criteria for advancing between modules while allowing targeted remediation; cumulative retrieval/retest spacing; readiness criteria before administering `F0-exit-assessment/ASSESSMENT.md`; exit scoring/remediation workflow; and the rule that one exit pass can support `APPLIED`/`INTEGRATED` but never automatic `MASTERED`. Keep personal/health data out of the public repository, change no learner state because no study has yet occurred, then update this checkpoint and leave exactly one subsequent `NEXT_ACTION` that begins the first observed F0.1 learner study session rather than producing more curriculum.