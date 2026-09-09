# F0.3 — NotebookLM Manifest

**Package state:** `READY_FOR_STUDY`
**Manifest version:** `1`
**Built/verified:** `2026-09-09`
**Learner state affected:** none

This manifest defines the approved, deliberately small NotebookLM corpus for `F0.3 — Bias, confounding, causal reasoning and validity`. GitHub remains canonical; NotebookLM is a source-controlled study layer.

The first-pass corpus is intentionally limited to six sources. The purpose is not to teach every formal risk-of-bias framework. It is to make the learner repeatedly execute the causal-validity reasoning sequence:

`target causal question/estimand → temporal/causal structure → bias mechanism → valid versus invalid adjustment/conditioning → repairability/data limitation → calibrated conclusion`

Formal RoB 2/ROBINS-I judgments, domain algorithms and GRADE certainty assessment remain reserved for F0.8.

```yaml
module_id: "F0.3"
module_title: "Bias, confounding, causal reasoning and validity"
version: 1
learning_objectives:
  - "Distinguish random error from systematic error/bias and explain why increasing sample size does not automatically repair systematic error."
  - "Translate an observed association into an explicit target causal question and identify the estimand/contrast whose validity is being judged."
  - "Use counterfactual and exchangeability intuition to explain why observed groups need causal comparability for an association to represent an effect."
  - "Identify confounding and residual confounding as causal-structure problems rather than merely statistical association between covariates and exposure/outcome."
  - "Construct and critique simple causal DAGs while treating arrows as explicit assumptions rather than empirical proof."
  - "Distinguish confounder, mediator and collider roles relative to a specified causal question/estimand."
  - "Explain why indiscriminate covariate adjustment can change the estimand or introduce bias, including mediator adjustment and collider conditioning."
  - "Identify selection mechanisms affecting study entry, retention, complete-case status or analytical inclusion and explain how conditioning on selection can distort an estimate."
  - "Identify measurement/information bias, exposure/outcome/confounder misclassification and the limits of simplistic rules such as 'non-differential misclassification always biases toward the null'."
  - "Treat attrition and missingness as causal processes and explain why missing-data percentage alone does not determine bias."
  - "Recognize reverse causation and connect it to temporal ordering from F0.2."
  - "Explain what randomization reduces at baseline and what post-randomization bias pathways can still remain."
  - "Use target-trial thinking as a causal-design benchmark without treating observational emulation as retroactive randomization."
  - "Separate internal validity from external validity/generalizability/transportability/applicability."
  - "For an applied scenario, distinguish what can be prevented or mitigated by design/measurement/analysis from information that cannot be recovered reliably when it was never measured or structurally unavailable."
  - "State conclusions whose causal certainty is proportional to the assumptions and data actually available."

sources:
  - source_id: "F0-R03"
    priority: "CORE"
    citation: "Sports Nutrition Mastery. F0.3 — Viés, confounding, raciocínio causal e validade. Canonical project lesson, version current at manifest v1."
    url_or_doi: "https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.3-bias-confounding-causal-validity/LESSON.md"
    why_included: "Primary instructional spine. It integrates the exact F0.3 vocabulary and forces the project reasoning sequence from causal question and structure through distortion mechanism, repairability and calibrated conclusion. It also enforces the curricular boundary that formal RoB/GRADE scoring belongs later."

  - source_id: "F0-S16"
    priority: "CORE"
    citation: "Hernán MA, Robins JM. Causal Inference: What If. Boca Raton: Chapman & Hall/CRC; 2020. Free online edition maintained and revised by the authors."
    url_or_doi: "https://miguelhernan.org/whatifbook"
    why_included: "Foundational causal-inference reference for counterfactuals, exchangeability, confounding, randomized versus observational contrasts, selection and causal identification. For F0.3 use only the introductory conceptual material assigned by the study guide; do not attempt to master the full advanced book in this unit. The authors' page should be used to obtain the latest edition rather than a stale mirrored copy."

  - source_id: "F0-S26"
    priority: "CORE"
    citation: "Feeney T, Hartwig FP, Davies NM. How to use directed acyclic graphs: guide for clinical researchers. BMJ. 2025;388:e078226. doi:10.1136/bmj-2023-078226."
    url_or_doi: "https://www.bmj.com/content/388/bmj-2023-078226"
    why_included: "Practical DAG anchor. It links the target question and assumed causal structure to confounders, mediators, colliders, selection processes and covariate selection, and explicitly treats DAGs as assumption/communication tools rather than proof generators."

  - source_id: "F0-S11"
    priority: "SUPPORT"
    citation: "Catalogue of Bias Collaboration / Centre for Evidence-Based Medicine, University of Oxford. Catalogue of Bias."
    url_or_doi: "https://catalogofbias.org/biases/"
    why_included: "Concrete examples and plain-language definitions for confounding, collider bias, selection, attrition, information/measurement and related biases. It is included to connect named biases to mechanisms, not to encourage taxonomy memorization."

  - source_id: "F0-S07"
    priority: "SUPPORT"
    citation: "Risk of Bias Tools. ROBINS-I V2 tool page and current project hub. Revised ROBINS-I V2 draft posted 20 November 2025; still explicitly draft as verified 9 September 2026."
    url_or_doi: "https://www.riskofbias.info/welcome/robins-i-v2"
    why_included: "Boundary/support source showing that modern operational risk-of-bias work separates confounding, intervention classification, selection, missing data, outcome measurement and selective reporting rather than collapsing validity into one quality number. Use only to recognize domain separation and current version status. Do not apply the ROBINS-I V2 algorithms or produce formal risk-of-bias judgments in F0.3."

  - source_id: "F0-S17"
    priority: "CONTRAST"
    citation: "Hernán MA, Dahabreh IJ, Dickerman BA, Swanson SA. The Target Trial Framework for Causal Inference From Observational Data: Why and When Is It Helpful? Ann Intern Med. 2025;178(3):402-407. doi:10.7326/ANNALS-24-01871."
    url_or_doi: "https://pmc.ncbi.nlm.nih.gov/articles/PMC11936718/"
    why_included: "Contrast source for design versus data limitations. It shows how explicit target-trial specification can prevent design-induced biases while leaving unmeasured confounding and other data limitations unresolved. It reinforces that observational emulation does not create randomized assignment."

claims_to_master:
  - "A causal-validity judgment begins with the target causal question and estimand; there is no universally correct adjustment set independent of the question."
  - "Random error and systematic error are different problems. Larger sample size can reduce sampling variation while leaving systematic bias intact."
  - "Counterfactual reasoning asks what outcomes would occur under alternative strategies; because both potential outcomes are not observed for the same person at the same time, causal inference requires design and assumptions that make comparisons valid."
  - "Exchangeability is a comparability condition for causal contrasts, not a verbal certificate that observational groups are equivalent."
  - "Confounding is a causal/common-cause or open non-causal path problem; a variable is not a confounder merely because it predicts both exposure and outcome in the observed dataset."
  - "Residual confounding can remain after adjustment because a confounder is unmeasured, poorly measured, coarsened, represented by an inadequate proxy or modeled/structured incorrectly."
  - "A mediator lies on a causal pathway from exposure/intervention to outcome for the specified estimand. Conditioning on it can remove part of a total effect and therefore change the question being estimated."
  - "A collider is a common effect of two causes. Conditioning on a collider or on selection driven by a collider can open a non-causal path and create/distort association."
  - "DAGs encode assumptions about causal structure and temporal ordering. They can reveal adjustment implications but cannot establish that their arrows are true."
  - "Selection bias can arise through who enters the study, remains under follow-up, has complete data or is included in the analytical sample. Representativeness and selection bias are related but not identical questions."
  - "Measurement/information bias can affect exposure, outcome or confounders; misclassification behavior depends on structure, measure and direction, so simple universal rules are unsafe."
  - "Missingness/attrition is a process. Equal missing percentages between groups do not guarantee unbiased comparison, and unequal percentages do not by themselves determine the direction or magnitude of bias."
  - "Complete-case analysis is not automatically neutral; its validity depends on the process that created complete versus incomplete observations."
  - "Reverse causation is plausible when the outcome or preclinical state can influence the measured exposure, especially when temporal ordering is weak."
  - "Randomization reduces baseline confounding/selection in treatment assignment in expectation, but it does not prevent post-randomization missingness, differential measurement, adherence problems, protocol deviations or biased analysis/reporting."
  - "Target-trial emulation can prevent some design-induced biases by aligning eligibility, strategy assignment, time zero, follow-up and causal contrast, but it cannot create data that were never collected or eliminate unmeasured confounding by declaration."
  - "Internal validity asks whether the target effect is credibly estimated in the study context; external validity/applicability asks whether that estimate can be transported to another target population/context. These are separate judgments."
  - "A defensible causal conclusion states both what the observed design/data support and which assumptions or missing information limit certainty."

controversies_or_limits:
  - "The causal role of a variable is question/estimand-specific. The same variable can be a confounder for one question, mediator for another or irrelevant to a different target effect."
  - "DAGs can improve transparency and covariate reasoning but depend on substantive causal assumptions. A well-drawn DAG does not prove the data-generating mechanism."
  - "The Catalogue of Bias is useful for examples and terminology but can encourage label collection. The learner must always explain the mechanism by which the estimate is distorted."
  - "The official ROBINS-I V2 page currently labels the November 2025 revision as a draft and subject to change. F0.3 therefore uses it only as support for bias-domain separation and version literacy; formal use is deferred to F0.8."
  - "Risk-of-bias tools are result/domain-specific frameworks, not numerical quality scores. F0.3 does not teach formal tool algorithms, signaling questions or overall judgments."
  - "Causal Inference: What If is substantially deeper than the F0.3 target. The study guide restricts use to selected foundational concepts; advanced longitudinal causal methods remain outside scope."
  - "Target-trial framing is most natural for causal questions about sufficiently well-defined intervention strategies that can be mapped to available data. It is not a universal replacement for every descriptive, diagnostic or prognostic design."
  - "F0.3 intentionally defers standard errors, confidence intervals, p-values, power and multiplicity to F0.4-F0.6. A causal structure can be valid while an estimate is imprecise, and a precise estimate can be causally biased."
  - "F0.3 intentionally defers formal certainty-of-evidence assessment and GRADE to F0.8-F0.10. Verbal calibration here is conceptual, not a GRADE rating."

active_recall:
  basic:
    - "Define bias/systematic error and distinguish it from random error without mentioning p-values."
    - "What is the causal question/estimand and why must it be specified before choosing covariates?"
    - "Explain counterfactual intuition using strategy A versus strategy B."
    - "Define confounder, mediator and collider relative to a target causal question."
    - "What is residual confounding? Give four mechanisms that can produce it."
    - "What is reverse causation?"
    - "Distinguish internal validity from applicability/external validity."
  mechanism:
    - "Explain step by step how a common cause C can create an association between A and Y even when part of that association is non-causal."
    - "Explain how conditioning on a mediator can change a total-effect estimand."
    - "Explain how conditioning on a collider can open a path that was previously closed."
    - "Explain how loss to follow-up can become selection bias when retention depends on causes related to treatment/exposure and outcome."
    - "Explain why equal attrition percentages do not guarantee equal bias."
    - "Explain why increasing N cannot reconstruct an unmeasured confounder or repair systematic outcome mismeasurement."
    - "Explain why randomization protects the treatment-assignment stage but does not immunize all later study stages."
  evidence_critique:
    - "Using the BMJ DAG guide, construct a simple DAG for exposure A, outcome Y and a common cause C; identify the path that should be blocked and explain the assumption behind each arrow."
    - "Using the BMJ DAG guide, create one mediator and one collider example and state why adjustment decisions differ."
    - "Using the Catalogue of Bias, choose three named biases and translate each label into: who/what is selected or measured → why it differs → how the estimate can be distorted."
    - "Using the ROBINS-I V2 page only at a boundary level, list the current major domains shown for non-randomized intervention results and explain why F0.3 is not yet performing a formal ROBINS-I assessment."
    - "Using the target-trial paper, distinguish design-induced bias that better protocol alignment can prevent from data limitations such as unmeasured confounding that remain after emulation."
    - "Using What If and the canonical lesson, compare causal identification in a randomized assignment with observational exchangeability assumptions without claiming that statistical adjustment automatically makes them equivalent."
  integration:
    - "For an unfamiliar causal scenario, output exactly: Target causal question/estimand → causal structure → distortion mechanism → valid/invalid adjustment → repairability/data limitation → calibrated conclusion."
    - "Construct two DAGs for the same exposure/outcome pair under different plausible causal assumptions and show how the valid adjustment set can change."
    - "Give one randomized-trial bias pathway and one observational-study bias pathway that produce similar observed distortion through different stages of the study."
    - "Take a complete-case analysis scenario and describe at least two missingness mechanisms under which the same 20% missing-data rate would have different validity implications."
    - "Create a scenario where measuring more covariates makes the causal estimate worse because one added variable is a mediator or collider."
    - "Convert an observational causal question into a target trial, then explicitly separate: preventable design bias → measurable/adjustable limitation → unrecoverable absent data → remaining assumption."
    - "For a result with strong internal validity but narrow eligibility, write one internally valid conclusion and a separate cautious applicability statement."

notebooklm_tasks:
  - "Act as a Socratic examiner. Present one causal-validity scenario at a time and wait for the learner's full causal structure before grading."
  - "For every applied scenario, require the final six fields exactly: 'Target causal question/estimand:', 'Causal structure:', 'Distortion mechanism:', 'Adjustment/conditioning:', 'Repairability/data limitation:', 'Calibrated conclusion:'."
  - "Generate paired scenarios with the same variables but different arrow directions so the learner cannot classify confounder/mediator/collider roles from variable names alone."
  - "Require the learner to draw or describe a DAG before choosing an adjustment set; then challenge one assumed arrow and ask how the adjustment decision changes."
  - "Generate collider traps where a seemingly predictive covariate should not be adjusted for the total-effect question."
  - "Generate mediator traps where adjustment answers a different estimand than the requested total effect."
  - "Generate selection/attrition scenarios with identical missing percentages but different causal mechanisms and require different conclusions."
  - "Generate exposure/outcome measurement scenarios and ask whether the problem is random noise, systematic measurement bias, differential measurement or unresolved from the information given."
  - "Contrast one well-randomized trial with one observational study and ask which bias mechanisms are reduced at allocation and which can arise later in both."
  - "Use the target-trial source to require eligibility, strategies, assignment, time zero, outcome, follow-up and causal contrast, then ask separately which design bias was prevented and which data limitation remains."
  - "When using the ROBINS-I V2 webpage, never run or simulate formal signaling-question algorithms and never output an overall ROBINS-I risk-of-bias judgment; that is reserved for F0.8."
  - "For every explanation, cite only the approved corpus and state explicitly when the corpus cannot determine an arrow, missingness mechanism or unmeasured variable."
  - "Never treat a NotebookLM-generated claim lacking support in the approved corpus as canonical project knowledge."
```

