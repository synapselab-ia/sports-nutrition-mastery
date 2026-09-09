# F0.7 — NotebookLM Study Package QA Report

**Module:** `F0.7 — Systematic reviews, meta-analyses and heterogeneity`
**Package version:** `1`
**Reviewed:** `2026-09-09`
**Package decision:** `PASS — READY_FOR_STUDY`
**Learner-state change:** none
**F0.4 quantitative diagnostic change:** none; remains `UNOBSERVED`

This report records QA of the NotebookLM package only. It does not record that the learner studied F0.7 and does not authorize any mastery-state transition.

---

## 1. Package contents — PASS

Required files:

- `notebooklm/F0.7-systematic-reviews-meta-analysis-heterogeneity/MANIFEST.md`;
- `notebooklm/F0.7-systematic-reviews-meta-analysis-heterogeneity/STUDY_GUIDE.md`;
- `notebooklm/F0.7-systematic-reviews-meta-analysis-heterogeneity/QA_REPORT.md`.

Package is aligned to:

- approved canonical F0.7 lesson;
- F0.7 production QA;
- F0.2 study-design boundaries;
- F0.5 effect-estimate/CI interpretation;
- F0.6 prespecification/multiplicity safeguards;
- project NotebookLM protocol;
- F0.7/F0.8 scope boundary.

---

## 2. Corpus-size and auditability gate — PASS

The initial corpus contains exactly **five sources**:

1. canonical F0.7 lesson — `CORE`;
2. Cochrane Handbook Chapter 10 — `CORE`;
3. Cochrane Handbook Chapter 6 — `SUPPORT`;
4. Cochrane Handbook Chapter 13 — `SUPPORT`;
5. PRISMA 2020 — `CONTRAST`.

### Why only five

The package needs four external functions:

- meta-analysis/heterogeneity/weighting/model logic — Cochrane Chapter 10;
- effect-measure/unit compatibility before pooling — Cochrane Chapter 6;
- missing-evidence/small-study/funnel limitations — Cochrane Chapter 13;
- reporting-transparency versus validity contrast — PRISMA 2020.

The canonical lesson integrates these functions into one F0.7 workflow. Additional review-method sources would be mostly redundant for first-pass retrieval and would increase noise.

---

## 3. Source/link/version verification — PASS

Verification date: `2026-09-09`.

### Canonical F0.7 lesson

Verified on canonical `main` with production state `APPROVED`.

### Cochrane Handbook Chapter 10

Official current page verified at:

`https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-10`

Current citation on the page remains:

- title: *Analysing data and undertaking meta-analyses*;
- Handbook version `6.5`;
- Cochrane 2024;
- chapter last updated November 2024.

Rechecked methodological points used in this package:

- meta-analysis should follow, not precede, a defensible review question/eligibility/search/extraction process;
- numerical pooling should be considered only when studies address a sufficiently coherent scientific question;
- generic inverse-variance weighting uses the inverse of the effect-estimate variance, so smaller SE generally means greater statistical weight;
- random-effects models assume different but related underlying effects and do not make heterogeneity cease to matter;
- fixed-effect/random-effects choice has no universal one-model rule and should not be based only on a heterogeneity test;
- clinical, methodological and statistical heterogeneity are distinct;
- I² threshold interpretation can mislead and requires context;
- random-effects pooled CI describes uncertainty around the average effect, not the width of the underlying effect distribution;
- prediction intervals are conceptually relevant to between-study effect spread;
- sensitivity analyses should examine robustness to influential methodological decisions.

No current-page change invalidated the approved F0.7 lesson or package.

### Cochrane Handbook Chapter 6

Official current page verified at:

`https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-06`

Current citation remains:

- title: *Choosing effect measures and computing estimates of effect*;
- Handbook version `6.5`;
- Cochrane 2024;
- chapter last updated August 2023.

Rechecked functions used here:

- outcome data type constrains valid effect measures;
- MD/SMD and risk/odds/rate measures are different statistical objects;
- ratio measures are commonly analysed on logarithmic scales;
- study results may require conversion to a consistent usable format before synthesis;
- unit-of-analysis structure must be preserved.

F0.7 uses these points for compatibility decisions, not as a license to mechanically convert substantively different constructs.

### Cochrane Handbook Chapter 13

Official current page verified at:

`https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-13`

Current citation remains:

- title: *Assessing risk of bias due to missing evidence in a meta-analysis*;
- Handbook version `6.5`;
- Cochrane 2024;
- chapter last updated August 2024.

