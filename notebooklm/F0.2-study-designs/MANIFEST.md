# F0.2 — NotebookLM Manifest

**Package state:** `READY_FOR_STUDY`
**Manifest version:** `1`
**Built/verified:** `2026-09-08`
**Learner state affected:** none

This manifest defines the approved, deliberately small NotebookLM corpus for `F0.2 — Study designs and what they can answer`. GitHub remains canonical; NotebookLM is a source-controlled study layer.

The corpus is intentionally limited to six sources. Separate crossover and cluster CONSORT extensions are **not** loaded into the first-pass notebook because Cochrane Chapter 23 already provides the required crossover/cluster architecture and the canonical lesson translates it into F0.2-level reasoning. This avoids redundant source loading while preserving design coverage.

```yaml
module_id: "F0.2"
module_title: "Study designs and what they can answer"
version: 1
learning_objectives:
  - "Classify common human-research designs from their architecture rather than from superficial labels."
  - "Distinguish randomized parallel, crossover, cluster and factorial trials and state the comparison structure each creates."
  - "Distinguish between-subject from within-subject comparisons and explain when each is structurally appropriate."
  - "Explain washout, carryover and period effects and use them to judge whether crossover is suitable for a question."
  - "Distinguish unit of allocation, unit of observation and unit of analysis in cluster-randomized trials."
  - "Distinguish non-randomized intervention studies, cohort, case-control and cross-sectional designs from the direction of sampling/time rather than from the age of the data."
  - "Separate acute mechanistic questions from chronic adaptation/outcome questions."
  - "Recognize diagnostic and prognostic questions as distinct design problems rather than forcing them into an intervention hierarchy."
  - "Explain the introductory target-trial concept and why emulating a target trial does not manufacture randomization."
  - "For every study design, state the strongest defensible inference and at least one tempting inference the design does not establish."

sources:
  - source_id: "F0-R02"
    priority: "CORE"
    citation: "Sports Nutrition Mastery. F0.2 — Desenhos de estudo e o que eles podem responder. Canonical project lesson, version current at manifest v1."
    url_or_doi: "https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.2-study-designs/LESSON.md"
    why_included: "Primary instructional spine. It integrates randomized and observational designs into the project's required reasoning sequence: question → origin of contrast → temporal direction → unit of allocation → comparison structure → strongest defensible inference → tempting unsupported inference."

  - source_id: "F0-S22"
    priority: "CORE"
    citation: "Higgins JPT, Eldridge S, Li T. Chapter 23: Including variants on randomized trials. In: Higgins JPT, Thomas J, Chandler J, et al., eds. Cochrane Handbook for Systematic Reviews of Interventions. Version 6.5. Cochrane; 2024. Chapter last updated October 2019."
    url_or_doi: "https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-23"
    why_included: "Authoritative design-methods anchor for cluster-randomized and crossover trials. It makes unit of allocation, clustering/dependence, within-person structure, crossover suitability, carryover and period issues explicit. Use the design concepts; defer meta-analysis/statistical machinery beyond F0.2."

  - source_id: "F0-S01"
    priority: "SUPPORT"
    citation: "Hopewell S, Chan A-W, Collins GS, et al. CONSORT 2025 statement: updated guideline for reporting randomised trials. BMJ. 2025;389:e081123. doi:10.1136/bmj-2024-081123."
    url_or_doi: "https://www.bmj.com/content/389/bmj-2024-081123"
    why_included: "Current general randomized-trial reporting standard. It helps the learner identify allocation, intervention groups, outcomes, participant flow, protocol/registration information and other architecture needed to reconstruct a trial. It is reporting guidance, not a risk-of-bias or quality score."

  - source_id: "F0-S25"
    priority: "SUPPORT"
    citation: "Kahan BC, Juszczak E, Beller E, et al. Guidance for protocol content and reporting of factorial randomised trials: explanation and elaboration of the CONSORT 2010 and SPIRIT 2013 extensions. BMJ. 2025;388:e080785. doi:10.1136/bmj-2024-080785. Related factorial CONSORT extension: Kahan BC, Hall SS, Beller EM, et al. JAMA. 2023;330(21):2106-2114. doi:10.1001/jama.2023.19793."
    url_or_doi: "https://www.bmj.com/content/388/bmj-2024-080785"
    why_included: "Open-access explanation/elaboration for factorial trial architecture. It teaches why multiple factors are randomized, how main comparisons are defined, why interaction matters, and why effects of two factors must not be assumed automatically additive. Detailed interaction statistics remain deferred to F0.6."

  - source_id: "F0-S02"
    priority: "SUPPORT"
    citation: "von Elm E, Altman DG, Egger M, Pocock SJ, Gøtzsche PC, Vandenbroucke JP; STROBE Initiative. The Strengthening the Reporting of Observational Studies in Epidemiology (STROBE) statement. J Clin Epidemiol. 2008;61(4):344-349. doi:10.1016/j.jclinepi.2007.11.008."
    url_or_doi: "https://www.strobe-statement.org/"
    why_included: "Compact official support for distinguishing the three major analytical observational designs taught in F0.2: cohort, case-control and cross-sectional. It is used to identify what design information should be visible, never as a methodological-quality score or proof of causality."

  - source_id: "F0-S17"
    priority: "CONTRAST"
    citation: "Hernán MA, Dahabreh IJ, Dickerman BA, Swanson SA. The Target Trial Framework for Causal Inference From Observational Data: Why and When Is It Helpful? Ann Intern Med. 2025;178(3):402-407. doi:10.7326/ANNALS-24-01871."
    url_or_doi: "https://pmc.ncbi.nlm.nih.gov/articles/PMC11936718/"
    why_included: "Contrast source for observational causal questions. It teaches the discipline of specifying the hypothetical randomized target trial before emulation, while making clear that observational emulation does not create randomization or eliminate data/assumption limitations."

claims_to_master:
  - "Study design is architecture relative to a scientific question, not a universal prestige ranking."
  - "Randomization is an allocation mechanism that improves causal comparability in expectation; it does not guarantee perfect baseline equality, flawless execution, representative sampling or universal applicability."
  - "A parallel randomized trial is primarily a between-subject comparison; a crossover trial is primarily a within-subject comparison in which participants receive multiple conditions across periods."
  - "Crossover requires a sufficiently stable setting and effects that are reversible/transient enough for sequence, washout, carryover and period effects to be managed."
  - "Washout is the interval intended to reduce persistence of a prior condition; carryover is persistence of a prior condition into a later period."
  - "In cluster trials, the randomized unit can be a team/clinic/school while outcomes are measured on individuals; the observed individuals are not thereby independent randomized units."
  - "A factorial randomized trial evaluates multiple randomized factors; the effect of one factor may depend on the level of another, so simple additivity is not guaranteed."
  - "A non-randomized intervention can establish temporal change/differences under an intervention without becoming automatically causal merely because investigators introduced the intervention."
  - "A cohort starts from exposure/baseline and follows toward outcomes; a case-control study samples by outcome status and reconstructs prior exposure; a cross-sectional study measures exposure/outcome in an essentially contemporaneous window."
  - "Retrospective use of historical data does not by itself define case-control design; sampling logic does."
  - "Temporal ordering strengthens interpretation in longitudinal designs but is not, by itself, proof of causality."
  - "An acute mechanistic outcome directly answers an acute/mechanistic question; chronic hypertrophy, performance, composition-body or health conclusions require evidence at the corresponding outcome and time scale."
  - "Diagnostic accuracy, prognosis, prevalence, rare harms and intervention effects are different questions that may require different optimal designs."
  - "Target-trial thinking clarifies eligibility, strategies, time zero, follow-up, outcome, causal contrast and analysis target before observational emulation; it does not manufacture random allocation."
  - "For any unfamiliar study, the learner should be able to state both the strongest defensible inference and a tempting unsupported inference."

controversies_or_limits:
  - "CONSORT 2025 is the current general CONSORT statement. Design-specific crossover/cluster/factorial extensions were developed against CONSORT 2010; this package uses current CONSORT 2025 generally and uses design-specific material only for architecture not replaced by the general update."
  - "Cochrane Chapter 23 belongs to Handbook v6.5 (2024) but the chapter itself was last updated in October 2019. It remains the current Handbook chapter located for cluster/crossover variants; its statistical/meta-analytic detail exceeds F0.2."
  - "STROBE explicitly describes reporting recommendations for cohort, case-control and cross-sectional studies. It is not a prescription for study design/conduct and not an instrument for evaluating methodological quality."
  - "The factorial explanation/elaboration is about reporting/protocol transparency. Its treatment of factor structure and interaction is useful pedagogically, but reporting compliance does not establish low risk of bias."
  - "Target-trial emulation applies to causal intervention questions that can be meaningfully specified as a hypothetical trial. It is not a universal template for prevalence, descriptive, diagnostic or every prognostic question."
  - "F0.2 intentionally stops before formal confounding, selection-bias, measurement-bias, missing-data and causal-identification analysis; those are F0.3 topics."
  - "The package does not teach interaction-test mathematics, multiplicity adjustment or power calculations; those belong to later quantitative units."

active_recall:
  basic:
    - "Define allocation, follow-up, exposure, unit of allocation, unit of observation and unit of analysis."
    - "What structural feature distinguishes a randomized parallel trial from a randomized crossover trial?"
    - "Define washout, carryover and period effect in your own words."
    - "What is randomized in a cluster-randomized trial?"
    - "What is a 2 × 2 factorial design?"
    - "How does a cohort differ from a case-control study when both use historical records?"
    - "What is the strongest structural inference of a cross-sectional study?"
  mechanism:
    - "Explain step by step why crossover can reduce between-person variability but become invalid for a persistent adaptation such as long-term hypertrophy."
    - "Explain why athletes within the same randomized team cannot be interpreted as independently randomized individuals."
    - "Explain why temporal ordering helps a cohort yet cannot alone establish causality."
    - "Explain why an acute molecular response can be mechanistically informative without answering a chronic adaptation question."
  evidence_critique:
    - "Use Cochrane Chapter 23 to compare cluster and crossover architecture: unit randomized, dependence structure, repeated measurements, and design-specific failure modes."
    - "Using CONSORT 2025, identify which reported elements would let you reconstruct who was randomized, to what, for how long, and for which outcomes—then explain why this does not amount to a quality score."
    - "Using STROBE, distinguish cohort, case-control and cross-sectional reporting targets, then state one causal conclusion that remains unsupported by the reporting guideline itself."
    - "Using the factorial guidance, explain why A and B showing effects in a factorial trial does not logically imply that A+B equals the sum of the two effects."
    - "Using the target-trial paper, list the elements of a hypothetical target trial and identify what observational emulation still cannot create."
  integration:
    - "Classify an unfamiliar study description, then state: question type → origin of contrast → temporal direction → between/within-subject structure → unit of allocation → strongest defensible inference → tempting unsupported inference."
    - "Design one acute nutrition-performance question that is suitable for crossover and one chronic adaptation question that is unsuitable for crossover; justify the difference using carryover/reversibility."
    - "Construct a cluster trial in sports nutrition and identify three distinct units: allocation, observation and analysis."
    - "Convert one observational causal question into a target-trial specification, then state which assumptions/data problems would remain after emulation."
    - "Give one example each of a question best answered primarily by a randomized trial, cohort, case-control and cross-sectional design; justify by question rather than evidence hierarchy."

notebooklm_tasks:
  - "Act as a Socratic examiner. Present one unfamiliar study description at a time and wait for the learner to classify it before revealing any answer."
  - "For every study-description exercise, require exactly two final sentences: 'Strongest defensible inference:' and 'Tempting unsupported inference:'."
  - "Generate paired examples that differ by only one architectural feature—for example cohort versus case-control sampling, parallel versus crossover comparison, or individual versus cluster allocation—and require the learner to explain why the design label changes."
  - "Create crossover scenarios and ask whether washout is biologically plausible; include at least one persistent/chronic intervention where crossover should be rejected."
  - "Create cluster-trial scenarios where the number of observed individuals is much larger than the number of randomized clusters and require the learner to identify the randomized unit."
  - "Create 2 × 2 factorial scenarios and ask what the two factors are, which main contrasts exist, and why interaction prevents assuming simple additivity."
  - "Alternate cohort, case-control and cross-sectional descriptions using both prospective and retrospective data so the learner cannot classify by the word 'retrospective' alone."
  - "Generate acute mechanistic findings and ask the learner to rewrite exaggerated chronic conclusions so the scope matches the measured outcome/time window."
  - "Use the target-trial source to make the learner specify eligibility, strategies, assignment, time zero, follow-up, outcome and causal contrast before discussing observational emulation."
  - "For every explanation, cite only the approved corpus and distinguish reporting guidance from causal/risk-of-bias judgment."
  - "Never treat a NotebookLM-generated statement that lacks support in the approved corpus as canonical project knowledge."
```

