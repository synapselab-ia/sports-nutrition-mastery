# F0.7 — Production QA Report

**Unit:** `F0.7 — Systematic reviews, meta-analyses and heterogeneity`

**Reviewed:** `2026-09-09`

**Production decision:** `APPROVED`

This QA records curriculum production only. It does **not** record learner study/performance and changes no mastery state.

---

## 1. Scope gate — PASS

Required by `COURSE_MAP.md` / `F0-A14`:

- systematic-review workflow from protocol/question through eligibility/search/screening/extraction/synthesis — covered;
- systematic review versus meta-analysis — explicitly separated;
- effect-measure compatibility before pooling — central teaching point;
- fixed-effect versus random-effects conceptual distinction — covered without declaring one universally superior;
- inverse-variance weighting intuition — P1 with arithmetic example;
- forest-plot anatomy and interpretation — covered;
- statistical versus clinical/methodological heterogeneity — explicitly separated;
- I² interpretation — covered with threshold/quality safeguards;
- when pooling is inappropriate — dedicated section;
- sensitivity analyses — covered;
- subgroup analyses — covered with interaction safeguard;
- meta-regression — conceptual level only;
- small-study effects/publication/non-reporting bias — introductory level;
- funnel-plot asymmetry — explicitly non-diagnostic;
- PRISMA — reporting guideline, not risk-of-bias/quality score;
- F0.5 magnitude/CI interpretation — preserved in all forest/pooled tasks;
- F0.6 multiplicity/prespecification — preserved in subgroup/meta-regression/sensitivity interpretation;
- performance task includes a heterogeneous five-study forest/synthesis scenario plus an incompatible sixth SMD study;
- performance task requires at least two clinical/methodological heterogeneity explanations before subgroup story;
- performance task requires defensible pooling judgment;
- full formal risk-of-bias/certainty/GRADE machinery remains F0.8.

No required F0-A14 element is missing.

---

## 2. Current external source recheck — PASS

Verification date: `2026-09-09`.

The unit intentionally uses only already-registered synthesis sources `F0-S03`, `F0-S04`, `F0-S05`, `F0-S06`. No duplicate/new source ID was required.

### `F0-S03` — PRISMA 2020

Current PRISMA Executive site and BMJ statement rechecked.

Verified:

- PRISMA 2020 remains the current general PRISMA statement;
- statement published 2021 and replaces PRISMA 2009;
- contains 27-item checklist plus expanded checklist, abstract checklist and flow diagrams;
- reporting items expose eligibility, information sources/search, selection, synthesis, heterogeneity investigation, sensitivity analyses, registration/protocol and related reporting.

Instructional limitation preserved:

- PRISMA is a reporting guideline;
- checklist completion is not used as proof of low risk of bias, high methodological quality or high certainty.

### `F0-S04` — Cochrane Handbook Chapter 10

Current official Chapter 10 page rechecked.

Verified:

- title remains *Analysing data and undertaking meta-analyses*;
- page citation states Chapter 10 last updated November 2024;
- page cites Handbook version 6.5 (Cochrane 2024);
- key points support weighted-average interpretation, inverse-variance framework, fixed/random-effects distinction, heterogeneity, subgroup/meta-regression cautions and sensitivity analysis;
- chapter explicitly states meta-analysis should only be considered when studies are sufficiently homogeneous in participants/interventions/outcomes to provide a meaningful summary;
- chapter warns that random effects is not a substitute for investigating heterogeneity;
- model choice should not be driven solely by a statistical heterogeneity test;
- I² thresholds are rough and can be misleading without magnitude/direction and uncertainty context.

Version nuance:

- Cochrane `Versions and changes` currently lists patch-level Handbook `6.5.1` changes during 2025/2026;
- those listed patch changes concern other chapters/corrections and do not replace the Chapter-10 citation or alter the F0.7 teaching points used here;
- the current Handbook landing page still labels the main edition `Version 6.5, 2024`.

### `F0-S05` — Cochrane Handbook current core methods

Current Handbook landing page rechecked.

Instructional use in F0.7:

- review workflow/question/eligibility/search/synthesis architecture;
- Chapter 13 missing-evidence/small-study-effects guidance.

Current Chapter 13 rechecked:

- last updated August 2024;
- funnel-plot asymmetry is framed as a generic small-study-effect signal with multiple possible explanations;
- non-reporting bias is one possible cause, not a diagnostic inference;
- asymmetry tests generally have low power and common guidance uses approximately 10 studies as a rule of thumb before considering many such tests;
- symmetry/asymmetry alone cannot settle missing-evidence bias.

F0.7 uses only introductory reasoning; formal ROB-ME application remains deferred to F0.8.

### `F0-S06` — Cochrane Chapter 6 effect measures

Current official Chapter 6 page rechecked.

Verified:

