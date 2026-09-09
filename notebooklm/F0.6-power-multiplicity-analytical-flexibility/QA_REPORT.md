# F0.6 — NotebookLM Study Package QA Report

**Module:** `F0.6 — Power, Type I/II error, multiplicity and analytical flexibility`
**Package version:** `1`
**Reviewed:** `2026-09-09`
**Package decision:** `PASS — READY_FOR_STUDY`
**Learner-state change:** none
**F0.4 quantitative diagnostic change:** none; remains `UNOBSERVED`

This report records QA of the NotebookLM package only. It does not record that the learner studied F0.6 and does not authorize any mastery-state transition.

---

## 1. Package contents — PASS

Required files:

- `notebooklm/F0.6-power-multiplicity-analytical-flexibility/MANIFEST.md`;
- `notebooklm/F0.6-power-multiplicity-analytical-flexibility/STUDY_GUIDE.md`;
- `notebooklm/F0.6-power-multiplicity-analytical-flexibility/QA_REPORT.md`.

The package is aligned to:

- approved canonical F0.6 lesson;
- F0.6 production QA;
- F0.4/F0.5 prerequisite chain;
- project NotebookLM protocol;
- public-repository/copyright policy;
- canonical F0.6/F0.7 curriculum boundary.

---

## 2. Corpus-size and auditability gate — PASS

The initial corpus contains exactly **eight sources**:

1. canonical F0.6 lesson — `CORE`;
2. ASA Statement on p-values 2016 — `CORE`;
3. FDA Multiple Endpoints Guidance 2022 — `CORE`;
4. Lakens 2022 Sample Size Justification — `CORE`;
5. Greenland et al. 2016 — `SUPPORT`;
6. Heinsberg & Weeks 2022 — `SUPPORT`;
7. CONSORT 2025 — `SUPPORT`;
8. ASA Task Force 2021 — `CONTRAST`.

### Why these eight

The package requires distinct external functions:

- p-value/threshold/transparency safeguards — ASA 2016;
- multiplicity and endpoint-family architecture — FDA 2022;
- sample-size rationale and effect/precision goals — Lakens 2022;
- probability-reversal/error-rate interpretation — Greenland et al.;
- focused observed-power misuse correction — Heinsberg & Weeks;
- registration/protocol/SAP/deviation audit trail — CONSORT 2025;
- balanced contrast against categorical p-value abolition — ASA Task Force 2021.

The canonical lesson integrates those functions into the ten-field F0.6 audit.

No additional power textbook, multiplicity catalog or trial-reporting guideline is required for first-pass mastery. Eight sources remain small enough to audit while covering the module's non-redundant objectives.

---

## 3. Source/link/version verification — PASS

Verification date: `2026-09-09`.

### Canonical F0.6 lesson

Verified on canonical `main` with production state `APPROVED`.

### ASA Statement on p-values — 2016

Official ASA PDF remains accessible at:

`https://www.amstat.org/asa/files/pdfs/P-ValueStatement.pdf`

Verified:

- document dated March 7, 2016;
- explicitly presents six principles;
- p-values are model-conditional;
- p-values do not provide probability that a hypothesis is true;
- conclusions should not rely only on threshold crossing;
- proper inference requires full reporting/transparency;
- statistical significance does not measure effect size/importance;
- p-value alone is not a sufficient evidence summary.

F0.6 uses the threshold/transparency/selective-analysis boundary and preserves the full F0.5 interpretation safeguards.

### FDA Multiple Endpoints Guidance — 2022

Current official FDA page remains accessible at:

`https://www.fda.gov/regulatory-information/search-fda-guidance-documents/multiple-endpoints-clinical-trials`

Verified:

- status remains **Final Guidance**;
- dated October 2022;
- FDA states that increasing the number of endpoints can increase the likelihood of false conclusions if multiplicity is not appropriately addressed;
- guidance addresses grouping/ordering endpoints and statistical multiplicity-management strategies.

Use limitation is explicit: this is regulatory guidance for drug/biologic trials. The package transfers inferential concepts, not universal regulatory obligations to sports/exercise research.

### Lakens 2022 — Sample Size Justification

Current University of California Press article remains accessible at:

`https://online.ucpress.edu/collabra/article/8/1/33267/120491/Sample-Size-Justification`

Verified:

- published in 2022, Collabra: Psychology 8(1):33267;
- article frames sample-size justification as a design decision based on what researchers want to learn;
- supports multiple defensible approaches rather than one universal sample-size convention;
- distinguishes inferential goals such as prospective power and accuracy/precision;
- smallest effects of interest can inform planning.

The package does not convert any single target-power convention into a universal adequacy rule.

### Greenland et al. 2016

Open-access PMC article remains accessible at:

`https://pmc.ncbi.nlm.nih.gov/articles/PMC4877414/`

Verified:

- DOI `10.1007/s10654-016-0149-3`;
- article explicitly catalogs misinterpretations of p-values, confidence intervals and power;
- warns against probability reversals;
- notes that unstated/violated analysis protocols and selection of analyses by p-value can distort interpretation.

