# F0.7 — Practical NotebookLM Study Guide

**Package version:** `1`
**Module:** `F0.7 — Systematic reviews, meta-analyses and heterogeneity`
**Current learner state:** `UNSEEN`
**F0.4 quantitative diagnostic:** `UNOBSERVED`

This guide defines how to build and use the approved NotebookLM corpus for F0.7. Creating the notebook, reading sources or completing these study passes does **not** change learner state. Any transition requires observed performance under the mastery protocol.

## 0. Prerequisite integrity

F0.7 learner validation requires F0.2 + F0.5 + F0.6 as structural P2 prerequisites. F0.3 is required before formal risk-of-bias interpretation inside evidence synthesis.

This package therefore assumes the learner can already:

- identify what study designs can/cannot support;
- interpret effect measures, estimates and confidence intervals;
- separate magnitude/precision from p-value thresholding;
- recognize prespecification, multiplicity and analytical flexibility.

The F0.4 quantitative entry diagnostic remains `UNOBSERVED` and must stay outside this notebook.

---

## 1. Create the notebook

Create one NotebookLM notebook named:

`Sports Nutrition Mastery — F0.7 Evidence Synthesis`

Keep it separate from F0.6. F0.6 focuses on error rates and analytical decisions inside studies; F0.7 moves to assembling and interpreting a body of studies.

---

## 2. Add exactly five initial sources

### Source 1 — canonical F0.7 lesson — CORE

Repository file:

`foundations/F0-scientific-literacy/F0.7-systematic-reviews-meta-analysis-heterogeneity/LESSON.md`

Preferred URL:

`https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.7-systematic-reviews-meta-analysis-heterogeneity/LESSON.md`

Use as the instructional spine for:

- systematic review versus meta-analysis;
- review workflow;
- compatibility before pooling;
- inverse-variance intuition;
- fixed/random effects;
- forest plots;
- heterogeneity/I²;
- sensitivity/subgroup/meta-regression;
- small-study/missing-evidence reasoning;
- PRISMA boundary;
- integrated twelve-field audit.

If the raw URL cannot be ingested, upload the canonical Markdown file itself. Do not substitute an AI summary.

### Source 2 — Cochrane Handbook Chapter 10 — CORE

Add:

`https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-10`

Use for:

- deciding whether numerical pooling is meaningful;
- inverse-variance weighting;
- fixed-effect versus random-effects models;
- clinical/methodological/statistical heterogeneity;
- I² and tau²;
- pooled CI versus prediction interval;
- subgroup/meta-regression cautions;
- sensitivity analyses.

Do not turn this into a software/estimator course. The target is methodological interpretation.

### Source 3 — Cochrane Handbook Chapter 6 — SUPPORT

Add:

`https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-06`

Use for:

- data/effect-measure compatibility;
- MD, SMD, RD, RR and OR distinctions;
- ratio-measure log-scale reminder;
- unit-of-analysis structure;
- conversions needed before pooling.

Required rule:

> Same sign does not make different effect measures numerically poolable.

### Source 4 — Cochrane Handbook Chapter 13 — SUPPORT

Add:

`https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-13`

Use for:

- missing evidence/non-reporting;
- small-study effects;
- funnel-plot interpretation;
- alternative causes of funnel asymmetry;
- why symmetry/asymmetry is non-diagnostic.

Do not perform formal ROB-ME judgments in F0.7.

### Source 5 — PRISMA 2020 — CONTRAST

Add:

`https://www.prisma-statement.org/prisma-2020`

Use to answer this contrast question repeatedly:

> What can complete reporting make visible, and what does it still fail to prove about validity, risk of bias or certainty?

Target answer:

- PRISMA improves transparency/auditability;
- checklist completion does not certify scientific correctness;
- formal RoB/certainty remains F0.8.

---

## 3. Do NOT add these yet

Keep outside the initial notebook:

- F0.7 `EXERCISES.md` — independent assessment;
- F0.7 `ANSWER_KEY.md` — answer leakage;
- F0.7 production `QA_REPORT.md` — metadata;
- F0.4 `ENTRY_DIAGNOSTIC.md` — prerequisite diagnostic must remain uncontaminated;
- full `SOURCE_INDEX.md` — retrieval noise;
- formal RoB 2 / ROBINS-I / ROB-ME manuals — F0.8;
- GRADE guidance — F0.8;
- transportability/applicability guidance — F0.8;
- network meta-analysis/IPD/advanced estimator manuals — outside F0.7 core;
- substantive sports-nutrition intervention papers — not required for this methodological package.

---

# 4. Study sequence

Do not begin with “summarize all sources”. Complete the passes in order.

## Pass 1 — systematic review versus meta-analysis

Prompt:

> Give me 10 short research-synthesis descriptions. Make me classify each as systematic review, meta-analysis, both, or neither. Do not reveal the answer until I commit.

Required distinctions:

- systematic review = explicit evidence process;
- meta-analysis = statistical combination;
- a systematic review may legitimately not pool;
- a numerical meta-analysis may be methodologically weak if study identification/selection is poor.

Critical fail:

`systematic review = meta-analysis`.

---

## Pass 2 — reconstruct the review workflow

Prompt:

> Give me eight incomplete review-method descriptions. Require me to reconstruct: protocol/question → eligibility → search → screening → extraction → appraisal/result selection → effect measure/synthesis plan → heterogeneity/missing evidence → interpretation.

For each case, identify what missing stage could change the evidence body or conclusion.

Include at least:

- changed eligibility after seeing results;
- incomplete search date;
- duplicate reports from one trial;
- selective timepoint extraction;
- unit-of-analysis problem.

---

## Pass 3 — study versus report

Prompt:

> Present citation clusters where one trial generated multiple papers, conference abstracts or follow-up reports. Make me decide how many independent studies exist and which reports contribute which outcomes/timepoints.

Required rule:

> Multiple reports do not automatically mean multiple independent studies.

Explain how double-counting can distort precision and weights.

---

## Pass 4 — compatibility before pooling

Use canonical lesson + Cochrane Chapter 6.

Prompt:

> Generate 12 study-result rows mixing MD, SMD, RR, OR, different timepoints, outcome directions and unit structures. Require a pool / harmonize first / keep separate decision before any numerical synthesis.

For every row/checklist answer:

1. construct;
2. outcome direction;
3. effect measure/scale;
4. timepoint;
5. target contrast;
6. unit-of-analysis structure;
7. whether a defensible conversion/harmonization exists.

Critical rule:

`same direction ≠ same numerical quantity`.

---

## Pass 5 — forest-plot anatomy before interpretation

Prompt:

> Generate 10 synthetic forest-plot rows or text representations. Make me identify study estimate, CI, marker/weight, null line, effect scale, pooled diamond and heterogeneity statistics before giving a conclusion.

Always require:

- difference-measure null = 0;
- ratio-measure null = 1;
- diamond centre = pooled estimate;
- diamond width = pooled CI;
- diamond ≠ truth.

Then use the F0.5 sequence:

`Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`

Only then add F0.7:

`Compatibility → Weight/model → Heterogeneity → Synthesis defensibility`.

---

## Pass 6 — inverse-variance weighting

Use Cochrane Chapter 10.

Start with:

`w ≈ 1/SE²`

Prompt:

> Give me pairs/triples of study SEs and require me to calculate approximate inverse-variance weights or weight ratios. After each calculation, ask what the weight does and does not represent.

Minimum manual examples:

- SE .20 versus .40;
- SE .30 versus .60;
- three studies normalized to percentages.

Required sentence:

> “This weight reflects statistical precision under the synthesis method; it is not a study-quality or certainty score.”

---

## Pass 7 — fixed-effect versus random-effects target

Use Cochrane Chapter 10.

Prompt:

> Give me eight synthesis scenarios. Make me state what quantity a fixed-effect/common-effect analysis and a random-effects analysis would summarize, then choose whether either model is scientifically defensible.

Required distinctions:

- fixed-effect/common-effect framing: common/typical target under model assumptions;
- random effects: average of different but related underlying effects under an assumed distribution;
- model choice is not determined only by heterogeneity-test p-value;
- neither model repairs bias.

Critical fail:

`random effects solves heterogeneity`.

---

## Pass 8 — pooled CI versus prediction/between-study variation

Prompt:

> Give me random-effects meta-analysis summaries where the pooled mean CI is narrow but study effects vary substantially. Require me to explain what the pooled CI estimates and what a prediction interval/between-study spread tries to represent.

Required distinction:

- pooled CI = uncertainty around average effect;
- prediction interval = possible spread of underlying effects/new comparable study effect under assumptions;
- narrow pooled CI does not imply homogeneous effects.

No advanced prediction-interval calculation is required.

---

## Pass 9 — three layers of heterogeneity

Prompt:

> Generate 10 examples and make me label each difference as clinical diversity, methodological diversity, statistical heterogeneity, or more than one.

Include:

- athlete training status;
- intervention duration;
- outcome instrument;
- risk-of-bias mechanism;
- different analysis population;
- unit-of-analysis mistake;
- genuinely different effect estimates.

Then require a causal story only as a hypothesis, never as proof from the heterogeneity statistic alone.

---

## Pass 10 — I² misconception repair

Use Cochrane Chapter 10.

Prompt:

> Present one I² claim at a time and require me to repair it. Include I²=0%, 20%, 55%, 87% and 95% in different clinical/methodological contexts.

Reject:

- “I² is percent of heterogeneous studies”;
- “low I² proves sameness”;
- “high I² automatically invalidates pooling”;
- “I² is a quality score”.

For every case require:

1. effect pattern;
2. number/precision of studies;
3. clinical diversity;
4. methodological diversity;
5. what I² adds;
6. what remains unresolved.

---

## Pass 11 — pooling versus no pooling

Prompt:

> Generate 10 evidence bodies. Some should be poolable, some should require harmonization first, and some should remain separate. Make me defend the decision in one paragraph.

Include cases with:

- materially different constructs;
- same construct/different validated scales;
- incompatible time horizons;
- crossover/cluster unit problems;
- opposite effects in meaningfully different contexts;
- high statistical heterogeneity but coherent common scientific question.

Required rule:

> No pooling is sometimes the correct synthesis decision; narrative/tabular synthesis is still synthesis.

---

## Pass 12 — sensitivity analysis as robustness, not result-shopping

Prompt:

> Give me planned and unplanned sensitivity analyses. Make me classify each as defensible robustness check, questionable post hoc exploration, or result-shopping.

Include:

- excluding a study with a known unit-of-analysis error;
- fixed versus random model comparison;
- alternative defensible conversion;
- excluding high attrition as prespecified;
- deleting studies one by one until p<.05.

Apply F0.6 timing/prespecification logic.

---

## Pass 13 — subgroup and meta-regression

Use Cochrane Chapter 10 + F0.6 concepts in the canonical lesson.

Prompt:

> Generate review-level subgroup/meta-regression scenarios with 5–20 studies. Make me identify prespecified versus post hoc moderators, direct interaction evidence, multiplicity, study-level confounding, collinearity and ecological limits.

Critical traps:

- significant subgroup A + nonsignificant subgroup B = interaction;
- p=.04 for one of many post hoc moderators = proven explanation;
- study-level meta-regression association = individual-level causal mechanism.

Before accepting a moderator story require at least **two alternative clinical/methodological explanations**.

---

## Pass 14 — small-study effects and funnel plots

Use Cochrane Chapter 13.

Prompt:

> Generate funnel-plot descriptions with few and many studies. Make me list possible causes of asymmetry and explain what symmetry cannot establish.

Required possible explanations for asymmetry include:

- missing/non-reported evidence;
- methodological bias in small studies;
- real clinical differences by study size/context;
- effect-measure artefacts;
- chance.

Critical rules:

`asymmetry ≠ publication bias proven`

`symmetry ≠ no missing evidence`

With only five studies, reject strong claims based on a visually symmetric funnel.

---

## Pass 15 — PRISMA transparency versus validity

Use PRISMA 2020 as a contrast source.

Prompt:

> Give me six reviews with different levels of PRISMA reporting completeness. Make me separate what I can audit from what I can conclude about methodological validity, risk of bias and certainty.

Required synthesis:

- reporting can be complete and methods still flawed;
- reporting can be incomplete and actual methods remain unknown rather than automatically wrong;
- PRISMA is not a quality score;
- formal RoB/GRADE judgments belong to F0.8.