- page citation remains Handbook v6.5;
- chapter states last update August 2023;
- data types/effect measures remain MD/SMD for continuous outcomes and common ratio/difference measures for dichotomous outcomes;
- ratio measures are normally handled on logarithmic scales;
- study results may require conversion to consistent/usable forms before synthesis.

F0.7 uses this source to block direct numerical pooling of incompatible scales/measures.

No source-version change required revision of prerequisite F0.5/F0.6 content.

---

## 3. CONTENT_QA — PASS

### Review architecture

Verified:

- review and meta-analysis are distinct;
- study versus report distinction prevents duplicate counting conceptually;
- protocol, eligibility, search, screening, extraction and synthesis are ordered coherently;
- synthesis planning is framed as ideally prespecified rather than result-driven.

### Effect compatibility

Verified:

- same direction is explicitly insufficient for pooling;
- MD/SMD/RR/OR are not treated as numerically interchangeable;
- construct, direction, timepoint and unit structure are checked before pooling;
- log-scale ratio intuition is carried forward from F0.5.

### Inverse-variance arithmetic

Lesson example:

- `SE=0.20 → 1/SE² = 25`;
- `SE=0.40 → 1/SE² = 6.25`;
- relative inverse-variance weight ratio = `4:1`.

Arithmetic correct.

### Fixed/random effects

Verified:

- fixed-effect common-effect interpretation is stated as model/target assumption;
- random-effects average-of-related-effects interpretation is explicit;
- between-study variance is conceptually represented by `tau²`;
- random-effects weighting intuition uses `1/(SE²+tau²)` only as conceptual framework;
- random effects is not described as bias repair or heterogeneity erasure;
- fixed/random choice is not based solely on heterogeneity-test p-value.

### Forest plot

Verified:

- study point estimates, CIs, null line, weights, pooled diamond, scale and heterogeneity information are identified;
- pooled diamond is model-dependent and not labeled truth;
- difference null 0 and ratio null 1 remain consistent with F0.5.

### Heterogeneity

Verified:

- clinical diversity, methodological diversity and statistical heterogeneity are separate;
- methodological differences can create apparent statistical heterogeneity through differential bias;
- heterogeneity is not automatically interpreted as biological effect modification.

### I²

Verified safeguards:

- not percent of studies heterogeneous;
- not percent effect explained;
- not quality score;
- low I² does not prove identical studies;
- high I² does not automatically prohibit pooling;
- few-study uncertainty and contextual interpretation are explicit.

### Pooling decision

Verified:

- no-pooling is treated as a valid synthesis decision;
- clinical/methodological incompatibility can outweigh desire for a single number;
- high I² alone is not used as a binary stop rule.

### Sensitivity/subgroup/meta-regression

Verified:

- sensitivity analysis asks robustness to defensible assumptions;
- outcome-driven exclusions are distinguished from methodological sensitivity analysis;
- subgroup significance-label comparison is rejected;
- direct interaction reasoning is required;
- post hoc meta-regression is not treated as causal explanation;
- multiplicity/collinearity/few-study limits are explicit.

### Small-study/missing evidence

Verified:

- small-study effects have multiple causes;
- funnel asymmetry is not publication-bias proof;
- symmetry is not no-bias proof;
- five-study funnel example is explicitly too weak for strong inference;
- publication bias is nested within broader non-reporting/missing-evidence reasoning.

---

## 4. Quantitative synthetic scenario QA — PASS

Five-study compatible MD example uses:

| Study | MD | SE |
|---|---:|---:|
| A | +0.2 | 0.35 |
| B | +0.5 | 0.40 |
| C | +1.1 | 0.30 |
| D | +2.4 | 0.45 |
| E | +3.0 | 0.50 |

Approximate fixed-effect inverse-variance weights independently recalculated:

- A ≈ 23.7%;
- B ≈ 18.1%;
- C ≈ 32.2%;
- D ≈ 14.3%;
- E ≈ 11.6%.

Fixed-effect pooled MD independently recalculated:

`≈ +1.185`.

Cochran-Q-based illustrative inconsistency calculation for the supplied data yields:

`I² ≈ 87.3%`.

A conventional illustrative random-effects calculation produces an average close to:

`+1.40`, with approximate 95% CI `+0.44 to +2.36`.

Lesson/assessment round this to:

`+1.4 [0.4,+2.4]`.

This is labeled synthetic software output and is not used as empirical nutrition/performance evidence.

Study F is deliberately SMD on a different construct to test incompatible-pooling recognition.

---

## 5. EVIDENCE_QA — PASS

- reporting claims use PRISMA;
- weighting/model/heterogeneity claims use Cochrane Chapter 10;
- effect-scale compatibility uses Cochrane Chapter 6;
- small-study/non-reporting claims use current Cochrane core/Chapter 13 guidance;
- no substantive intervention claim is made from synthetic performance examples;
- no reporting guideline is converted into risk-of-bias/certainty certification;
- no statistical heterogeneity metric is converted into study quality;
- no subgroup/meta-regression association is presented as causal mechanism;
- no funnel-plot pattern is diagnosticized as publication bias.

