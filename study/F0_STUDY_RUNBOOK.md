# F0 — Study-to-Exit Runbook

**State:** `READY_FOR_USE`
**Created:** `2026-09-11`
**Current learner state at creation:** `UNSEEN`
**F0.4 quantitative diagnostic at creation:** `UNOBSERVED`
**Purpose:** define the canonical learner workflow from first F0 study contact through legitimate readiness for the cumulative F0 Exit Assessment.

This file is an **operational learning protocol**, not evidence that any study has occurred. Creating, reading or versioning this runbook changes no learner state.

---

## 1. Non-negotiable rules

1. GitHub is canonical. NotebookLM is a controlled study layer.
2. Production status and learner status are separate.
3. `UNSEEN → STUDIED → RECALLED → APPLIED → INTEGRATED → MASTERED` requires progressively stronger observed evidence.
4. Reading, highlighting, watching an explanation or feeling confident does not equal mastery.
5. Initial NotebookLM corpora must follow each module `MANIFEST.md`; do not let NotebookLM silently expand the source set.
6. `EXERCISES.md`, `ANSWER_KEY.md`, production `QA_REPORT.md`, the full `SOURCE_INDEX.md` and prerequisite diagnostics stay outside initial NotebookLM corpora unless a manifest explicitly says otherwise.
7. Module answer keys are opened only after the learner has produced an independent first attempt.
8. Errors are routed to the **earliest broken dependency**, not merely the module where the error was noticed.
9. Retests use new numbers/scenarios/papers when transfer is being evaluated.
10. Personal health, diet, body-measurement, laboratory or other sensitive data are not persisted in this public repository.
11. The F0 Exit Assessment is quarantined until readiness is established. Its answer key is never used as study material.
12. A first Exit pass may support `APPLIED`/`INTEGRATED`; it never creates automatic `MASTERED`.

---

# 2. Canonical F0 study route

The preferred first-pass route is linear for simplicity, while advancement rules remain dependency-based:

`F0.1 → F0.2 → F0.3 → quantitative entry diagnostic → F0.4 → F0.5 → F0.6 → F0.7 → F0.8 → F0.9 → F0.10 → cumulative retrieval → F0 Exit Assessment`

This route respects the P2 dependencies in `foundations/F0-scientific-literacy/PREREQUISITE_GRAPH.md`.

The graph, not the calendar, is authoritative. If a learner needs targeted remediation in one branch, another branch may continue **only** when its own structural prerequisites are satisfied.

Examples:

- F0.2 weakness blocks F0.3 and later units that structurally depend on F0.2.
- F0.2 weakness does not automatically block F0.4 once F0.1 and the quantitative-entry requirements are satisfied.
- F0.5 cannot be validated while F0.4 sampling/uncertainty foundations remain structurally broken.
- F0.9 cannot be validated until F0.1–F0.8 dependencies have been demonstrated.
- F0.10 requires F0.5 + F0.7 + F0.8 + F0.9.
- the Exit Assessment requires F0.1–F0.10.

---

# 3. NotebookLM corpus instantiation

Create **one NotebookLM notebook per F0 module**. Do not combine all F0 sources into one giant first-pass notebook.

| Module | NotebookLM package |
|---|---|
| F0.1 | `notebooklm/F0.1-scientific-questions/` |
| F0.2 | `notebooklm/F0.2-study-designs/` |
| F0.3 | `notebooklm/F0.3-bias-confounding-causal-validity/` |
| F0.4 | `notebooklm/F0.4-descriptive-statistics/` |
| F0.5 | `notebooklm/F0.5-estimates-confidence-pvalues-effect-sizes/` |
| F0.6 | `notebooklm/F0.6-power-multiplicity-analytical-flexibility/` |
| F0.7 | `notebooklm/F0.7-systematic-reviews-meta-analysis-heterogeneity/` |
| F0.8 | `notebooklm/F0.8-risk-of-bias-certainty-applicability/` |
| F0.9 | `notebooklm/F0.9-critical-reading-complete-paper/` |
| F0.10 | `notebooklm/F0.10-synthesis-communication-uncertainty/` |

For every module, use this setup procedure:

### Step N1 — open the manifest

Open that package's `MANIFEST.md` and confirm:

- `Package state` is `READY_FOR_STUDY`;
- manifest version;
- learning objectives;
- exact `sources:` list;
- each source role (`CORE`, `SUPPORT`, `CONTRAST`);
- corpus exclusions.

### Step N2 — create the notebook