Rechecked functions used here:

- selective non-reporting/non-publication can distort a meta-analysis;
- funnel plots display effect estimates against study size/precision;
- funnel asymmetry can have multiple explanations;
- small-study effects are not synonymous with publication bias;
- funnel asymmetry is not diagnostic of non-reporting bias;
- tests for funnel asymmetry generally have low power and are usually considered only when a sufficient number of studies is available;
- apparent symmetry cannot establish complete evidence.

Formal ROB-ME judgment remains excluded from F0.7 and deferred to F0.8.

### PRISMA 2020

Official current site verified at:

`https://www.prisma-statement.org/prisma-2020`

Verified current state:

- PRISMA 2020 remains the main PRISMA reporting guideline;
- official site exposes the statement paper, 27-item checklist, expanded checklist, abstract checklist and flow diagrams;
- PRISMA describes how systematic reviews should transparently report why the review was done, methods used and results found.

Package use is intentionally contrastive:

`reporting visibility ≠ methodological validity ≠ low risk of bias ≠ high certainty`.

No source-version/access change requires amendment of the approved F0.7 lesson.

---

## 4. Role-assignment QA — PASS

### `CORE` — canonical F0.7 lesson

Function:

- exact project vocabulary;
- integrated F0.2/F0.5/F0.6 reasoning;
- synthetic heterogeneous synthesis;
- twelve-field audit sequence;
- critical fails and F0.8 boundary.

Limitation: project-authored instructional material rather than independent methodological authority.

### `CORE` — Cochrane Chapter 10

Function:

- pooling defensibility;
- inverse-variance weighting;
- fixed/random-effects models;
- heterogeneity/I²/tau²/prediction-interval reasoning;
- subgroup/meta-regression and sensitivity cautions.

Limitation: broad/technical chapter; package deliberately avoids advanced derivations and exhaustive estimator choice.

### `SUPPORT` — Cochrane Chapter 6

Function:

- effect-measure/data/unit compatibility before pooling.

Limitation: compatibility remains a scientific/construct judgment, not purely a statistical conversion exercise.

### `SUPPORT` — Cochrane Chapter 13

Function:

- missing evidence;
- small-study effects;
- funnel asymmetry limitations.

Limitation: formal missing-evidence risk-of-bias assessment extends beyond F0.7.

### `CONTRAST` — PRISMA 2020

Function:

- prevent the common category error `transparent reporting = high-quality/high-certainty evidence`;
- make review process visible enough to audit.

Limitation: reporting guideline, not a risk-of-bias/certainty tool.

Each source therefore has a distinct and non-redundant learning role.

---

## 5. Required F0-A15 coverage — PASS

### Systematic review versus meta-analysis

Pass 1 repeatedly distinguishes review process from statistical pooling and includes legitimate no-pooling reviews.

### Review workflow

Passes 2–3 cover protocol/question, eligibility, search, screening, extraction, study-versus-report and result/unit structure.

### Compatibility before pooling

Pass 4 requires construct, effect measure, timepoint, contrast, direction and unit compatibility before any synthesis.

### Inverse-variance weighting

Pass 6 requires manual P1 calculations and the explicit statement `weight = precision, not quality`.

### Fixed versus random effects

Pass 7 requires target-quantity/model reasoning and explicitly blocks `random effects solves heterogeneity`.

### Pooled CI versus between-study variation

Pass 8 requires the distinction between pooled-mean uncertainty and prediction/between-study spread.

### Forest plots

Pass 5 preserves the complete F0.5 interpretation sequence before adding compatibility, weight/model, heterogeneity and pooling-defensibility.

### Clinical/methodological/statistical heterogeneity

Pass 9 separates all three layers and requires plausible explanations without causal overclaim.

### I²

Pass 10 uses low and high I² values and explicitly blocks sameness, quality-score and automatic-invalidity interpretations.

### Pool/no-pool decision

Pass 11 includes coherent pooling, harmonization-before-pooling and defensible no-pooling scenarios.

### Sensitivity/subgroup/meta-regression

Passes 12–13 apply F0.6 prespecification/multiplicity/direct-comparison logic.

### Small-study effects/missing evidence

Pass 14 requires multiple alternative explanations for funnel asymmetry and blocks symmetry/asymmetry as diagnoses.

### PRISMA boundary

Pass 15 explicitly separates reporting completeness from validity/risk of bias/certainty.