## Evidence-critique task

Use `F0-S17` (target-trial framework) together with the canonical F0.2 lesson and produce a concise design appraisal of a hypothetical observational causal question:

> Among resistance-trained adults, does beginning strategy A rather than strategy B at the start of a 12-week training block improve the change in a prespecified performance outcome?

Your appraisal must:

1. write the hypothetical target-trial eligibility criteria;
2. define strategies A and B precisely enough to be assigned in principle;
3. define `time zero` and explain why eligibility, strategy assignment and follow-up should align there;
4. define the outcome and 12-week follow-up window;
5. state the causal contrast/target quantity in plain language;
6. state what observational data would have to contain to emulate this design plausibly;
7. explain why emulation still does **not** create randomization;
8. state the strongest defensible inference that could follow from a well-specified observational emulation **without prematurely claiming that confounding has been solved**;
9. state at least two tempting unsupported inferences;
10. finish by naming which unresolved causal-validity questions are intentionally deferred to F0.3.

**Scoring principle:** explicit design structure and inferential restraint matter more than using advanced causal terminology.

## Corpus exclusions

Do **not** add these to the initial NotebookLM corpus:

- `foundations/F0-scientific-literacy/F0.2-study-designs/ANSWER_KEY.md` — exclusion prevents answer leakage;
- `foundations/F0-scientific-literacy/F0.2-study-designs/EXERCISES.md` — keep the independent assessment outside the study corpus;
- `foundations/F0-scientific-literacy/F0.2-study-designs/QA_REPORT.md` — production metadata, not instructional evidence;
- the full `SOURCE_INDEX.md` — registry metadata would add noise;
- separate crossover/cluster CONSORT extension papers in the first pass — their essential F0.2 architecture is already represented by Cochrane Chapter 23 plus the canonical lesson;
- `F0-S16` full causal-inference textbook — valuable teacher reference but too broad/advanced for the deliberately small first-pass F0.2 NotebookLM corpus;
- F0.3 risk-of-bias/confounding sources — they would prematurely expand the unit beyond its intended scope.

`EXERCISES.md` must be completed independently after the NotebookLM study sequence, before consulting `ANSWER_KEY.md`.

## Version integrity

The corpus was verified on 2026-09-08 against the current accessible sources:

- CONSORT 2025 remains the current general randomized-trial statement;
- Cochrane Handbook Chapter 23 is currently presented under Handbook version 6.5 (2024), with the chapter itself last updated October 2019;
- STROBE's official site continues to identify cohort, case-control and cross-sectional as the three principal analytical designs covered by the statement and explicitly says the checklist is not a quality instrument;
- the factorial CONSORT extension is the 2023 JAMA extension, with a 2025 BMJ explanation/elaboration available openly;
- the target-trial framework article is the 2025 Annals of Internal Medicine paper, DOI `10.7326/ANNALS-24-01871`, with full text available through PMC.

If any source, lesson or learning objective changes materially, increment `version` and rebuild/QA the package before treating the NotebookLM corpus as current.
