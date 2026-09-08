# F0.1 — NotebookLM Study Package QA

**Package:** `notebooklm/F0.1-scientific-questions/`
**Manifest version:** `1`
**QA date:** `2026-09-08`
**Result:** `PASS — STUDY_PACKAGE_READY`
**Learner-state change:** none

## 1. Package artifacts

Verified package artifacts:

- `MANIFEST.md` — approved corpus, priorities, concepts/claims, limits, retrieval/integration prompts and evidence-critique task;
- `STUDY_GUIDE.md` — exact NotebookLM source setup and study sequence;
- this `QA_REPORT.md`.

Referenced canonical F0.1 artifacts verified in the repository:

- `foundations/F0-scientific-literacy/F0.1-scientific-questions/LESSON.md`;
- `foundations/F0-scientific-literacy/F0.1-scientific-questions/EXERCISES.md`;
- `foundations/F0-scientific-literacy/F0.1-scientific-questions/ANSWER_KEY.md`;
- `foundations/F0-scientific-literacy/F0.1-scientific-questions/QA_REPORT.md`;
- `foundations/F0-scientific-literacy/SOURCE_INDEX.md`.

## 2. Approved initial NotebookLM corpus

Initial corpus size: **6 sources**.

| Source | Priority | Function | QA judgment |
|---|---|---|---|
| canonical `LESSON.md` | CORE | instructional spine | PASS |
| Cochrane Handbook v6.5, Chapter 2 | CORE | answerable question/PICO framing | PASS |
| ICH E9 / E9(R1) | CORE | estimand/target-question framework | PASS |
| GRADE Book — Making answerable questions | CORE | structured question framing | PASS with ingestion caveat |
| CONSORT 2025 | SUPPORT | transparent objectives/outcomes/prespecification reporting | PASS |
| Areta et al. 2013 full text | CONTRAST | real sports-nutrition transfer/inferential-boundary case | PASS |

The corpus is intentionally smaller than the complete F0 source index. No F0.2+ source is imported merely for comprehensiveness.

## 3. External-link verification

Links were checked on `2026-09-08`.

### Cochrane Handbook

`https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-02`

Status: **verified**. The current Handbook identifies version 6.5 (2024); Chapter 2 explicitly covers determining scope/questions and explains that well-formulated questions guide eligibility, data collection, synthesis and presentation. PICO is explicitly used for intervention questions.

### EMA / ICH E9 and E9(R1)

`https://www.ema.europa.eu/en/ich-e9-statistical-principles-clinical-trials-scientific-guideline`

Status: **verified**. The page exposes the current ICH E9 document and the Step 5 E9(R1) addendum on estimands/sensitivity analysis. The addendum describes the framework aligning scientific question, estimand, planning, conduct, analysis and interpretation.

### GRADE Book

`https://book.gradepro.org/`

Status: **verified as current official living resource**. The site exposes the “Making answerable questions” chapter family and identifies the GRADE Book as the comprehensive current official GRADE resource.

Ingestion caveat: the site is a JavaScript application. Browser/search indexing can resolve its content, but NotebookLM URL ingestion may vary. `STUDY_GUIDE.md` therefore instructs the learner to keep the official page as a manual reference rather than importing an unofficial reproduction if ingestion fails.

### CONSORT 2025

`https://www.bmj.com/content/389/bmj-2024-081123`

Status: **verified**. BMJ hosts the CONSORT 2025 statement, and the joint CONSORT-SPIRIT site confirms the 2025 published statement. The package preserves the canonical distinction: CONSORT supports reporting transparency and is **not** used as a risk-of-bias/quality score.

### Areta et al. 2013

`https://pmc.ncbi.nlm.nih.gov/articles/PMC3650697/`

Status: **verified** as a free full-text PMC article. PubMed/PMC metadata match DOI `10.1113/jphysiol.2012.244897` and the registered `F0-S21` citation.

### Canonical lesson raw URL

`https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.1-scientific-questions/LESSON.md`

Status: **verified by canonical repository path/blob existence**. The study guide provides file-upload fallback if NotebookLM does not accept the raw URL.

## 4. Study Package QA checklist

### Sources in manifest exist and are intended

**PASS.** All internal files exist in `main`; every external source was independently resolved/verified. The six-source set matches F0.1 rather than the whole F0 bibliography.

### Priority/function explained

**PASS.** Every source is labeled `CORE`, `SUPPORT` or `CONTRAST`, with an explicit reason for inclusion.

### Questions cover concept, mechanism, critique and integration

**PASS.** Manifest prompts include:

- basic retrieval/definitions;
- mechanisms of interpretive failure (operationalization, prespecification, estimand-before-estimator);
- source-specific evidence critique;
- transfer/integration from popular claims to explicit target quantities.

### Evidence-critique task present

**PASS.** `F0-S21` is used for a constrained full-text exercise requiring reconstruction of the actual question/outcome/time boundary and explicit identification of unsupported extrapolations.

### Answer leakage controlled

**PASS.** `ANSWER_KEY.md` is excluded from the initial corpus. `EXERCISES.md` is kept outside NotebookLM for the independent first attempt.

### Copyright/public-repository compliance

**PASS.** No third-party PDF or article text was copied into the repository. The package contains only citations, links, project-authored instructions and project-authored lesson material. The Areta full text is referenced via PMC rather than mirrored.

### Version correspondence

**PASS.** Manifest v1 references the current approved F0.1 lesson and the current registered `F0-S01`, `F0-S05`, `F0-S14`, `F0-S15`, `F0-S21` source set as of 2026-09-08.

### Learner mastery separation

**PASS.** Package generation is explicitly recorded as a production state only. F0.1 remains `UNSEEN` until actual study/performance is observed.

## 5. Misuse protections

The package explicitly prevents the following foreseeable errors:

- treating PICO as a universal mechanical quality checklist;
- treating CONSORT as study quality/risk of bias;
- treating ICH regulatory detail as if all of it were required in introductory sports-science appraisal;
- inventing a primary/secondary outcome hierarchy in the Areta paper if the report does not clearly support it;
- treating acute myofibrillar protein synthesis as equivalent to months-long hypertrophy or performance;
- adding random web sources to NotebookLM and allowing them to silently become project authority;
- using the answer key before first retrieval/application.

## 6. Residual limitations

- NotebookLM ingestion behavior for dynamic JavaScript pages such as the GRADE Book is external to this repository and cannot be guaranteed. The official manual-reference fallback is documented.
- Source websites can change. A later material source revision requires manifest version review.
- Passing the package QA demonstrates that the study environment is ready; it does not demonstrate that the learner has studied or learned F0.1.

## 7. Gate decision

`STUDY PACKAGE QA: PASS`

F0.1 may be marked **`STUDY_PACKAGE_READY` in production**.

Learning state remains **`UNSEEN`**.
