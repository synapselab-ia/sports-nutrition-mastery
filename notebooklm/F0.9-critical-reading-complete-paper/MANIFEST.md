# F0.9 — NotebookLM Manifest

**Package state:** `READY_FOR_STUDY`
**Manifest version:** `1`
**Built/verified:** `2026-09-10`
**Learner state affected:** none
**F0.4 quantitative diagnostic affected:** none; remains `UNOBSERVED`

This manifest defines the approved first-pass NotebookLM corpus for `F0.9 — Critical reading of a complete paper`. GitHub remains canonical; NotebookLM is a controlled study layer.

The corpus is intentionally limited to **seven sources**. It contains the canonical F0.9 lesson, the real full-paper appraisal object and its registry companion, plus only four methodological supports needed to preserve the unit's core boundaries.

The required appraisal sequence is:

`1. Question/estimand → 2. Design/sampling → 3. Intervention/exposure/comparator → 4. Outcome measurement → 5. Bias/confounding/missingness → 6. Sample size/analysis plan → 7. Effect estimate/uncertainty → 8. Multiplicity/exploration → 9. Result robustness → 10. Applicability → 11. Consistency with authors’ conclusion → 12. What the paper does not establish`

The first-pass notebook must train **independent reconstruction**. It must not import the completed appraisal from `EXERCISES.md` or `ANSWER_KEY.md`.