## Evidence-critique task

Use the canonical F0.3 lesson, `F0-S26` (BMJ DAG guide) and `F0-S17` (target-trial framework) to appraise this hypothetical observational causal question:

> Among resistance-trained adults beginning a 12-week training block, does starting nutrition strategy A rather than strategy B improve a prespecified performance outcome at week 12?

Assume the observational dataset contains baseline age, sex, baseline performance, training volume, prior supplement use, self-selected strategy A/B, week-12 performance and follow-up status, but does **not** contain sleep duration or coaching quality.

Your appraisal must:

1. define the target causal contrast/estimand in plain language;
2. specify the hypothetical target trial: eligibility, strategies, assignment, time zero, follow-up, outcome and causal contrast;
3. draw or text-describe a plausible DAG containing strategy, week-12 outcome, training volume, baseline performance, sleep and coaching quality;
4. identify which variables are plausible baseline confounders under your DAG and why;
5. identify at least one plausible variable that would become a mediator if it were measured after strategy initiation;
6. create one plausible collider/selection mechanism involving follow-up or analytical inclusion;
7. explain what observed variables could be adjusted/stratified by design or analysis and what causal assumptions this requires;
8. explain why unmeasured sleep/coaching cannot be guaranteed repaired merely by large N or by adjusting every measured covariate;
9. describe how attrition could distort the result and why its percentage alone is insufficient;
10. distinguish what target-trial specification prevents from what it cannot repair in these data;
11. state one internally calibrated causal conclusion that does not overclaim observational identification;
12. state a separate applicability limitation if the sample is restricted to young trained men.

