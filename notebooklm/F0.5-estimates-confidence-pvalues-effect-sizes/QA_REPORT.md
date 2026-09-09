# F0.5 — NotebookLM Study Package QA Report

**Module:** `F0.5 — Estimates, confidence intervals, p-values, effect sizes and practical relevance`
**Package version:** `1`
**Reviewed:** `2026-09-09`
**Package decision:** `PASS — READY_FOR_STUDY`
**Learner-state change:** none
**F0.4 quantitative diagnostic change:** none; remains `UNOBSERVED`

This report records QA of the NotebookLM package only. It does not record that the learner studied F0.5 and does not authorize any mastery-state transition.

---

## 1. Package contents — PASS

Required files:

- `notebooklm/F0.5-estimates-confidence-pvalues-effect-sizes/MANIFEST.md`;
- `notebooklm/F0.5-estimates-confidence-pvalues-effect-sizes/STUDY_GUIDE.md`;
- `notebooklm/F0.5-estimates-confidence-pvalues-effect-sizes/QA_REPORT.md`.

The package is aligned to:

- approved canonical F0.5 lesson;
- F0.5 production QA;
- F0.4 prerequisite distinction SD versus SE;
- project NotebookLM protocol;
- canonical F0.5/F0.6 curriculum boundary.

---

## 2. Corpus-size and auditability gate — PASS

The initial corpus contains exactly **six sources**:

1. canonical F0.5 lesson — `CORE`;
2. Cochrane Handbook Chapter 6 — `CORE`;
3. ASA Statement on p-values — `CORE`;
4. Greenland et al. 2016 — `SUPPORT`;
5. Lakens 2022 — `SUPPORT`;
6. ASA Task Force 2021 — `CONTRAST`.

### Why these six

The package needs only three external functions:

- effect-measure scale logic — Cochrane;
- correct p-value/CI interpretation and error repair — ASA + Greenland;
- practical threshold/informativeness reasoning — Lakens;
- balanced contrast preventing the false lesson that p-values are intrinsically useless — ASA Task Force 2021.

The canonical lesson integrates these sources into one coherent F0.5 interpretation workflow.

NIST and Altman/Bland remain useful registered sources but are not required in the first-pass NotebookLM corpus because the canonical lesson already carries the F0.4 SD/SE bridge and Greenland provides the needed CI interpretation safeguard. This keeps retrieval compact.

---

## 3. Source/link/version verification — PASS

Verification date: `2026-09-09`.

### Canonical F0.5 lesson

Verified on canonical `main` with production state `APPROVED`.

### Cochrane Chapter 6

Current official chapter verified at:

`https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-06`

Verified facts:

- title remains *Choosing effect measures and computing estimates of effect*;
- chapter belongs to Cochrane Handbook version 6.5 (2024);
- page states last updated August 2023;
- key points distinguish MD/SMD for continuous outcomes and RD/RR/OR for dichotomous outcomes;
- difference measures have null 0 and ratio measures null 1;
- ratio measures are commonly analysed/displayed on log scales;
- effect estimates should be accompanied by uncertainty such as CI or SE.

Use is restricted to effect-measure interpretation relevant to F0.5.

### ASA Statement on p-values

Official ASA PDF remains accessible at:

`https://www.amstat.org/asa/files/pdfs/P-ValueStatement.pdf`

All six principles were rechecked:

1. p-values can indicate incompatibility with a specified statistical model;
2. p-values do not provide the probability that the hypothesis is true or that random chance alone produced the data;
3. scientific conclusions should not depend only on crossing a threshold;
4. proper inference requires full reporting and transparency;
5. p-value/statistical significance does not measure effect magnitude or importance;
6. p-value alone is not a sufficient measure of evidence regarding a model/hypothesis.

The package requires paraphrase/application rather than rote quotation.

### Greenland et al. 2016

Verified open-access PMC article:

`https://pmc.ncbi.nlm.nih.gov/articles/PMC4877414/`

- DOI `10.1007/s10654-016-0149-3`;
- PMCID `PMC4877414`;
- CC BY 4.0;
- explicitly catalogs common p-value/CI/power misinterpretations;
- supports repeated-sampling CI coverage and warns against posterior-probability reversal;
- emphasizes effect estimates/confidence limits over binary significance classification.

Power material is deliberately excluded from F0.5 study tasks.

### Lakens 2022

Verified current University of California Press article:

`https://online.ucpress.edu/collabra/article/8/1/33267/120491/Sample-Size-Justification`

The article explicitly states that a smallest effect size of interest should be justified from theory or practical implications rather than merely stated.

F0.5 uses only this threshold/informativeness concept; formal sample-size/power planning remains F0.6.

### ASA Task Force 2021

Verified current ASA-hosted page:

`https://magazine.amstat.org/blog/2021/08/01/task-force-statement-p-value/`

The statement explicitly clarifies that properly applied/interpreted p-values and significance tests remain useful tools that should not simply be abandoned, while uncertainty, variability, multiplicity, replicability, design and reporting context remain essential.

F0.5 uses this as a contrast source, not as a license for threshold ritualism.

No source-version change found on 2026-09-09 requires modification of the approved F0.5 lesson.

---

## 4. Role-assignment QA — PASS

### `CORE` — canonical lesson

Function:

- exact F0.5 vocabulary and interpretation sequence;
- worked synthetic examples;
- SD/SE bridge;
- practical-threshold reasoning;
- forest/trial application;
- F0.6 scope boundary.