```yaml
module_id: "F0.9"
module_title: "Critical reading of a complete paper"
version: 1
learning_objectives:
  - "Appraise a complete paper from question through conclusion rather than accepting title, abstract or discussion as the analysis."
  - "Navigate main text, supplement, registry, protocol, SAP and data/code resources while preserving source provenance and timestamps."
  - "Extract a compact PICO/estimand table before interpretation."
  - "Extract a result table containing outcome/timepoint, contrast, effect measure, point estimate, uncertainty, statistical output, analysis population, prespecification status, practical threshold and caveat."
  - "Apply the fixed twelve-step F0.9 appraisal sequence without replacing reasoning with a checklist score."
  - "Distinguish within-group change from between-group treatment effect."
  - "Interpret magnitude and confidence intervals before binary significance labels."
  - "Reject p>0.05 as automatic evidence of no effect or equivalence."
  - "Separate prospective sample-size/power planning from completed-study precision and from observed/post-hoc power."
  - "Use registry/protocol/SAP timestamps to classify evidence for prespecification rather than assuming that a document's existence proves prospectivity."
  - "Map multiplicity across outcomes, timepoints, contrasts, subgroups, models and analytical choices."
  - "Use result-specific bias mechanisms rather than a total study-quality score."
  - "Distinguish robustness analysis from result-shopping."
  - "Use reporting guidance to locate information without converting reporting completeness into validity."
  - "Audit applicability across population, intervention/exposure, comparator, outcome, time horizon, setting and decision context."
  - "Distinguish appraisal of one paper from certainty of a body of evidence."
  - "Judge whether the authors' conclusion is proportional to the measured estimand and observed uncertainty."
  - "End every appraisal with an explicit strongest defensible inference and what the paper does not establish."

sources:
  - source_id: "F0-R09"
    priority: "CORE"
    citation: "Sports Nutrition Mastery. F0.9 — Critical reading of a complete paper. Canonical project lesson, current at manifest v1."
    url_or_doi: "https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.9-critical-reading-complete-paper/LESSON.md"
    why_included: "Primary instructional spine defining the exact twelve-step appraisal workflow, extraction tables, navigation rules, F0.1–F0.8 integration, critical fails and the boundary between paper appraisal and F0.10 communication."
    limitation: "Project-authored teaching material, not an independent methodological authority. Material methodological claims remain traceable to the external sources below."

  - source_id: "F0-S30"
    priority: "CORE"
    citation: "Klemp AO, Ormsbee MJ, Yeh M, et al. Neither pre-sleep nor post-exercise protein consumption influences resistance exercise training adaptations in older adults. Journal of the International Society of Sports Nutrition. 2025;22(1):2519511. doi:10.1080/15502783.2025.2519511."
    url_or_doi: "https://pmc.ncbi.nlm.nih.gov/articles/PMC12897527/"
    why_included: "Real human exercise/nutrition full-paper study object. It contains enough design, intervention, outcome, longitudinal-analysis, uncertainty, multiplicity, open-science and registration information to require integrated use of F0.1–F0.8."
    limitation: "A single study cannot establish body-of-evidence certainty or a universal nutrition recommendation. The learner must derive appraisal judgments from the full text and companion sources rather than from the paper's title or conclusion."

  - source_id: "F0-S31"
    priority: "SUPPORT"
    citation: "ClinicalTrials.gov. NCT05922475 — Efficacy of Pre-sleep or Post-exercise Protein During 12 Weeks of Resistance Exercise Training. Florida State University."
    url_or_doi: "https://clinicaltrials.gov/study/NCT05922475"
    why_included: "External registry/timeline companion for the full paper. It lets the learner inspect registration dates, study dates, intervention arms, outcome records and version history when evaluating prespecification and transparency."
    limitation: "A registry record is an audit source, not a validity certificate. Its evidentiary value for prespecification depends on timing and version history, which the learner must reconstruct rather than assume."

  - source_id: "F0-S01"
    priority: "SUPPORT"
    citation: "Hopewell S, Chan A-W, Collins GS, et al. CONSORT 2025 statement: updated guideline for reporting randomised trials. BMJ. 2025;389:e081123. doi:10.1136/bmj-2024-081123."
    url_or_doi: "https://doi.org/10.1136/bmj-2024-081123"
    why_included: "Reporting-navigation support for randomized trials, including trial registration, protocol/SAP access, participant flow, interventions, analysis populations, missing data and outcome reporting."
    limitation: "CONSORT is reporting guidance. Checklist completeness must never be converted into low risk of bias, high certainty or a numerical validity score."

  - source_id: "F0-S07"
    priority: "SUPPORT"
    citation: "Risk of Bias Tools. RoB 2 current version resources."
    url_or_doi: "https://www.riskofbias.info/welcome/rob-2-0-tool/current-version-of-rob-2"
    why_included: "Operational anchor for result-specific/domain-based risk-of-bias reasoning in individually randomized parallel-group trials."
    limitation: "The package uses conceptual domain reasoning only. It does not republish licensed tool documents, and domain judgments are not converted into a total quality score."

  - source_id: "F0-S29"
    priority: "SUPPORT"
    citation: "Heinsberg LW, Weeks DE. Post hoc Power is Not Informative. Genetic Epidemiology. 2022;46(7):390-394. doi:10.1002/gepi.22464."
    url_or_doi: "https://pmc.ncbi.nlm.nih.gov/articles/PMC9452450/"
    why_included: "Focused methodological safeguard against using observed/post-hoc power as interpretation of a completed study."
    limitation: "Focused commentary/simulation rather than a complete sample-size text. It does not imply that every post-study design-sensitivity calculation is mathematically identical; the F0.9 rule is that such calculations cannot substitute for the observed estimate, CI, design and bias analysis."

  - source_id: "F0-S18"
    priority: "CONTRAST"
    citation: "Neumann I, Brennan S, Meerpohl J, et al. Overview of the GRADE approach. In: The GRADE Book. GRADE Working Group. Last modified 12 May 2026."
    url_or_doi: "https://book.gradepro.org/guideline/overview-of-the-grade-approach"
    why_included: "Explicit contrast source for the boundary between one-paper critical appraisal and certainty of an evidence body/recommendation process."
    limitation: "GRADE is not a single-paper quality score. The source is included to prevent overreach, not to require a full GRADE rating during F0.9."

claims_to_master:
  - "A paper's title, abstract and discussion are claims to audit, not substitutes for Methods and Results."
  - "A complete-paper appraisal begins by reconstructing question, target population, contrast, outcome, time and estimand."
  - "The reader should extract PICO/estimand and material results before accepting the authors' narrative."
  - "Article, supplement, registry, protocol, SAP and data/code repository are distinct provenance objects; timestamps determine what they can establish about prespecification."
  - "The existence of a registry/protocol/SAP does not prove that it existed prospectively before relevant results could influence choices."
  - "Design labels constrain possible inference but do not by themselves determine validity."
  - "Intervention and comparator must be operationally reconstructed; if arms differ in more than one component, the causal contrast differs in more than one component."
  - "Outcome measurement must match the construct claimed; precision/repeatability does not guarantee construct validity."
  - "Risk of bias is result-specific and mechanism-based, not a paper-wide quality score."
  - "Missingness must be evaluated through reasons, differential patterns and relation to the outcome, not only percentage missing."
  - "Prospective sample-size/power planning, observed precision and post-hoc/observed power are different objects."
  - "Completed-study interpretation is based on effect estimate, uncertainty, practical threshold/context, design and bias—not observed power."
  - "Within-group improvement does not establish a between-group treatment effect."
  - "p>0.05 does not establish no effect or equivalence."
  - "Equivalence/non-inferiority requires a defensible margin and design/analysis appropriate to that claim."
  - "Multiplicity concerns the family of available claims/analyses, including outcomes, timepoints, contrasts, subgroups and models."
  - "Registration and prespecification improve auditability; they do not make an analysis scientifically correct by definition."
  - "Robustness analysis asks whether the conclusion survives defensible assumptions; outcome-driven model searching is not confirmation."
  - "Open data/code can increase auditability and reproducibility but do not retroactively repair design, measurement, missingness or prespecification."
  - "Reporting completeness and methodological validity are separate objects."
  - "Applicability is a structured evidence-versus-target comparison and is independent of internal validity."
  - "A single paper can be appraised for result-specific bias and applicability but cannot by itself be assigned the certainty of an entire evidence body."
  - "The strongest defensible inference may be narrower than the paper's title or conclusion."
  - "Every appraisal must state what the paper does not establish rather than ending with a generic call for more research."

critical_repairs:
  - "abstract-only appraisal → inspect Methods, Results and available external materials"
  - "RCT = trustworthy → design architecture first, then result-specific execution/bias"
  - "CONSORT-complete = low bias → reporting visibility is not validity"
  - "p<0.05 = true/important → estimate, CI, magnitude and context remain required"
  - "p>0.05 = no effect/equivalence → inspect compatible effect range and appropriate equivalence margin/design"
  - "within-group significant change = treatment effect → require direct between-group contrast/interaction"
  - "low observed power explains the result → use observed estimate/CI plus design/bias; post-hoc power adds no posterior evidence"
  - "registry exists = prespecified → reconstruct timestamp/version history"
  - "many outcomes but one highlighted p-value = no multiplicity issue → reconstruct claim family"
  - "global quality score = RoB → explain result-specific mechanism/domain/rationale"
  - "sensitivity analysis that gives desired p-value = robustness → distinguish planned/defensible checks from result-shopping"
  - "open data = valid study → auditability does not repair causal/statistical flaws"
  - "one paper = high/low GRADE certainty → certainty is a body/outcome/question object"
  - "authors said it, so paper proved it → independently reconstruct estimand/results and compare conclusion scope"

notebooklm_tasks:
  - "Act as a Socratic examiner. Do not reveal a completed appraisal of F0-S30. Require the learner to cite where in the approved sources each extracted fact came from."
  - "Before discussing the conclusion of F0-S30, require a provenance note, PICO/estimand table and material-result table."
  - "Ask the learner to reconstruct the paper-versus-registry timeline from F0-S30 and F0-S31 without supplying the conclusion in advance."
  - "Generate generic trial snippets and ask which source layer—main text, supplement, registry, protocol, SAP or data repository—should be checked next."
  - "Generate intervention/comparator descriptions where more than one component differs and require the exact causal contrast to be stated."
  - "Generate within-group and between-group outputs and require the learner to identify which one estimates the intervention contrast."
  - "Generate nonsignificant contrasts with wide and narrow CIs and require the learner to distinguish uncertainty from evidence compatible with trivial effects."
  - "Generate equivalence claims and require a prespecified practical/equivalence margin before accepting them."
  - "Generate sample-size, precision and observed-power statements and require classification of each object."
  - "Generate multiple-outcome/timepoint/model scenarios and require a claim-family/multiplicity map."
  - "Generate result-specific RoB scenarios and prohibit numerical quality scoring."
  - "Generate robustness checks and result-shopping variants and require the learner to separate them."
  - "Generate a well-reported but biased trial and a poorly reported but potentially valid trial to preserve reporting-versus-validity reasoning."
  - "Ask for an applicability audit using population, intervention/exposure, comparator, outcome, time, setting and decision context."
  - "Ask why GRADE certainty cannot be assigned from F0-S30 alone without reconstructing the relevant evidence body."
  - "Require a one-paragraph strongest-defensible-inference statement that is narrower than any unsupported claim."
  - "Require at least three explicit 'does not establish' boundaries for the real paper, but do not suggest which ones before the learner inspects the sources."
  - "At the end, require the full twelve-step F0.9 sequence from memory and a source-cited audit of F0-S30/F0-S31."

initial_corpus_exclusions:
  - "foundations/F0-scientific-literacy/F0.9-critical-reading-complete-paper/EXERCISES.md"
  - "foundations/F0-scientific-literacy/F0.9-critical-reading-complete-paper/ANSWER_KEY.md"
  - "foundations/F0-scientific-literacy/F0.9-critical-reading-complete-paper/QA_REPORT.md"
  - "foundations/F0-scientific-literacy/SOURCE_INDEX.md"
  - "foundations/F0-scientific-literacy/F0.4-descriptive-statistics/ENTRY_DIAGNOSTIC.md"

mastery_state_policy:
  - "Package production changes no learner state."
  - "F0.1–F0.9 remain pending/unvalidated until observed learning/performance."
  - "F0.4 quantitative diagnostic remains UNOBSERVED."
  - "NotebookLM practice is study support and does not itself authorize MASTERED."
```

