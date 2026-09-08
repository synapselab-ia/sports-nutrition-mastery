# F0.1 — Practical NotebookLM Study Guide

**Package version:** `1`
**Module:** `F0.1 — Scientific questions, hypotheses and operationalization`
**Current learner state:** `UNSEEN`

This guide tells the learner exactly how to build and use the approved NotebookLM corpus. Completing these setup steps does **not** change mastery state. Learning-state changes require observed study/assessment evidence.

## 1. Create the notebook

Create one NotebookLM notebook named:

`Sports Nutrition Mastery — F0.1 Scientific Questions`

Do not mix F0.2+ sources into this notebook yet. The point is to keep the corpus small enough that every answer can be audited against the intended sources.

## 2. Add the initial source corpus

Add the following **six** sources and no others for the first pass.

### Source 1 — canonical lesson — CORE

Repository file:

`foundations/F0-scientific-literacy/F0.1-scientific-questions/LESSON.md`

Preferred source URL for NotebookLM:

`https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.1-scientific-questions/LESSON.md`

If NotebookLM does not accept the raw URL, open/download that Markdown file from GitHub and upload the file itself. Do not substitute an AI-generated summary for the lesson.

### Source 2 — Cochrane question framing — CORE

Add as website:

`https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-02`

Use it for:

- why question formulation precedes evidence selection;
- explicit PICO elements;
- why question scope constrains what evidence is relevant.

Do not treat the entire Cochrane Handbook as required reading for F0.1.

### Source 3 — ICH E9 / E9(R1) estimand framework — CORE

Official landing page:

`https://www.ema.europa.eu/en/ich-e9-statistical-principles-clinical-trials-scientific-guideline`

Add the EMA page. For stronger source capture, also use the current **ICH E9(R1) Step 5 addendum PDF** linked under “Current version” on that page if NotebookLM permits direct PDF URL ingestion or after downloading it from EMA.

Focus only on:

- scientific question of interest;
- estimand as the target quantity/effect to be estimated;
- population;
- treatment/conditions compared;
- variable/outcome;
- intercurrent events concept;
- population-level summary;
- the principle that the estimator should not redefine the scientific question.

Do not try to master the full regulatory/statistical document in F0.1.

### Source 4 — GRADE Book: answerable questions — CORE

Add as website:

`https://book.gradepro.org/`

Navigate/use the chapter family **“Making answerable questions.”**

Use it for:

- structuring explicit decision/research questions;
- making population, intervention/exposure, comparator and outcomes visible;
- understanding that a question defines which evidence can answer it.

The site is a living JavaScript application. If NotebookLM cannot ingest the page reliably, keep the official page open as a manual reference rather than importing an unofficial copy or scraper.

### Source 5 — CONSORT 2025 — SUPPORT

Add as website:

`https://www.bmj.com/content/389/bmj-2024-081123`

Use it for:

- transparent objectives/questions;
- explicit outcomes and timing;
- visibility of protocol/registration/statistical-analysis-plan information;
- distinguishing planned from undeclared post-hoc changes.

**Do not ask NotebookLM to score study quality with CONSORT.** CONSORT is a reporting guideline, not a risk-of-bias instrument.

### Source 6 — Areta et al. 2013 full text — CONTRAST / TRANSFER

Add the free full-text PMC page:

`https://pmc.ncbi.nlm.nih.gov/articles/PMC3650697/`

Use it only as a concrete sports-nutrition transfer case for:

- reconstructing the empirical question;
- distinguishing construct from operational outcome;
- identifying population, feeding conditions and time window;
- detecting extrapolation from acute myofibrillar protein synthesis to months-long hypertrophy/performance claims.

Do not convert this single acute experiment into a practical universal protein-timing recommendation.

## 3. Do NOT add these yet

Keep these repository files outside NotebookLM during the first study pass:

- `ANSWER_KEY.md` — prevents answer leakage;
- `EXERCISES.md` — the final first-pass assessment should be answered independently;
- `QA_REPORT.md` — production metadata, not study evidence;
- `SOURCE_INDEX.md` — registry metadata would add noise to this small corpus.

The approved corpus is defined in `MANIFEST.md`. Do not let NotebookLM discover/import random web results to “complete” the corpus.

## 4. Study sequence

Follow this order. Do not jump directly to the Areta article.

### Pass 1 — build the conceptual skeleton from the lesson

Read/study `LESSON.md` first.

Then ask NotebookLM:

> Based only on the F0.1 lesson, build a concept map connecting: claim → scientific question → population → contrast → construct → operational definition → variable/outcome → time → estimand → interpretation boundary. Define every node and show where people commonly confuse adjacent concepts.

Audit the output against the lesson. If NotebookLM adds a concept unsupported by the approved sources, do not treat it as canonical.

### Pass 2 — question framing with Cochrane + GRADE

Ask:

> Compare how the Cochrane Handbook and GRADE Book make broad questions answerable. What do they agree must become explicit? Where is PICO useful, and why should PICO not be treated as a mechanical quality checklist?

Then, without asking NotebookLM for the answer first, transform these claims yourself:

- “Creatine improves performance.”
- “Carbohydrate prevents fatigue.”
- “Protein after training maximizes recovery.”

For each, write population, intervention/exposure, comparator, operational outcome and time.

Only after writing your version, ask NotebookLM to critique it source-by-source.

### Pass 3 — estimand thinking with ICH E9(R1)

Ask:

> Teach the F0.1-level estimand concept using ICH E9(R1), but stop before advanced estimator/statistical-analysis detail. Explain why the scientific question and target quantity should be defined before choosing an analysis.

Then create one estimand for a hypothetical sports-nutrition question using:

1. target population;
2. conditions compared;
3. variable/outcome;
4. time window;
5. one relevant intercurrent event and how the question conceptually handles it;
6. population-level contrast/summary.

Finally ask NotebookLM to identify any ambiguity still present.

### Pass 4 — confirmatory versus exploratory with CONSORT

Ask:

> Using CONSORT 2025 and the F0.1 lesson, explain how a reader can distinguish what investigators planned from what may have been discovered after seeing the data. Do not treat CONSORT as a risk-of-bias score.

Create two examples yourself:

- one legitimate exploratory finding correctly labeled;
- the same finding rewritten misleadingly as though it were prespecified confirmation.

Ask NotebookLM to explain exactly what changed in the evidential claim.

### Pass 5 — transfer to a real sports-nutrition paper

Read the methods/results-relevant portions of Areta et al. 2013.

Before asking NotebookLM anything, write:

- target/sample population;
- conditions compared;
- total protein/source;
- construct of interest;
- exact operational outcome(s) relevant to the F0.1 exercise;
- measurement window;
- one introductory target quantity/estimand;
- four conclusions the paper does **not** directly establish.

Then use this prompt:

> Audit my reconstruction against the Areta paper. For every correction, cite the paper itself. Separate what the experiment actually measured from any long-term hypertrophy, strength, performance, female, older-adult, other-sport, other-protein-source or other-total-dose extrapolation. If the paper does not clearly establish a primary/secondary hierarchy, say that rather than inventing one.

### Pass 6 — Socratic retrieval

Use this exact instruction:

> Act as an examiner for F0.1. Ask one question at a time and wait for my answer. Do not reveal the answer before I respond. Alternate among definitions, examples, counterexamples, question reformulation, estimand construction, exploratory-versus-confirmatory classification and inferential-boundary critique. After each answer, grade it as Correct / Partly correct / Incorrect, explain the missing reasoning using citations to the approved sources, and keep a temporary list of recurring errors. Do not advance to F0.2 topics.

Continue until the learner can answer the core concepts without relying on NotebookLM to generate the initial response.

## 5. Independent assessment outside NotebookLM

After the study sequence:

1. open `foundations/F0-scientific-literacy/F0.1-scientific-questions/EXERCISES.md`;
2. answer all Parts A–F **without consulting NotebookLM or the answer key**;
3. save your answers outside the public repository if they contain any personal material; ordinary academic answers can be shared in chat for grading;
4. only after the first attempt, open `ANSWER_KEY.md` or submit the answers to the project assistant for correction;
5. use the canonical scoring rule: `>=80/100` and no critical fail permits progression evidence, but does not equal `MASTERED`;
6. any critical fail requires targeted repair even if the numerical score is high.

### Critical fails from the canonical assessment

- treating an acute biomarker/mechanistic outcome as automatic proof of a chronic applied outcome;
- presenting a post-hoc analysis as a prespecified confirmatory hypothesis;
- inability to distinguish construct from operational definition;
- inability to formulate a question with an identifiable outcome or contrast.

## 6. What to send back to ChatGPT after study

To let the canonical project update learning state honestly, provide either:

- your completed `EXERCISES.md` answers; or
- a statement that the lesson/NotebookLM study sequence was completed **plus** your answers to a fresh assessment administered in chat.

Do not merely say “I understood everything” if you want the project to record a competence state. The mastery protocol requires observed performance.

## 7. When NotebookLM disagrees with the repository

Use this order of authority:

1. inspect the exact approved external source;
2. inspect the current repository lesson/manifest;
3. if the repository is demonstrably wrong or outdated, research and update GitHub;
4. do not silently overwrite canonical project knowledge because NotebookLM generated a confident answer.

## 8. Package completion criterion

The F0.1 NotebookLM package is correctly set up when:

- the six approved sources are the only initial corpus sources;
- the learner can identify which source supports each methodological point;
- the answer key has not contaminated the first retrieval attempt;
- Areta et al. is used as a boundary/transfer case rather than a universal recommendation;
- active recall occurs before answer exposure;
- the independent F0.1 assessment remains outside the initial NotebookLM corpus.