**Scoring principle:** causal structure, mechanism and inferential restraint matter more than naming the largest number of biases.

## Corpus exclusions

Do **not** add these to the initial NotebookLM corpus:

- `foundations/F0-scientific-literacy/F0.3-bias-confounding-causal-validity/ANSWER_KEY.md` — exclusion prevents answer leakage;
- `foundations/F0-scientific-literacy/F0.3-bias-confounding-causal-validity/EXERCISES.md` — keep the independent assessment outside the study corpus;
- `foundations/F0-scientific-literacy/F0.3-bias-confounding-causal-validity/QA_REPORT.md` — production metadata, not instructional evidence;
- the full `SOURCE_INDEX.md` — registry metadata would add noise;
- RoB 2 full tool documents or ROBINS-I V2 full/template documents — formal domain algorithms belong to F0.8 and current ROBINS-I V2 is still draft;
- GRADE Book certainty chapters — certainty-of-evidence framework belongs to F0.8-F0.10;
- F0.4-F0.6 statistical references — sampling variation, confidence intervals, p-values, effect sizes, power and multiplicity are intentionally deferred;
- additional DAG tutorials on the first pass — the canonical lesson plus BMJ 2025 guide are sufficient for introductory DAG reasoning;
- broad collections of individual bias pages — use the Catalogue index selectively so the notebook does not become a taxonomy dump.

`EXERCISES.md` must be completed independently after the NotebookLM study sequence, before consulting `ANSWER_KEY.md`.

## Version integrity

The corpus was verified on 2026-09-09 against current accessible sources:

- the canonical F0.3 lesson exists on `main` and remains `APPROVED`;
- the official `Causal Inference: What If` page remains available and explicitly directs readers to the latest revision; the current linked PDF observed during verification is dated `19aug26`, so the package points to the authors' landing page rather than freezing a stale mirror;
- the BMJ DAG guide remains available as BMJ 2025;388:e078226, DOI `10.1136/bmj-2023-078226`, published 21 March 2025;
- the Catalogue of Bias remains live under the Centre for Evidence-Based Medicine and continues to expose confounding, collider, selection and attrition entries among its current catalogue;
- `riskofbias.info` remains the official hub for RoB 2, ROBINS-I, ROBINS-E and ROB ME; its ROBINS-I V2 page states that the revised V2 was posted `20 November 2025`, remains a **draft version** and is subject to change;
- the target-trial framework remains available in free full text via PMC as Ann Intern Med. 2025;178(3):402-407, DOI `10.7326/ANNALS-24-01871`.

If any living source changes materially, recheck the manifest before using the affected source for a new formal assessment.