---

## External source/link verification — 2026-09-10

All external sources included in manifest v1 were rechecked before package creation.

### F0-S30 — full paper

- PMC full-text record remains accessible.
- Citation remains *JISSN* 2025;22(1):2519511, DOI `10.1080/15502783.2025.2519511`.
- PMC states Open Access under **CC BY 4.0**.
- The paper remains appropriate as the full-paper training object.

### F0-S31 — ClinicalTrials.gov

- `https://clinicaltrials.gov/study/NCT05922475` resolves to the public registry resource.
- The learner must inspect study/record dates and version history directly; the manifest does not supply the completed prespecification judgment.

### F0-S01 — CONSORT 2025

- CONSORT 2025 remains the current general reporting statement for randomized trials.
- The statement contains a 30-item checklist and explicitly surfaces registration, protocol/SAP access, open-science materials, analysis populations, missing data and changes to outcomes/analyses.
- It remains a reporting guideline, not a risk-of-bias score.

### F0-S07 — RoB 2

- Official `riskofbias.info` current-version page still lists **22 August 2019** for individually randomized parallel-group trials.
- RoB 2/related tool documents are licensed **CC BY-NC-ND 4.0**; no tool PDF/template is copied into this repository.

### F0-S29 — Heinsberg & Weeks 2022