No cherry-picking issue applies to a treatment-effect conclusion because F0.7 is a methodological unit and all applied effects are synthetic.

---

## 6. PEDAGOGICAL_QA — PASS

### P2 integrity

F0.7 learner validation requires:

- F0.2 study-design architecture;
- F0.5 effect measures + estimate/CI;
- F0.6 multiplicity/prespecification;
- F0.3 before formal risk-of-bias synthesis.

The lesson explicitly reconnects these dependencies and does not mark them learned.

### Progression

The lesson progresses:

`review vs meta-analysis → workflow → PRISMA → effect compatibility → weighted average → inverse variance → fixed/random effects → prediction interval intuition → forest plot → heterogeneity layers → I² → pooling decision → sensitivity → subgroup/meta-regression → small-study/missing evidence → integrated audit`.

### P1 bridges

- inverse-variance arithmetic included;
- forest-plot anatomy taught explicitly;
- ratio log-scale reminder included;
- interaction reasoning reused from F0.6;
- prediction interval distinguished from pooled-mean CI without derivation burden.

### Anti-memorization

Assessment requires:

- workflow reconstruction;
- compatibility audit;
- inverse-variance calculation;
- fixed/random error repair;
- forest-plot reconstruction;
- heterogeneity classification;
- I² misconception repair;
- sensitivity-analysis judgment;
- subgroup/meta-regression critique;
- funnel/missing-evidence critique;
- integrated pooling decision.

---

## 7. MASTERY_QA — PASS

Assessment mapping:

- `K1`: systematic review/meta-analysis/heterogeneity/weight definitions;
- `K2`: review workflow and forest-plot structure;
- `K3`: fixed/random and heterogeneity distinctions;
- `K4`: pooled estimate/CI/I²/funnel interpretation;
- `K5`: predict consequences of incompatible pooling/heterogeneity/missing evidence;
- `K6`: inverse-variance calculation and forest application;
- `K7`: integrate F0.2/F0.5/F0.6;
- `K8`: recognize pooling, PRISMA, subgroup and small-study limits.

Local gate:

`>=80/100 + no critical fail`.

This gate can alter learner state only after actual observed responses.

Critical fails match F0-A14 and include all required structural misconceptions.

---

## 8. Performance-task QA — PASS

Integrated task contains:

- prespecified review protocol/question;
- search/reporting information;
- five compatible MD studies;
- heterogeneous study effects;
- fixed versus random outputs;
- high I²;
- one deliberately incompatible SMD study;
- multiple post hoc moderators;
- collinearity between elite status and measurement setting;
- subgroup interaction p=0.04;
- five-study funnel-plot overclaim;
- complete PRISMA reporting;
- overconfident pooled conclusion.

Required response reconstructs:

- process strengths/limits;
- compatibility;
- weights;
- pooled result;
- heterogeneity;
- alternative explanations;
- subgroup/meta-regression status;
- missing evidence;
- PRISMA boundary;
- defensible pooling/conclusion.

This directly satisfies the F0-A14 performance requirement.

---

## 9. F0.7 → F0.8 boundary — PASS

F0.7 does **not** formally teach:

- RoB 2 domain judgments;
- ROBINS-I application;
- ROB-ME formal signaling/judgment algorithm;
- GRADE certainty ratings;
- certainty downgrade decisions;
- applicability/indirectness rating;
- recommendation strength.

These remain F0.8.

F0.7 may identify that bias/missing evidence matters, but does not certify certainty.

---

## 10. Public repository / privacy / copyright — PASS

- no learner health/personal data;
- no fabricated learner performance;
- all applied numerical examples are synthetic;
- no third-party PDF/full article/chapter is committed;
- only project-authored Markdown, references/source IDs and links are stored;
- no substantive sports-nutrition recommendation is inferred from the examples.

---

## 11. Production/learning separation — PASS

After F0-A14 production:

- F0.1 learner state remains pending;
- F0.2 remains pending;
- F0.3 remains pending;
- F0.4 remains pending;
- F0.4 quantitative diagnostic remains `UNOBSERVED`;
- F0.5 remains pending;
- F0.6 remains pending;
- F0.7 remains `UNSEEN`.

No mastery state is changed from curriculum production.

---

## 12. Final gate

> Can a learner with F0.2/F0.5/F0.6 prerequisites distinguish systematic review from meta-analysis, reconstruct the review workflow, verify effect compatibility, interpret weights/fixed/random models/forest plots, reason about clinical-methodological-statistical heterogeneity and I², judge whether pooling is meaningful, critique subgroup/meta-regression/sensitivity analyses and reason about small-study/missing-evidence signals without converting PRISMA or a pooled estimate into a quality/truth certificate?

**Decision:** yes.

**Production state:** `APPROVED`.