F0.6 uses it for conditional/repeated-use reasoning and analytical-selection safeguards.

### Heinsberg & Weeks 2022

Open-access PMC article remains accessible at:

`https://pmc.ncbi.nlm.nih.gov/articles/PMC9452450/`

Verified:

- final publication: Genetic Epidemiology. 2022;46(7):390-394;
- DOI `10.1002/gepi.22464`;
- article states that post hoc power estimates calculated after a study are misleading/not informative for data interpretation;
- simulation/heuristic argument shows post hoc power is tied to observed results and adds no independent interpretation;
- prospective power remains useful for study design/sample-size determination.

The package uses this source only for the observed-power problem it directly addresses.

### CONSORT 2025

Current BMJ statement remains accessible at:

`https://www.bmj.com/content/389/bmj-2024-081123`

Verified:

- CONSORT 2025 is the current general statement and supersedes CONSORT 2010;
- consists of a 30-item checklist;
- open-science section includes trial registration and access to trial protocol/SAP;
- checklist/reporting guidance requires important changes after trial commencement, including non-prespecified outcomes/analyses, to be reported;
- statement emphasizes transparent reporting needed to evaluate trials.

The package explicitly prevents the misuse `CONSORT-complete = low risk of bias`.

### ASA Task Force 2021

Current ASA-hosted page remains accessible at:

`https://magazine.amstat.org/blog/2021/08/01/task-force-statement-p-value/`

Verified:

- task force states that properly applied/interpreted p-values and significance tests are useful tools that should not simply be abandoned;
- emphasizes uncertainty, variability, multiplicity and replicability;
- identifies poor design/conduct, insufficient data, model choice, inadequate analysis description and selective reporting as threats to replicability;
- notes that multiplicity adjustment can mitigate selective-result problems in some settings.

The package uses this as a contrast source, not as permission for threshold ritualism.

### Source-change decision

No source-version or access change found on 2026-09-09 requires modification of the approved F0.6 lesson.

---

## 4. Role-assignment QA — PASS

### `CORE` — canonical lesson

Function:

- exact F0.6 vocabulary and sequence;
- Type I/II and power definitions;
- worked FWER and observed-power examples;
- sample-size reasoning;
- analytical-flexibility framework;
- ten-field audit;
- critical fails and F0.7 boundary.

Limitation: project-authored instructional source.

### `CORE` — ASA 2016

Function:

- model-conditional p-value reasoning;
- threshold safeguards;
- full reporting/transparency;
- effect-size/importance separation.

Limitation: not a complete power/multiplicity manual.

### `CORE` — FDA 2022

Function:

- multiple-endpoint false-conclusion problem;
- family/grouping/ordering concepts;
- multiplicity-management architecture.

Limitation: regulatory scope.

### `CORE` — Lakens 2022

Function:

- sample-size justification by inferential goal;
- a-priori power versus desired precision;
- smallest-effect planning and transparent constraints.

Limitation: broad review, not a universal power target prescription.

### `SUPPORT` — Greenland et al.

Function:

- probability-reversal repair;
- conditional error-rate interpretation;
- analysis-selection caution.

Limitation: broad critical tutorial.

### `SUPPORT` — Heinsberg & Weeks

Function:

- focused rejection of observed/post hoc power for completed-study interpretation.

Limitation: narrow methodological commentary/simulation.

### `SUPPORT` — CONSORT 2025

Function:

- registration/protocol/SAP/deviation auditability;
- prespecified versus post hoc transparency.

Limitation: reporting guideline, not validity certification.

### `CONTRAST` — ASA Task Force 2021

Function:

- prevent overcorrection to categorical p-value abandonment;
- connect p-values to broader uncertainty/multiplicity/replicability practice.

Limitation: high-level statement rather than technical manual.

Each source has a distinct instructional role.

---

## 5. Required F0-A13 coverage — PASS

### Type I/alpha versus Type II/beta

Passes 1–2 require repeated-use definitions and reject posterior-probability wording.

### Power definition and effect dependence

Passes 2–3 require a specified effect/design/model and explicitly reject `power=P(H1 true)`.

### `1-power` critical fail

Pass 2 and the critical-fail section explicitly reject `1-power=P(this result is a false negative)`.

### Prospective power versus observed precision

Pass 4 requires completed-study interpretation through estimate/CI/practical threshold.

### Observed/post hoc power

Pass 5 uses Heinsberg & Weeks directly and requires replacing observed-power rescue with CI-based interpretation.

### Sample-size justification

Passes 6–7 compare a-priori power, desired precision, near-census, resource constraints and planning-effect justification.

### Effective family of hypotheses

Pass 9 makes the learner reconstruct intended confirmatory claims before selecting any multiplicity strategy.

### FWER illustration

Pass 8 requires `1-.95^m` calculations only under explicit independent-test/all-null assumptions and requires a non-universality warning.

### Endpoint hierarchy / alpha allocation

Pass 10 covers conceptual strategies and one simple Bonferroni illustration without creating an exhaustive correction catalog.