Limitation: project-authored instructional source.

### `CORE` — Cochrane Chapter 6

Function:

- MD/SMD/RD/RR/OR definitions;
- difference versus ratio logic;
- null values;
- log-scale intuition;
- uncertainty accompanying effect estimates.

Limitation: evidence-synthesis context and methods beyond F0.5.

### `CORE` — ASA 2016

Function:

- six p-value principles;
- threshold and effect-importance safeguards;
- transparency principle.

Limitation: not a complete CI/effect-measure manual.

### `SUPPORT` — Greenland et al.

Function:

- explicit misconception repair;
- CI repeated-sampling meaning;
- compatibility framing;
- p-value probability-reversal traps.

Limitation: includes power material outside scope.

### `SUPPORT` — Lakens

Function:

- smallest-effect/decision-relevance reasoning.

Limitation: broader sample-size/power focus deferred to F0.6.

### `CONTRAST` — ASA Task Force 2021

Function:

- prevent overcorrection from “p<0.05 decides truth” to “p-values are useless”;
- locate p-values within uncertainty and broader statistical practice.

Limitation: high-level statement, not technical instruction.

Each source has a distinct non-redundant role.

---

## 5. Required F0-A11 coverage — PASS

### Six-block sequence

Every major applied pass requires:

`Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`

### Frequentist CI

Pass 2 explicitly blocks posterior-probability language and requires repeated-sampling coverage interpretation.

### Six ASA principles

Pass 3 requires all six principles plus repair of false statements.

### MD/SMD

Pass 5 requires choosing/calculating MD or SMD and explicitly rejects universal SMD importance labels.

### RD/RR/OR

Pass 6 requires calculation and interpretation of all three while preserving RR ≠ OR.

### Absolute baseline context

Pass 7 repeatedly uses the same RR at different baselines and requires absolute RD comparison.

### Smallest-effect/threshold reasoning

Pass 8 distinguishes intervals entirely meaningful, entirely trivial, spanning multiple zones and precise near-null exclusion.

### Forest-plot-row practice

Pass 10 includes difference and ratio scales, varied precision and practical thresholds.

### Synthetic trial-table practice

Pass 11 includes continuous and binary tables and requires full six-block interpretation.

### SD versus SE bridge

Passes 1–2 preserve SE as precision/sampling variability of an estimate and never as individual spread.

### F0.6 boundary

The guide explicitly stops formal alpha/beta, power, multiplicity, FWER/FDR and analytical-flexibility machinery.

---

## 6. Answer-leakage and prerequisite control — PASS

Excluded from initial NotebookLM corpus:

- F0.5 `EXERCISES.md`;
- F0.5 `ANSWER_KEY.md`;
- F0.5 production `QA_REPORT.md`;
- F0.4 `ENTRY_DIAGNOSTIC.md`;
- full `SOURCE_INDEX.md`.

The study guide instructs the learner to complete independent assessment only after closing NotebookLM and to consult the answer key only after a first attempt.

The F0.4 quantitative diagnostic remains `UNOBSERVED`; package creation does not create diagnostic evidence.

---

## 7. Scientific-boundary QA — PASS

The package preserves these safeguards:

- frequentist CI ≠ posterior credible interval;
- CI precision ≠ causal validity;
- p-value ≠ P(H0|data);
- p<0.05 ≠ truth/importance;
- p>0.05 ≠ proof of no effect;
- p=0.049 and 0.051 are not automatic opposite scientific conclusions;
- SMD labels are not universal practical thresholds;
- RR ≠ OR;
- relative effects require baseline context for practical interpretation;
- crossing/excluding null is not the whole CI interpretation;
- wide intervals can remain compatible with meaningful benefit/harm;
- narrow near-null intervals can be informative if meaningful effects are excluded;
- systematic bias and applicability are not repaired by statistical precision;
- synthetic sports/nutrition examples remain methodological examples only.

---

## 8. Pedagogical QA — PASS

The study sequence progresses from:

`statistical object → CI meaning → p-value principles → joint p/CI interpretation → continuous effect measures → binary effect measures → absolute/relative context → practical thresholds → log-ratio intuition → forest plots → trial tables → balanced synthesis`

This prevents threshold-first learning.

The package repeatedly requires explanation, calculation, misconception repair and integrated interpretation rather than passive source summarization.

---

## 9. Copyright/public-repository QA — PASS

- no third-party PDF/article/chapter was committed into GitHub;
- only project-authored Markdown, citations and links were added;
- Greenland et al. open-access status is recorded but the article itself is linked rather than copied;
- no learner personal/health data;
- no substantive nutrition recommendation from synthetic examples.

---

## 10. Production/learning-state separation — PASS

After F0-A11 package production:

- F0.1 learner state remains pending/unvalidated;
- F0.2 remains pending/unvalidated;
- F0.3 remains pending/unvalidated;
- F0.4 remains pending/unvalidated;
- F0.4 quantitative diagnostic remains `UNOBSERVED`;
- F0.5 remains `UNSEEN`/unvalidated;
- no module is promoted from production activity.

---

## 11. Final gate

> Can a learner with the F0.4 prerequisite use the controlled corpus to interpret unfamiliar estimates, CIs, p-values and common effect measures; reject probability/significance shortcuts; integrate practical thresholds and baseline effects; and produce a bounded six-block conclusion without importing F0.6 machinery?

**Decision:** yes.

**Package decision:** `PASS — READY_FOR_STUDY`.