Use a stable name:

`Sports Nutrition Mastery — F0.x <short module title>`

Never reuse another module's notebook as the first-pass corpus.

### Step N3 — add exactly the approved first-pass sources

For each manifest source:

1. add the canonical repository lesson when listed;
2. add the exact official/open source URL or legally obtained file named in the manifest;
3. preserve source-role intent;
4. if NotebookLM cannot ingest a living/JavaScript page reliably, keep the official page open as a manual reference rather than importing an unofficial scrape;
5. do not replace a primary/official source with an AI summary.

### Step N4 — verify contamination controls

Before studying, confirm that the notebook does **not** contain:

- module `ANSWER_KEY.md`;
- module `EXERCISES.md` unless a future manifest explicitly changes policy;
- module production `QA_REPORT.md`;
- F0.4 `ENTRY_DIAGNOSTIC.md`;
- the entire `SOURCE_INDEX.md`;
- F0 Exit Assessment or its answer key;
- random web sources discovered by NotebookLM.

### Step N5 — follow `STUDY_GUIDE.md`

The module's `STUDY_GUIDE.md` determines the approved pass order. Do not jump directly to the final real-paper/transfer task before building the conceptual skeleton.

NotebookLM should usually be prompted to:

- ask one question at a time;
- wait for the learner's answer;
- grade after the response, not before;
- cite approved sources;
- distinguish repository synthesis from source-stated claims;
- keep a temporary error list for the session;
- avoid topics from future F0 modules unless the current guide intentionally integrates them.

---

# 4. Standard module study cycle

Every F0 module uses six learner phases.

## Phase M1 — source-guided first pass

Complete the ordered passes in that module's `STUDY_GUIDE.md`.

Goal: construct the model, not memorize wording.

Evidence that may support `STUDIED`:

- observed participation in a study session;
- completion of the guide's required reconstruction/worked tasks;
- source-guided explanation showing the learner actually engaged with the module.

A simple statement such as “I read it” can document exposure, but by itself does not support `RECALLED` or higher.

## Phase M2 — closed-book active recall

Before opening the module assessment or answer key:

1. close the lesson/notes when practical;
2. answer the guide's active-recall prompts from memory;
3. include definitions, mechanisms, counterexamples and boundaries—not definitions only;
4. let NotebookLM/ChatGPT correct only **after** each response.

Evidence for `RECALLED` requires actual responses that retrieve the core model without answer exposure.

## Phase M3 — fresh micro-transfer

Before the formal module assessment, solve at least one fresh example not copied from the lesson.

Examples by competency:

- reformulate a new claim;
- classify a new design;
- explain a new causal distortion path;
- interpret a new graph/table;
- interpret a new estimate + CI + threshold;
- map a new multiplicity family;
- interpret a new forest-plot scenario;
- compare two new evidence bodies;
- appraise a new paper fragment;
- translate a new evidence statement across audiences.

The point is to detect answer-pattern memorization before the scored attempt.

## Phase M4 — independent module assessment

Open only:

`foundations/F0-scientific-literacy/<module>/EXERCISES.md`

Rules:

- first attempt without `ANSWER_KEY.md`;
- no NotebookLM answer generation during the attempt;
- show reasoning/calculations when requested;
- ordinary academic answers may be submitted in chat for grading;
- do not persist personal/sensitive examples in GitHub.

All current F0 module assessments use the local competence gate:

`>=80/100 + no critical fail`

Interpretation:

- `>=80` + no critical fail: sufficient local progression evidence;
- `70–79`: targeted remediation + fresh equivalent items before treating the competency as stable;
- `<70`: broader module review + equivalent reassessment;
- any critical fail: targeted repair is mandatory regardless of total score.

A passing local assessment can support `APPLIED` when the scored work actually contains application. It does not automatically support `INTEGRATED` or `MASTERED`.

## Phase M5 — correction and error routing

Only after the independent attempt:

1. score with the canonical `ANSWER_KEY.md`;
2. identify incorrect/partial reasoning;
3. classify each material error;
4. route it to the earliest broken dependency;
5. create remediation using new examples;
6. retest the repaired concept before dependent validation.

Do not simply reread the same answer until it feels familiar.

## Phase M6 — persist observed evidence

After a meaningful observed session, update the study artifacts according to Section 8 of this runbook.

---

# 5. Quantitative entry diagnostic — exact position and routing

The diagnostic is:

`foundations/F0-scientific-literacy/F0.4-descriptive-statistics/ENTRY_DIAGNOSTIC.md`