- PMC record remains accessible for *Post hoc Power is Not Informative*.
- The source continues to support the specific safeguard that observed-effect post-hoc power should not be used to interpret a completed study.

### F0-S18 — GRADE Book overview

- Living GRADE Book overview remains last modified **12 May 2026**.
- It continues to frame certainty as a property of evidence supporting a question/outcome and separates certainty from recommendation processes.
- F0.9 uses it only to block a single-paper certainty shortcut.

No external-source change required revision of the approved F0.9 lesson before building this package.

---

## Copyright/public-repository controls

- No third-party PDF, figure, table, RoB template or full-text article is committed by this package.
- `F0-S30` may be added to NotebookLM through its legal PMC source; the GitHub package stores only citation/link/instructions.
- `F0-S31` is referenced by its public registry URL.
- Licensed methodological sources are linked rather than republished.
- All NotebookLM prompts and study instructions are original project material.

---

## First-pass completion gate

The first-pass F0.9 notebook is complete only when the learner can, **without the answer key**:

1. reproduce the twelve-step appraisal sequence;
2. navigate paper/registry/support sources with correct provenance;
3. produce PICO/estimand and result tables;
4. separate within-group and between-group inference;
5. interpret estimate/CI without binary p-value shortcuts;
6. classify prospective versus retrospective evidence using timestamps;
7. map multiplicity and result-specific bias mechanisms;
8. distinguish robustness from result-shopping;
9. audit applicability;
10. distinguish single-paper appraisal from body-level certainty;
11. audit the authors' conclusion independently;
12. state the strongest defensible inference and explicit non-established claims.

This is readiness for independent assessment, not evidence that mastery has already occurred.