### Hypothesis versus analytical-path multiplicity

Pass 11 requires explicit separation of scientific hypotheses from model/outlier/covariate paths.

### Subgroup/secondary analyses

Passes 9, 10, 12 and 15 audit secondary and subgroup claims and reject significance-label comparison as interaction proof.

### Researcher degrees of freedom

Pass 13 covers outcome definitions, time windows, exclusions, missing-data rules, transformations, covariates, subgroups, models, stopping and reporting choices.

### Registration/preregistration/protocol/SAP

Pass 14 distinguishes each document and requires timing/version/deviation checks.

### Preregistration limitation

Pass 14 and critical fails explicitly reject `preregistered = low risk of bias`.

### Confirmatory versus exploratory

Pass 15 preserves exploratory value while blocking undisclosed relabeling.

### F0.5 continuity

Pass 4, integrated audit field 8 and the completion standard require magnitude + CI + practical threshold for completed-study interpretation.

### Integrated synthetic audit

Pass 17 plus Section 5 uses the required many-outcome/timepoint/subgroup/model scenario and requires all ten F0.6 audit fields.

### F0.7 boundary

Section 9 explicitly defers systematic-review/meta-analysis/heterogeneity/I2/publication-bias machinery.

---

## 6. Answer-leakage and prerequisite control — PASS

Excluded from initial NotebookLM corpus:

- F0.6 `EXERCISES.md`;
- F0.6 `ANSWER_KEY.md`;
- F0.6 production `QA_REPORT.md`;
- F0.4 `ENTRY_DIAGNOSTIC.md`;
- full `SOURCE_INDEX.md`.

The study guide requires independent assessment only after closing NotebookLM and prohibits answer-key consultation before the first attempt.

F0.4 diagnostic remains `UNOBSERVED`; package creation does not create diagnostic evidence.

---

## 7. Scientific-boundary QA — PASS

The package preserves these safeguards:

- alpha ≠ posterior probability of H0;
- beta/power are effect/design conditional;
- power ≠ P(H1 true);
- `1-power` ≠ posterior false-negative probability;
- high prospective power ≠ valid/bias-free study;
- observed power based on observed effect ≠ independent result interpretation;
- completed-study uncertainty is read from estimate/CI, not reconstructed through observed power;
- sample-size justification follows inferential goal rather than one universal convention;
- planning effect/SESOI is independently justified;
- many nominal .05 tests do not automatically preserve family-level confirmatory error control;
- independent-test FWER arithmetic is not generalized to correlated tests;
- family definition follows claims/decision strategy;
- alternative models are not mechanically counted as independent hypotheses;
- significance in one subgroup but not another does not establish interaction;
- prespecification improves auditability but does not certify validity;
- exploratory findings are not treated as inherently invalid;
- CONSORT is not a risk-of-bias score;
- FDA guidance is not generalized as universal sports-science regulation;
- synthetic sports/nutrition examples remain methodological examples only.

---

## 8. Pedagogical QA — PASS

The sequence progresses from:

`Type I/alpha → Type II/beta/power → power curve → power vs precision → observed-power trap → sample-size goals → planning effect → multiplicity/FWER → family reconstruction → control concepts → analytical paths → subgroup interaction → degrees of freedom → registration/protocol/SAP → confirmatory/exploratory → integrated audit`

This order preserves F0.5 rather than replacing it.

The package repeatedly requires:

- explanation in learner language;
- prediction;
- calculation;
- misconception repair;
- document/timestamp auditing;
- classification of confirmatory/exploratory outputs;
- integrated transfer to unfamiliar studies.

No pass can be completed by terminology recognition alone.

---

## 9. Copyright/public-repository QA — PASS

- no third-party PDF/article/chapter was committed into GitHub;
- only project-authored Markdown, citations and links were added;
- open-access PMC articles are linked rather than copied;
- ASA PDF, FDA guidance and BMJ CONSORT are linked rather than redistributed;
- no learner personal/health data;
- no substantive nutrition recommendation from synthetic examples.

---

## 10. Production/learning-state separation — PASS

After F0-A13 package production:

- F0.1 learner state remains pending/unvalidated;
- F0.2 remains pending/unvalidated;
- F0.3 remains pending/unvalidated;
- F0.4 remains pending/unvalidated;
- F0.4 quantitative diagnostic remains `UNOBSERVED`;
- F0.5 remains pending/unvalidated;
- F0.6 remains `UNSEEN`/unvalidated;
- no module is promoted from production activity.

---

## 11. Final gate

> Can a learner with F0.4/F0.5 prerequisites use the controlled corpus to define Type I/II error and power without probability reversal; distinguish prospective power from observed precision; reject observed-power misuse; justify sample size by inferential goal; reconstruct effective hypothesis families and analytical paths; reason about multiplicity and subgroup claims; audit registration/protocol/SAP timing; separate confirmatory from exploratory outputs; and complete the ten-field F0.6 study audit while preserving estimate/CI interpretation?

**Decision:** yes.

**Package decision:** `PASS — READY_FOR_STUDY`.