It tests the quantitative bridge **before F0.4 validation**, not F0.4 statistics itself.

Canonical operational position in the preferred route:

`after first-pass F0.1–F0.3 work and before beginning F0.4 validation`

It may be administered earlier, but it **must** be completed and scored before quantitative readiness is treated as demonstrated for F0.4.

### Diagnostic administration

- first attempt without calculator unless an item says otherwise;
- no lesson, answer key or AI assistance;
- show calculations;
- total = `16` points across eight domains.

### Routing

#### `READY_FOR_F0.4`

- `14–16/16`; and
- no domain at `0/2`.

Action: proceed to F0.4. Isolated slips may be repaired locally.

#### `P1_REPAIR`

Typical criteria:

- `10–13/16`; or
- `14–16/16` with one or two zeroed domains;
- at least six of eight domains show some competence (`>=1/2`).

Action:

1. identify the specific broken domains;
2. give a short targeted micro-lesson;
3. solve new equivalent items;
4. verify correction before the affected F0.4 task.

Do not label this as “bad at math.” It is a local academic gap.

#### `P2-QB_REQUIRED`

Trigger if any occurs:

- `<=9/16`;
- three or more domains at `0/2`;
- fewer than six of eight domains show any competence.

Action:

1. promote the quantitative bridge to structural prerequisite `P2-QB`;
2. pause F0.4 validation and all downstream quantitative validation that depends on it;
3. build a targeted bridge only around observed broken domains;
4. use new practice items;
5. administer an equivalent diagnostic form;
6. require a resolved bridge result before returning to F0.4 validation.

The diagnostic itself does not change F0.1–F0.3 states and never authorizes `MASTERED`.

---

# 6. Advancement and remediation rules

## 6.1 Local progression rule

A learner may treat a module's local validation as passed when:

- formal module assessment `>=80/100`;
- no local critical fail;
- observed reasoning is coherent enough that the score is not produced by unsupported guessing;
- any structural prerequisite for the next target module is already satisfied.

## 6.2 A pass does not erase prerequisite errors

If F0.6 scores 86 but the learner still interprets `p>0.05` as proof of no effect, the error routes to F0.5 and remains structural until repaired.

A high score cannot compensate for a broken conceptual safety gate.

## 6.3 Targeted-remediation parallelism

The curriculum is dependency-based, not a rigid calendar.

During remediation, the learner may continue a module on another branch only when the prerequisite graph permits it.

Example:

- unresolved F0.2 design inference blocks F0.3;
- F0.4 may still proceed after F0.1 + resolved quantitative diagnostic because F0.2 is not a P2 for F0.4;
- F0.7 must wait for its required F0.2/F0.5/F0.6 dependencies and formal causal interpretation also depends on F0.3.

## 6.4 Critical-fail rule

Any critical fail generates:

- an `ERROR_LEDGER` entry;
- targeted remediation;
- a fresh retest condition;
- no dependent validation until the error is demonstrably repaired.

---

# 7. Cumulative retrieval and spacing

Local passing performance is not enough for durable mastery. Use repeated retrieval with fresh material.

The canonical F0 cadence is:

### R0 — same study cycle

Before the module assessment, perform closed-book active recall and one fresh micro-transfer.

### R1 — short-delay retrieval

Target: `1–3 days` after local pass.

Use:

- 5–10 closed-book prompts;
- at least one counterexample/boundary item;
- no reused answer-key wording.

Purpose: verify that the model survives beyond the immediate session.

### R2 — one-week mixed retrieval

Target: approximately `7 ± 2 days` after local pass.

Mix:

- current module;
- one or two prerequisite modules;
- at least one fresh application.

Purpose: detect dependency decay and interference between similar concepts.

### R3 — cumulative integration

Target: approximately `14–21 days` after a meaningful cluster of modules, and again after F0.10.

Use fresh mixed scenarios requiring multiple modules in one chain.

Examples:

- question → design → bias → estimate/CI → uncertainty;
- trial → multiplicity → RoB → certainty → applicability;
- systematic review → heterogeneity → certainty → calibrated communication.

### Compression rule

If the learner studies faster than these windows, progression may continue when P2 dependencies are satisfied, but at least one **delayed** retrieval must still occur before treating the block as durable or administering the Exit Assessment.

Do not replace spacing with repeating the same item immediately.

---

# 8. Canonical study-record updates

Only observed evidence is persisted.

## 8.1 `study/STUDY_HISTORY.md`

