# F0.2 — Practical NotebookLM Study Guide

**Package version:** `1`
**Module:** `F0.2 — Study designs and what they can answer`
**Current learner state:** `UNSEEN`

This guide defines exactly how to build and use the approved NotebookLM corpus for F0.2. Completing the setup or reading the sources does **not** change learner state. Progression requires observed performance under the mastery protocol.

## 1. Create the notebook

Create one NotebookLM notebook named:

`Sports Nutrition Mastery — F0.2 Study Designs`

Do not merge the F0.1 notebook into this one. F0.1 is a prerequisite conceptually, but F0.2 needs a compact corpus focused on study architecture and inferential boundaries.

## 2. Add exactly six initial sources

Use only the sources below on the first pass.

### Source 1 — canonical F0.2 lesson — CORE

Repository file:

`foundations/F0-scientific-literacy/F0.2-study-designs/LESSON.md`

Preferred NotebookLM URL:

`https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.2-study-designs/LESSON.md`

Use it as the primary instructional spine for:

- identifying design from architecture;
- origin of the contrast;
- temporal direction;
- between- versus within-subject comparison;
- unit of allocation/observation/analysis;
- randomized parallel/crossover/cluster/factorial designs;
- non-randomized intervention studies;
- cohort/case-control/cross-sectional discrimination;
- acute versus chronic outcomes;
- diagnostic/prognostic questions;
- introductory target-trial thinking;
- strongest defensible inference versus tempting unsupported inference.

If NotebookLM cannot ingest the raw Markdown URL, download/upload the file from GitHub. Do not replace it with an AI summary.

### Source 2 — Cochrane Chapter 23 — CORE

Add as website:

`https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-23`

Use it primarily for:

- cluster-randomized design;
- unit of allocation;
- dependence/clustering among individuals;
- crossover design;
- within-person comparisons;
- suitability of crossover;
- carryover and period effects.

Do **not** try to learn the chapter's full meta-analysis/statistical machinery in F0.2. The goal here is design architecture.

### Source 3 — CONSORT 2025 — SUPPORT

Add as website:

`https://www.bmj.com/content/389/bmj-2024-081123`

Use it to practice extracting from a randomized-trial report:

- who was randomized;
- what conditions were compared;
- outcomes and timing;
- participant flow;
- protocol/registration/SAP visibility;
- other design features needed to reconstruct the trial.

Critical rule:

> CONSORT is a reporting guideline. Do not ask NotebookLM to turn it into a study-quality score or causal-validity checklist.

### Source 4 — factorial trial explanation/elaboration — SUPPORT

Add as website:

`https://www.bmj.com/content/388/bmj-2024-080785`

Use it for:

- what makes a factorial trial factorial;
- identifying factors and treatment combinations;
- main comparisons;
- interaction intuition;
- why factor effects cannot be assumed automatically additive.

Detailed interaction tests, multiplicity and statistical power belong later, especially F0.6.

### Source 5 — STROBE — SUPPORT

Add as website:

`https://www.strobe-statement.org/`

Use it for the three major observational analytical designs:

- cohort;
- case-control;
- cross-sectional.

The purpose is to identify what information distinguishes them. STROBE itself explicitly says its recommendations are for reporting, not prescriptions for design/conduct and not a quality instrument.

### Source 6 — target-trial framework — CONTRAST

Add the free full text:

`https://pmc.ncbi.nlm.nih.gov/articles/PMC11936718/`

Use it for:

- specifying the randomized trial one would ideally run for a causal intervention question;
- eligibility;
- strategies compared;
- treatment assignment concept;
- time zero;
- follow-up;
- outcome;
- causal contrast;
- observational emulation;
- limits of what emulation can create.

Critical rule:

> Target-trial emulation clarifies design. It does not retrospectively randomize observational data.

## 3. Do NOT add these yet

Keep the following outside NotebookLM for the first pass:

- `ANSWER_KEY.md` — prevents answer leakage;
- `EXERCISES.md` — final first-pass assessment must remain independent;
- F0.2 `QA_REPORT.md` — production metadata, not study evidence;
- full `SOURCE_INDEX.md` — registry noise;
- separate crossover and cluster CONSORT extensions — redundant for the initial corpus because Cochrane Chapter 23 plus the canonical lesson already cover their essential architecture;
- full `Causal Inference: What If` — useful teacher reference, but too broad and advanced for this first-pass notebook;
- F0.3 risk-of-bias/confounding sources — premature for this unit.

## 4. Study sequence

Follow the passes in order. Do not start by asking NotebookLM to summarize all sources at once.

### Pass 1 — reconstruct the universal design-reading algorithm

Study the canonical lesson first.

Then ask NotebookLM:

> Based only on the F0.2 lesson, build a design-identification flowchart using this order: question type → who determined exposure/intervention → where sampling starts → temporal direction → unit of allocation → between/within-subject structure → outcome/time horizon → strongest defensible inference → tempting unsupported inference. Do not introduce F0.3 bias terminology beyond what the lesson itself states.

After NotebookLM responds, reproduce the flowchart from memory without looking.

