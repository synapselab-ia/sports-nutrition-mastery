# F0.1 — NotebookLM Manifest

**Package state:** `READY_FOR_STUDY`
**Manifest version:** `1`
**Built/verified:** `2026-09-08`
**Learner state affected:** none

This manifest defines the approved, auditably small NotebookLM corpus for `F0.1 — Scientific questions, hypotheses and operationalization`. GitHub remains canonical; NotebookLM is a source-controlled study layer.

```yaml
module_id: "F0.1"
module_title: "Scientific questions, hypotheses and operationalization"
version: 1
learning_objectives:
  - "Transform a vague sports-nutrition/performance claim into an empirically answerable question with explicit population, contrast, outcome and time window."
  - "Distinguish construct, operational definition, variable, outcome/endpoint and estimand."
  - "Distinguish directional from non-directional hypotheses and explain why falsifiability alone does not rescue poor operationalization."
  - "Distinguish prespecified confirmatory reasoning from transparent exploratory/post-hoc hypothesis generation."
  - "Explain the roles of primary, secondary and exploratory outcomes without treating them as interchangeable."
  - "Construct an introductory estimand before choosing an estimator or statistical analysis."
  - "Detect inferential overreach from an acute mechanistic outcome to chronic hypertrophy, performance or health claims."

sources:
  - source_id: "F0-R01"
    priority: "CORE"
    citation: "Sports Nutrition Mastery. F0.1 — Perguntas científicas, hipóteses e operacionalização. Canonical project lesson, version current at manifest v1."
    url_or_doi: "https://github.com/synapselab-ia/sports-nutrition-mastery/blob/main/foundations/F0-scientific-literacy/F0.1-scientific-questions/LESSON.md"
    why_included: "Primary instructional spine. It integrates the approved methodological sources into the vocabulary, sequence, sports-nutrition examples and inferential boundaries expected from the learner."

  - source_id: "F0-S05"
    priority: "CORE"
    citation: "Higgins JPT, Thomas J, Chandler J, et al., eds. Cochrane Handbook for Systematic Reviews of Interventions. Version 6.5. Cochrane; 2024. Especially Chapter 2: Determining the scope of the review and the questions it will address."
    url_or_doi: "https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-02"
    why_included: "Authoritative methodological support for why well-formulated questions matter and how explicit population, intervention, comparator and outcomes constrain evidence selection and interpretation."

  - source_id: "F0-S14"
    priority: "CORE"
    citation: "International Council for Harmonisation. ICH E9 Statistical Principles for Clinical Trials and ICH E9(R1) Addendum on Estimands and Sensitivity Analysis in Clinical Trials."
    url_or_doi: "https://www.ema.europa.eu/en/ich-e9-statistical-principles-clinical-trials-scientific-guideline"
    why_included: "Primary methodological anchor for introductory estimand thinking: define the treatment-effect/scientific question and target quantity before selecting the estimator or analysis."

  - source_id: "F0-S15"
    priority: "CORE"
    citation: "GRADE Working Group. The GRADE Book. Chapter family: Making answerable questions. Living official resource."
    url_or_doi: "https://book.gradepro.org/"
    why_included: "Current official support for converting broad decision questions into explicit answerable questions and recognizing that question structure constrains later evidence judgments."

  - source_id: "F0-S01"
    priority: "SUPPORT"
    citation: "Hopewell S, Chan A-W, Collins GS, et al. CONSORT 2025 statement: updated guideline for reporting randomised trials. BMJ. 2025;389:e081123. doi:10.1136/bmj-2024-081123."
    url_or_doi: "https://www.bmj.com/content/389/bmj-2024-081123"
    why_included: "Supports transparent reporting of objectives, outcomes, prespecification-related materials and the distinction between what was planned and what was reported. Used as reporting guidance, not as a risk-of-bias or study-quality score."

  - source_id: "F0-S21"
    priority: "CONTRAST"
    citation: "Areta JL, Burke LM, Ross ML, et al. Timing and distribution of protein ingestion during prolonged recovery from resistance exercise alters myofibrillar protein synthesis. J Physiol. 2013;591(9):2319-2331. doi:10.1113/jphysiol.2012.244897."
    url_or_doi: "https://pmc.ncbi.nlm.nih.gov/articles/PMC3650697/"
    why_included: "Full-text sports-nutrition transfer case. The learner must reconstruct what was operationalized and contrast the acute mechanistic question with tempting but unsupported chronic hypertrophy/performance claims."

claims_to_master:
  - "A scientific question acts as a contract of interpretation: population, contrast, outcome and time constrain what a result can legitimately answer."
  - "PICO(T) is a decomposition aid for relevant question types; filling its letters mechanically does not guarantee a precise or important question."
  - "A construct is theoretical; an operational definition specifies how it becomes observable; a variable can vary; an outcome is a result of interest; an estimand is the target quantity whose value would answer the scientific question."
  - "Operationalization changes the empirical meaning of a construct; two studies can use the same label while measuring meaningfully different outcomes."
  - "A falsifiable hypothesis can still be scientifically weak if its population, contrast, measurement or time window is vague."
  - "Exploratory analysis is legitimate when transparently labeled; a post-hoc pattern must not be rewritten as a prespecified confirmatory hypothesis."
  - "Primary, secondary and exploratory outcomes have different interpretive roles; a favorable secondary/exploratory result must not be silently promoted to the original primary question."
  - "An estimand is defined before the estimator: question → estimand → design/data → estimator/analysis → estimate → interpretation."
  - "An acute mechanistic outcome can be biologically informative without directly establishing chronic hypertrophy, performance or health effects."

controversies_or_limits:
  - "PICO is especially useful for intervention-effect questions but is not a universal framework for every scientific question; the learner should not force all research into PICO."
  - "ICH E9(R1) was written for regulated clinical trials. F0.1 borrows its estimand logic conceptually and does not import every regulatory or statistical requirement into sports science."
  - "CONSORT 2025 is a reporting guideline. Complete checklist reporting does not prove low risk of bias, correct design or causal validity."
  - "The GRADE Book is oriented toward evidence synthesis and decision questions; it supports question framing here but is not the sole authority for basic/mechanistic hypothesis formulation."
  - "F0-S21 studied 24 trained men, a single resistance-exercise setting, fixed total whey protein (80 g) distributed across 12 h, with acute integrated myofibrillar protein synthesis among the outcomes. Its scope does not establish a universal long-term protein-distribution prescription."

active_recall:
  basic:
    - "Define population-alvo and sample, then explain why confusing them can produce an overgeneralized conclusion."
    - "Define construct, operational definition, variable, outcome/endpoint and estimand without using the terms as synonyms."
    - "What four elements must be identifiable in the minimum F0.1 question skeleton, and when does time become essential?"
    - "What is the difference between a directional and a non-directional hypothesis?"
    - "What is the role of a primary outcome?"
  mechanism:
    - "Explain step by step how a vague construct such as 'recovery' can enable outcome switching or interpretive overreach."
    - "Explain why defining the estimand before the estimator protects the scientific question from being reshaped around whichever analysis is convenient."
    - "Explain why prespecification changes the evidential status of a finding without making a study automatically valid."
  evidence_critique:
    - "Using CONSORT 2025, identify which reporting elements help a reader distinguish planned objectives/outcomes from undeclared post-hoc changes, while explaining why CONSORT itself is not a risk-of-bias score."
    - "Using F0-S21, reconstruct the actual population, conditions compared, outcome and time window, then list at least four conclusions the experiment does not directly establish."
    - "Find one place where a source uses broad language such as 'effect' or 'outcome' and rewrite it as a more explicit target quantity suitable for F0.1."
  integration:
    - "Take the claim 'creatine improves performance' and produce: vague-term audit → answerable PICO(T) → directional hypothesis → operationalized outcome → introductory estimand → one result that would count against the hypothesis → one tempting unsupported conclusion."
    - "Compare Cochrane question framing with ICH E9(R1) estimand thinking: what problem does each solve, and where do they overlap?"
    - "Explain how the same construct can yield two legitimate but non-equivalent scientific questions because the outcome or time window differs."
    - "Build an example in which an exploratory result is scientifically valuable but would become misleading if reported as confirmatory."

notebooklm_tasks:
  - "Act as a Socratic tutor. Ask one active-recall question at a time, wait for the learner's answer, then grade it against the approved sources before showing corrections."
  - "For every explanation, cite the specific approved source and distinguish project synthesis from claims directly stated in external sources."
  - "Create a comparison table with columns: source, question-framing contribution, estimand/outcome contribution, limitation for F0.1, and misuse to avoid."
  - "Use the Areta paper as an evidence-boundary exercise: separate what was measured from what a social-media post might incorrectly infer about months-long hypertrophy or universal protein timing."
  - "Generate three new sports-nutrition claims not used in the lesson and require the learner to convert each into an answerable question before discussing any evidence."
  - "Never treat a NotebookLM-generated statement that lacks support in the approved corpus as canonical project knowledge."
```