Append one entry after a meaningful study/validation event using the existing template:

```text
Date:
Module:
Activity:
Evidence of performance:
Observed strengths:
Observed gaps:
Mastery changes:
Next study action:
```

Good evidence descriptions are concrete:

- `F0.2 EXERCISES 84/100, no critical fail; misclassified one retrospective cohort item`;
- `closed-book recall: 8/10, confused SD vs SE`;
- `F0.4 entry diagnostic 12/16 → P1_REPAIR in percentage-points and ratio domains`.

Avoid vague entries such as `understood well`.

## 8.2 `study/ERROR_LEDGER.md`

Create an entry for a material observed error when it is:

- conceptual;
- recurrent;
- a critical fail;
- a structural prerequisite issue;
- significant enough to require planned remediation/retest.

Use the canonical fields:

```text
ERROR-ID:
Date:
Module/competency:
Observed error:
Error type: CONCEPT | MECHANISM | EVIDENCE | STATISTICS | APPLICATION | INTEGRATION
Likely cause:
Correct model:
Remediation:
Retest condition:
Status: OPEN | RETEST_PENDING | RESOLVED
```

`Likely cause` must refer to an academic reasoning gap, not psychological speculation.

One trivial arithmetic slip corrected immediately does not need to become a persistent ledger item unless it reveals a pattern.

## 8.3 `study/MASTERY_MATRIX.md`

Do not advance states by content completion alone.

Evidence model:

- `STUDIED` — actual source-guided study occurred, but retrieval/application remains insufficient;
- `RECALLED` — core concepts retrieved without answer exposure;
- `APPLIED` — successful fresh application/assessment supports use of the competency;
- `INTEGRATED` — observed cross-module reasoning combines competencies coherently;
- `MASTERED` — robust repeated performance across time and contexts, including delayed retest.

When evidence begins, module-level rows may be added beneath the F0 aggregate row, for example:

`F0.1 question operationalization | APPLIED | <date/evidence> | independent assessment | <next review>`

Do not raise the aggregate F0 row beyond what the observed block-level evidence supports.

A single local module pass does not make aggregate F0 `APPLIED`.

---

# 9. Module-by-module first-pass checklist

For each module below, the learner repeats the standard M1–M6 cycle.

## F0.1 — Scientific questions, hypotheses and operationalization

NotebookLM:

- `notebooklm/F0.1-scientific-questions/MANIFEST.md`
- `notebooklm/F0.1-scientific-questions/STUDY_GUIDE.md`

Independent assessment:

- `foundations/F0-scientific-literacy/F0.1-scientific-questions/EXERCISES.md`

Primary progression target:

`question → target population → contrast → outcome → time → estimand`

Do not begin with the answer key.

## F0.2 — Study designs and inference boundaries

NotebookLM:

- `notebooklm/F0.2-study-designs/MANIFEST.md`
- `notebooklm/F0.2-study-designs/STUDY_GUIDE.md`

Assessment:

- `foundations/F0-scientific-literacy/F0.2-study-designs/EXERCISES.md`

P2: F0.1.

## F0.3 — Bias, confounding, causal reasoning and validity

NotebookLM:

- `notebooklm/F0.3-bias-confounding-causal-validity/MANIFEST.md`
- `notebooklm/F0.3-bias-confounding-causal-validity/STUDY_GUIDE.md`

Assessment:

- `foundations/F0-scientific-literacy/F0.3-bias-confounding-causal-validity/EXERCISES.md`

P2: F0.1 + F0.2.

## Quantitative gate before F0.4

Administer and resolve:

- `foundations/F0-scientific-literacy/F0.4-descriptive-statistics/ENTRY_DIAGNOSTIC.md`

Record only the observed routing result.

## F0.4 — Descriptive statistics, distributions and sampling variation

NotebookLM:

- `notebooklm/F0.4-descriptive-statistics/MANIFEST.md`
- `notebooklm/F0.4-descriptive-statistics/STUDY_GUIDE.md`

Assessment:

- `foundations/F0-scientific-literacy/F0.4-descriptive-statistics/EXERCISES.md`

P2: F0.1 + resolved conditional quantitative bridge.

## F0.5 — Estimates, CIs, p-values, effect sizes and practical relevance

NotebookLM:

- `notebooklm/F0.5-estimates-confidence-pvalues-effect-sizes/MANIFEST.md`
- `notebooklm/F0.5-estimates-confidence-pvalues-effect-sizes/STUDY_GUIDE.md`