### Integrated synthetic audit

Pass 16 reproduces the canonical F0.7 synthetic evidence body:

- five compatible MD studies;
- random-effects pooled MD `+1.4 [0.4,+2.4]`;
- `I²=87%`;
- fixed-effect `+1.18`;
- one incompatible/differently constructed `SMD=+0.60 [0.10,+1.10]` study;
- multiple post hoc moderators;
- elite-status `p=0.04` with collinearity/non-prespecification;
- five-study symmetric-funnel overclaim;
- PRISMA/high-certainty overclaim.

All twelve audit fields are required in order.

---

## 6. Answer-leakage and prerequisite control — PASS

Excluded from initial NotebookLM corpus:

- F0.7 `EXERCISES.md`;
- F0.7 `ANSWER_KEY.md`;
- F0.7 production `QA_REPORT.md`;
- F0.4 `ENTRY_DIAGNOSTIC.md`;
- full `SOURCE_INDEX.md`.

The study guide requires closing NotebookLM before independent assessment and opening the answer key only after a first attempt.

The F0.4 quantitative diagnostic remains `UNOBSERVED`; package production creates no learner evidence.

---

## 7. Scientific-boundary QA — PASS

Package preserves these safeguards:

- systematic review ≠ meta-analysis;
- pooled estimate ≠ automatic truth/superior evidence;
- same sign ≠ effect-measure compatibility;
- SMD/MD/RR/OR are not numerically interchangeable without defensible transformation/context;
- inverse-variance weight ≠ methodological quality/certainty;
- random effects ≠ heterogeneity cure;
- fixed/random choice ≠ decision from heterogeneity p-value alone;
- pooled CI ≠ full between-study effect spread;
- clinical/methodological diversity ≠ I²;
- low I² ≠ study sameness;
- high I² ≠ automatic invalidity;
- sensitivity analysis ≠ outcome-driven result-shopping;
- subgroup significance comparison ≠ interaction;
- post hoc meta-regression ≠ proven source of heterogeneity;
- small-study effect ≠ publication bias proven;
- funnel asymmetry ≠ diagnosis;
- funnel symmetry ≠ proof of complete evidence;
- PRISMA-complete ≠ low risk/high quality/high certainty;
- formal RoB/GRADE/applicability remains F0.8.

---

## 8. Pedagogical QA — PASS

The study sequence progresses from:

`review object/workflow → study/report structure → compatibility → forest anatomy → weighting → model target → pooled CI versus effect spread → heterogeneity layers → I² repair → pooling decision → sensitivity → subgroup/meta-regression → small-study/missing evidence → PRISMA contrast → integrated audit`

This prevents the common error of teaching meta-analysis from the pooled diamond outward.

The package repeatedly requires:

- classification;
- calculation;
- misconception repair;
- model comparison;
- scientific pooling decisions;
- alternative explanations;
- full evidence-synthesis audit.

It therefore reaches application/integration rather than passive terminology recall.

---

## 9. Copyright/public-repository QA — PASS

- no third-party PDF/chapter/article text was committed to GitHub;
- package contains only project-authored Markdown, citations and links;
- PRISMA's CC BY status does not need to be relied upon because the checklist itself was not copied into the repository;
- no personal/clinical learner data was persisted;
- all sports/performance examples are synthetic methodological exercises;
- no substantive nutrition recommendation is produced by the package.

---

## 10. Production/learning-state separation — PASS

After F0-A15 package production:

- F0.1 remains pending/unvalidated;
- F0.2 remains pending/unvalidated;
- F0.3 remains pending/unvalidated;
- F0.4 remains pending/unvalidated;
- F0.4 quantitative diagnostic remains `UNOBSERVED`;
- F0.5 remains pending/unvalidated;
- F0.6 remains pending/unvalidated;
- F0.7 remains `UNSEEN`/unvalidated;
- no module is promoted by content/package production.

---

## 11. Final gate

> Can a learner with the F0.2/F0.5/F0.6 prerequisites use this controlled corpus to reconstruct an evidence body, decide what can be pooled, interpret study weights/models/forest plots/heterogeneity, repair I² and funnel-plot misconceptions, audit post hoc moderators, distinguish PRISMA reporting from validity, and produce a bounded twelve-field synthesis conclusion without importing formal F0.8 certainty machinery?

**Decision:** yes.

**Package decision:** `PASS — READY_FOR_STUDY`.