Then test yourself with three descriptions you invent.

For each description, always finish with exactly:

- `Strongest defensible inference:`
- `Tempting unsupported inference:`

### Pass 2 — randomized parallel versus crossover

Ask NotebookLM:

> Compare randomized parallel and crossover designs using only the lesson, Cochrane Chapter 23 and CONSORT 2025. Cover allocation, between- versus within-subject comparison, reversibility, washout, carryover, period effects and situations where crossover is unsuitable.

Then answer these without help:

1. Why can crossover reduce between-person noise?
2. Why does that not make crossover universally superior?
3. Why would a 12-week hypertrophy adaptation often be unsuitable for a simple crossover?
4. What biological question should determine washout duration?
5. How can a period effect exist even when carryover is absent?

Then create two original scenarios:

- one acute sports-nutrition question suitable for crossover;
- one chronic question for which crossover is structurally poor.

Ask NotebookLM to critique your reasoning only after you answer.

### Pass 3 — cluster randomization and unit logic

Use the lesson plus Cochrane Chapter 23.

Ask:

> Teach cluster randomization without doing advanced statistics. Distinguish unit of allocation, unit of observation and unit of analysis. Explain why 300 athletes nested in 20 randomized teams are not 300 independently randomized units.

Then solve three variations yourself:

#### Scenario A

20 teams randomized; 300 athletes measured.

Identify:

- allocation unit;
- observation unit;
- dependence structure that must not be ignored;
- strongest defensible inference;
- tempting unsupported inference.

#### Scenario B

12 schools randomized; cafeterias implement a nutrition policy; students provide outcomes.

Repeat the same five outputs.

#### Scenario C

50 individual athletes randomized within one training center.

Explain why this is **not** automatically a cluster trial just because everyone trains in one center.

### Pass 4 — factorial trials

Use the canonical lesson and the 2025 BMJ factorial explanation/elaboration.

Ask:

> Build a 2 × 2 factorial example in sports nutrition with factors A and B. Show all four cells, identify the main comparison for A, identify the main comparison for B, and explain interaction conceptually without using advanced interaction-test statistics.

Then create your own 2 × 2 example.

You must answer:

1. What are the two randomized factors?
2. What are the four combinations?
3. What does the main effect of A conceptually compare?
4. What does the main effect of B conceptually compare?
5. Why can interaction make “A+B = effect A + effect B” false?
6. What tempting inference would overstate what the factorial architecture itself guarantees?

### Pass 5 — cohort, case-control and cross-sectional discrimination

Use the lesson plus STROBE.

Ask NotebookLM:

> Generate nine short observational study descriptions: three cohorts, three case-control studies and three cross-sectional studies. Mix prospective and retrospective data so that the word 'retrospective' cannot be used as the answer key. Present one at a time and wait for my classification.

For every case, give these outputs before NotebookLM grades you:

1. design;
2. where sampling/selection begins;
3. temporal structure;
4. strongest defensible inference;
5. tempting unsupported inference.

You must be able to explain these rules without notes:

- cohort: begins from exposure/baseline and proceeds toward outcomes;
- case-control: begins by outcome/case status and reconstructs prior exposures;
- cross-sectional: exposure/outcome are assessed in an essentially contemporaneous window.

Critical trap:

> Historical records do not automatically mean “case-control.” A retrospective cohort is still a cohort if its sampling logic starts from baseline/exposure and then reconstructs later outcomes.

### Pass 6 — acute versus chronic inference boundary

Return to the canonical lesson.

Ask NotebookLM to create five paired statements such as:

- measured acute outcome;
- exaggerated chronic conclusion.

Do not let it correct them immediately.

For each pair, rewrite the conclusion so that outcome and time horizon match what was actually measured.

You should be able to reject statements of this form automatically:

> “This condition changed an acute molecular marker, therefore it necessarily improves 16-week hypertrophy.”

The correct response is not “acute mechanisms are useless.” The correct response is:

> they answer a different question and may inform mechanistic plausibility without directly establishing the chronic outcome.

### Pass 7 — question-specific design choice

Ask:

> Give me one intervention-effect question, one prevalence question, one prognostic question, one rare-harm question and one acute mechanistic question. Do not tell me the preferred design. Wait for me to choose and justify one.

For each, justify the design from the **question**, not from a universal evidence hierarchy.

Your explanation should explicitly reject the statement:

> “RCT is always the best design for every scientific question.”

### Pass 8 — target-trial thinking

Read the target-trial article sections relevant to why/when the framework is useful.

Then ask NotebookLM:

> At an introductory F0.2 level, teach me how to specify a target trial before emulating it with observational data. Require eligibility, strategies, assignment concept, time zero, follow-up, outcome and causal contrast. Do not pretend emulation creates randomization or solves unmeasured confounding.

Then use this hypothetical question:

> Among resistance-trained adults, does starting strategy A rather than B at the beginning of a 12-week training block improve a prespecified performance outcome?

Before asking for feedback, specify:

1. eligibility;
2. strategies A and B;
3. ideal assignment mechanism;
4. time zero;
5. follow-up;
6. outcome;
7. causal contrast/target quantity;
8. observational data needed to emulate the protocol;
9. what emulation still cannot create;
10. which unresolved validity questions belong to F0.3.

### Pass 9 — mixed unfamiliar classification

Use this exact prompt:

> Act as an examiner for F0.2. Generate unfamiliar study descriptions one at a time. Randomly alternate among randomized parallel, crossover, cluster, factorial, non-randomized intervention, cohort, case-control, cross-sectional, acute mechanistic, chronic longitudinal, diagnostic, prognostic and target-trial-emulation scenarios. Do not put the design name in the wording. Wait for my answer. Require me to state design, origin of contrast, temporal direction, between/within-subject structure when applicable, allocation unit when applicable, strongest defensible inference and tempting unsupported inference. Only then grade me using citations to the approved corpus. Do not teach F0.3 in place of F0.2.

Continue until classification is based on structure rather than trigger words.

## 5. Source-comparison tasks

These are required because the corpus contains different source types.

### Task A — CONSORT versus Cochrane

Ask:

> Which parts of trial architecture can I reconstruct from CONSORT 2025 reporting expectations, and which cluster/crossover design details are explained more directly by Cochrane Chapter 23? Explain why neither document is a universal quality score.

### Task B — STROBE versus causal inference

Ask:

> What does STROBE help a reader locate in cohort, case-control and cross-sectional reports? What causal conclusion does STROBE itself not authorize merely because reporting is complete?

### Task C — general CONSORT versus factorial extension

Ask:

> Why is CONSORT 2025 the current general randomized-trial reporting standard while the factorial-specific guidance still refers to a CONSORT 2010 extension? Which factorial architecture concepts remain instructionally useful?

Expected answer:

- current general standard = CONSORT 2025;
- factorial-specific extension was built against CONSORT 2010;
- factorial factor structure, main comparisons and interaction remain specialized concepts not erased by the general update;
- reporting compliance remains different from risk-of-bias judgment.

### Task D — randomized ideal versus target-trial emulation

Ask:

> Compare an actual randomized trial with an observational target-trial emulation. What design elements can be made analogous, and what central feature cannot be recreated retrospectively?

The central missing feature is actual randomized treatment assignment.

## 6. Independent assessment outside NotebookLM

After completing the study sequence:

1. open `foundations/F0-scientific-literacy/F0.2-study-designs/EXERCISES.md`;
2. answer the full assessment **without NotebookLM and without `ANSWER_KEY.md`**;
3. only after the first attempt, use `ANSWER_KEY.md` or submit the answers to ChatGPT for correction;
4. use the canonical local gate: `>=80/100` plus no critical fail can support progression evidence;
5. this still does not equal `MASTERED`; later cumulative retesting is required.

The package itself does not change `UNSEEN`.

## 7. F0.2 critical-fail patterns to prevent

Treat these as structural failures even if terminology recall is otherwise good:

- classifying retrospective cohort as case-control solely because the data are historical;
- claiming temporal ordering alone proves causality;
- treating all individuals in a cluster RCT as independently randomized units;
- recommending crossover when intervention effects are meaningfully persistent/irreversible without addressing the structural problem;
- assuming factorial effects combine additively by default;
- converting an acute mechanistic outcome directly into proof of a chronic adaptation;
- claiming target-trial emulation itself creates randomization;
- using CONSORT/STROBE checklist completion as proof of low bias/high methodological quality.

## 8. What to send back to ChatGPT after study

For honest learning-state updates, provide one of:

- completed F0.2 `EXERCISES.md` answers;
- or confirmation that the study sequence was completed **plus** answers to a fresh F0.2 assessment administered in chat.

A statement such as “I read it” or “I understood everything” is not sufficient to mark `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED`.

## 9. When NotebookLM disagrees with GitHub

Use this order:

1. inspect the exact external source cited by NotebookLM;
2. inspect the canonical F0.2 lesson and manifest;
3. determine whether the disagreement is a source-version issue, interpretation issue or repository error;
4. if the repository is demonstrably wrong/outdated, research and update GitHub;
5. do not silently treat NotebookLM output as canonical.

## 10. Package completion criterion

The F0.2 notebook is correctly configured when:

- exactly six approved sources are loaded initially;
- `ANSWER_KEY.md` and `EXERCISES.md` are absent from the corpus;
- the learner can classify unfamiliar studies from architecture rather than keywords;
- crossover reasoning includes washout/carryover/period structure;
- cluster reasoning distinguishes allocation from observation/analysis;
- factorial reasoning includes factors, main contrasts and non-additivity/interaction intuition;
- cohort/case-control/cross-sectional classification does not depend on “prospective/retrospective” trigger words;
- acute versus chronic boundaries are preserved;
- target-trial emulation is not confused with actual randomization;
- every substantive classification ends with strongest defensible inference plus tempting unsupported inference;
- external reporting guidelines are not converted into study-quality scores;
- independent assessment occurs only after source-guided study and outside NotebookLM.