Assessment:

- `foundations/F0-scientific-literacy/F0.5-estimates-confidence-pvalues-effect-sizes/EXERCISES.md`

P2: F0.4.

## F0.6 — Power, Type I/II error, multiplicity and analytical flexibility

NotebookLM:

- `notebooklm/F0.6-power-multiplicity-analytical-flexibility/MANIFEST.md`
- `notebooklm/F0.6-power-multiplicity-analytical-flexibility/STUDY_GUIDE.md`

Assessment:

- `foundations/F0-scientific-literacy/F0.6-power-multiplicity-analytical-flexibility/EXERCISES.md`

P2: F0.4 + F0.5.

## F0.7 — Systematic reviews, meta-analysis and heterogeneity

NotebookLM:

- `notebooklm/F0.7-systematic-reviews-meta-analysis-heterogeneity/MANIFEST.md`
- `notebooklm/F0.7-systematic-reviews-meta-analysis-heterogeneity/STUDY_GUIDE.md`

Assessment:

- `foundations/F0-scientific-literacy/F0.7-systematic-reviews-meta-analysis-heterogeneity/EXERCISES.md`

P2: F0.2 + F0.5 + F0.6; F0.3 before formal RoB interpretation.

## F0.8 — Risk of bias, certainty and applicability

NotebookLM:

- `notebooklm/F0.8-risk-of-bias-certainty-applicability/MANIFEST.md`
- `notebooklm/F0.8-risk-of-bias-certainty-applicability/STUDY_GUIDE.md`

Assessment:

- `foundations/F0-scientific-literacy/F0.8-risk-of-bias-certainty-applicability/EXERCISES.md`

P2: F0.2 + F0.3 + F0.5 + F0.7.

## F0.9 — Critical reading of a complete paper

NotebookLM:

- `notebooklm/F0.9-critical-reading-complete-paper/MANIFEST.md`
- `notebooklm/F0.9-critical-reading-complete-paper/STUDY_GUIDE.md`

Assessment:

- `foundations/F0-scientific-literacy/F0.9-critical-reading-complete-paper/EXERCISES.md`

P2: F0.1–F0.8.

The completed F0.9 answer key must remain outside the initial NotebookLM corpus.

## F0.10 — Synthesis and communication of uncertainty

NotebookLM:

- `notebooklm/F0.10-synthesis-communication-uncertainty/MANIFEST.md`
- `notebooklm/F0.10-synthesis-communication-uncertainty/STUDY_GUIDE.md`

Assessment:

- `foundations/F0-scientific-literacy/F0.10-synthesis-communication-uncertainty/EXERCISES.md`

P2: F0.5 + F0.7 + F0.8 + F0.9.

---

# 10. Exit Assessment quarantine

Until the readiness criteria in Section 11 are met, do not use these as study sources:

- `foundations/F0-scientific-literacy/F0-exit-assessment/ASSESSMENT.md`;
- `foundations/F0-scientific-literacy/F0-exit-assessment/ANSWER_KEY.md`;
- F0-S32 full paper;
- F0-S33 trial registry/timeline companion.

The learner should encounter the Exit Assessment as a transfer task, not a memorized packet.

If the exit `ANSWER_KEY.md` is exposed before an independent attempt, assessment v1 should not be treated as clean validation. Use/author an alternate form before assigning exit-state evidence.

---

# 11. Readiness criteria before F0 Exit Assessment

Administer the cumulative Exit Assessment only when **all** conditions below are met.

## 11.1 Content exposure

- F0.1–F0.10 each have an observed first-pass study event.

## 11.2 Quantitative prerequisite

- F0.4 quantitative diagnostic has an observed resolved routing state;
- if `P2-QB_REQUIRED` occurred, the bridge has been completed and an equivalent retest demonstrates sufficient readiness.

## 11.3 Local validation

- all ten module assessments have independent attempts;
- each current local module gate has been met (`>=80/100 + no critical fail`), or a later equivalent retest has repaired the failed module;
- no unresolved structural prerequisite error remains.

## 11.4 Retrieval durability

- at least one delayed cumulative retrieval has occurred after F0.10;
- that retrieval includes material from early, middle and late F0 units;
- no unresolved critical misconception appears in causal inference, quantitative uncertainty, evidence synthesis/certainty or communication.

## 11.5 Integrative evidence

Before exit administration, the learner has already demonstrated, outside the exit packet, at least one complete chain resembling:

`question → design → bias → estimate/uncertainty → certainty/applicability → calibrated conclusion`

F0.9 and F0.10 assessments can provide this evidence when completed successfully.

## 11.6 Exit packet remains uncontaminated

- learner has not studied the exit answer key;
- F0-S32/F0-S33 have not been used as training exemplars;
- assessment questions have not been rehearsed item-for-item.

---

# 12. F0 Exit Assessment administration

Assessment:

`foundations/F0-scientific-literacy/F0-exit-assessment/ASSESSMENT.md`

Answer key, opened only after independent completion:

`foundations/F0-scientific-literacy/F0-exit-assessment/ANSWER_KEY.md`

Administration rules from the assessment remain authoritative:

- Sections A, B, C and E without module answer keys;
- Section D may use the assigned full paper, its public registry and directly linked study materials;
- write `NOT REPORTED`/`UNCLEAR` rather than inventing absent information;
- show reasoning;
- calculator allowed;
- external generative assistance is outside intended independent administration.

### Exit gate

Pass requires **all**:

- total `>=85/100`;
- every section `>=70%` of its points;
- no `CRITICAL_FAIL`;
- defensible integrated Section D chain;
- Section E preserves uncertainty when simplifying language.

### Result routing

#### PASS

Action:

- record the score/section profile and observed reasoning;
- update relevant module/aggregate states only to the strongest level actually supported;
- a strong first pass may support F0 `APPLIED` or `INTEGRATED` depending on the demonstrated cross-module reasoning;
- schedule delayed cumulative retest during later F1/F2/domain work;
- do **not** set `MASTERED` from one pass.

#### `75–84` and no critical fail

Result:

`NEAR_PASS / TARGETED_REMEDIATION`

Action:

1. map each loss to earliest F0 dependency;
2. reopen only the needed modules;
3. log material errors;
4. use fresh remediation tasks;
5. retest with an alternate form rather than repeating memorized answers.

#### `<75`

Action:

- broader remediation by earliest broken prerequisites;
- rebuild cumulative retrieval before another exit attempt;
- alternate-form exit retest required.

#### Any `CRITICAL_FAIL`

Action:

- exit not passed regardless of numeric total;
- create explicit `ERROR_LEDGER` entry;
- repair and independently retest the structural misconception;
- do not advance aggregate F0 state past what the repaired evidence supports.

---

# 13. What `MASTERED` requires after Exit

`MASTERED` is deliberately deferred.

Evidence should include robust performance across time, for example:

1. F0 Exit performance;
2. later cumulative retrieval after delay;
3. evidence appraisal in F1/F2 or a domain module;
4. new quantitative/evidence scenarios;
5. successful transfer to a different paper/evidence body;
6. no recurrence of critical misconceptions.

This protects the project from converting one good examination into a permanent claim of mastery.

---

# 14. Public-repository privacy rule during study

Persist only educational information needed for continuity:

- module studied;
- scores;
- conceptual strengths/gaps;
- academic error patterns;
- remediation/retest status.

Do not persist:

- body weight/body composition;
- laboratory results;
- diagnoses/medications;
- private dietary records;
- other identifiable health data.

If a learning example uses the learner's real personal data in chat, convert it to a fictitious/generic academic example before any repository persistence unless the user explicitly requests otherwise and public-repo policy still permits it.

---

# 15. Canonical session-closing checklist

At the end of every observed F0 learner session:

1. identify exactly what the learner actually did;
2. record observed responses/scores, not inferred ability;
3. append `STUDY_HISTORY.md` when the session is meaningful;
4. create/update `ERROR_LEDGER.md` only for material observed errors;
5. update `MASTERY_MATRIX.md` only when evidence supports a state transition;
6. preserve unresolved prerequisites;
7. assign a fresh next study/retest action;
8. never open an answer key before the independent attempt it scores.

---

# 16. Current starting point

At creation of this runbook:

- F0.1–F0.10 instructional units = produced/approved;
- F0.1–F0.10 NotebookLM packages = `READY_FOR_STUDY`;
- F0 Exit Assessment v1 = `READY_FOR_ADMINISTRATION` as an artifact, but learner not yet ready;
- learner F0 aggregate = `UNSEEN`;
- initial domain = `UNKNOWN` and must be measured;
- F0.4 quantitative diagnostic = `UNOBSERVED`;
- no observed learner study session is persisted yet.

Therefore the next legitimate project activity is **not more curriculum production and not the Exit Assessment**.

It is the first observed F0.1 learning session.