---

## Pass 16 — integrated twelve-field audit

Use the exact synthetic case in `MANIFEST.md`.

Do not let NotebookLM answer it as a one-paragraph summary.

Require these headings, in order:

1. `Review question`
2. `Eligibility`
3. `Search/selection`
4. `Extraction/unit structure`
5. `Effect compatibility`
6. `Study estimates/precision`
7. `Weight/model`
8. `Clinical/methodological heterogeneity`
9. `Statistical heterogeneity`
10. `Sensitivity/subgroup/meta-regression prespecification`
11. `Missing-evidence/small-study signals`
12. `Pooling/conclusion defensibility`

Mandatory conclusions:

- A–E can be synthesized as MD if the review assumptions remain defensible;
- Study F's `SMD=0.60` cannot simply be inserted into the MD pool;
- random-effects pooled `+1.4` is an average under a model, not a universal effect;
- `I²=87%` demands interpretation, not automatic rejection;
- elite-status post hoc interaction is not a proven explanation because of non-prespecification, multiple moderators and collinearity with measurement setting;
- five-study funnel symmetry cannot prove no publication/non-reporting bias;
- PRISMA completeness cannot establish high certainty.

---

# 5. Final closed-book checkpoint

Without NotebookLM, notes or answer key, explain:

1. systematic review versus meta-analysis;
2. the review workflow;
3. study versus report;
4. compatibility before pooling;
5. inverse-variance weighting and why weight ≠ quality;
6. fixed-effect versus random-effects target quantities;
7. why random effects does not solve heterogeneity;
8. pooled CI versus prediction/between-study variation;
9. forest-plot anatomy and interpretation order;
10. clinical versus methodological versus statistical heterogeneity;
11. what I² means and at least four things it does not mean;
12. when not to pool;
13. sensitivity analysis versus result-shopping;
14. subgroup/meta-regression direct-comparison and multiplicity safeguards;
15. small-study effects and funnel-plot limits;
16. PRISMA function and limitation;
17. the complete twelve-field F0.7 audit sequence from memory.

If an answer begins with the pooled p-value/diamond without first defining the evidence body and compatibility, repeat the relevant pass.

---

# 6. Independent assessment protocol

Only after study:

1. close NotebookLM;
2. complete `foundations/F0-scientific-literacy/F0.7-systematic-reviews-meta-analysis-heterogeneity/EXERCISES.md` independently;
3. do not open `ANSWER_KEY.md` until the first attempt is complete;
4. submit the attempt for observed scoring;
5. route errors backward to F0.2/F0.5/F0.6/F0.7 as appropriate;
6. do not infer `MASTERED` from package completion or one isolated attempt.

Local unit gate remains:

`>=80/100 + no critical fail`

but applies only to actual observed performance.

---

# 7. Scope boundary with F0.8

Stop and label `F0.8` if a question requires formal:

- RoB 2 domain application;
- ROBINS-I judgment;
- ROB-ME formal judgment;
- GRADE certainty rating;
- certainty downgrading/upgrading logic;
- directness/indirectness formal judgment;
- applicability/transportability to a target athlete/context;
- recommendation strength.

F0.7 can identify that these questions matter, but does not certify answers to them.

---

# 8. Completion standard

The study package has done its job when the learner can take an unfamiliar systematic review/meta-analysis and reliably produce:

`Review question → Eligibility → Search/selection → Extraction/unit structure → Effect compatibility → Study estimates/precision → Weight/model → Clinical/methodological heterogeneity → Statistical heterogeneity → Sensitivity/subgroup/meta-regression prespecification → Missing-evidence/small-study signals → Pooling/conclusion defensibility`

without:

- treating systematic review and meta-analysis as synonyms;
- pooling incompatible measures by sign;
- treating weight as quality;
- treating fixed/random effects as good/bad labels;
- treating random effects as a heterogeneity cure;
- interpreting I² by threshold alone;
- treating post hoc subgroup/meta-regression as causal proof;
- diagnosing publication bias from funnel shape;
- using PRISMA as a quality/certainty score;
- replacing individual-study estimates/CIs and context with one pooled number.

Package completion itself still changes no learner state.