## Evidence-critique task

Use the full text of `F0-S21` (Areta et al. 2013) and produce a one-page appraisal limited to F0.1 competencies:

1. state the broad claim/topic that a casual reader might infer from the title;
2. reconstruct the most defensible scientific question from the actual methods;
3. identify population, conditions compared, total protein/source, outcome and measurement window;
4. distinguish construct from the exact operational outcome;
5. write an introductory estimand/target quantity in plain language;
6. identify which conclusions are directly supported by the measured acute outcome;
7. list at least four chronic, practical or population-general claims that remain unsupported by this experiment alone;
8. identify any ambiguity in the paper about what was primary/secondary rather than inventing a hierarchy not clearly reported;
9. finish with a two-sentence conclusion whose certainty and scope exactly match the study question.

**Scoring principle:** precision of scope is more important than producing a favorable or unfavorable conclusion about protein timing.

## Corpus exclusions

Do **not** add these to the initial NotebookLM corpus:

- `ANSWER_KEY.md` — exclusion prevents answer leakage before the learner attempts retrieval/application;
- `QA_REPORT.md` — production metadata, not instructional evidence;
- the entire `SOURCE_INDEX.md` — useful registry but unnecessarily expands the study corpus;
- unrelated F0.2+ methodological sources — they introduce concepts before their scheduled units.

`EXERCISES.md` is an assessment artifact rather than an evidence source. Keep it outside NotebookLM during initial study and complete it independently after the source-guided study sequence.

## Version integrity

If any source, lesson or learning objective changes materially, increment `version` and rebuild/QA the package before treating the NotebookLM corpus as current.
