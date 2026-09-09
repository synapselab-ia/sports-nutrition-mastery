# F0.8 — NotebookLM Manifest

**Package state:** `READY_FOR_STUDY`
**Manifest version:** `1`
**Built/verified:** `2026-09-09`
**Learner state affected:** none
**F0.4 quantitative diagnostic affected:** none; remains `UNOBSERVED`

This manifest defines the approved first-pass NotebookLM corpus for `F0.8 — Risk of bias, certainty of evidence and applicability`. GitHub remains canonical; NotebookLM is a controlled study layer.

The corpus is intentionally limited to **six sources**. The required F0.8 audit sequence is:

`Target question/outcome → Reporting visibility → Design/effect of interest → Result-level RoB mechanisms → RoB judgment/rationale → Body estimate + threshold → Inconsistency → Indirectness → Imprecision → Missing/dissemination evidence → Overall certainty → Applicability to target → Recommendation-strength boundary`

The package must preserve prior modules rather than replacing them:

- F0.2 supplies design/inference boundaries;
- F0.3 supplies causal bias mechanisms and internal/external-validity reasoning;
- F0.5 supplies estimate + CI + magnitude + decision-threshold reasoning;
- F0.7 supplies heterogeneity and missing-evidence reasoning.

F0.8 adds structured result-level risk-of-bias appraisal, body/outcome certainty and target-context applicability. Full-paper integration remains F0.9.

```yaml
module_id: "F0.8"
module_title: "Risk of bias, certainty of evidence and applicability"
version: 1
learning_objectives:
  - "Keep reporting completeness, broad critical appraisal, result-level risk of bias, body/outcome certainty, applicability/transportability and recommendation strength as distinct objects."
  - "Explain why CONSORT/STROBE/PRISMA visibility does not certify low risk of bias or high certainty."
  - "Distinguish missing reporting from demonstrated methodological failure; do not invent a low- or high-risk judgment when information is insufficient."
  - "Treat risk of bias as result-specific and domain-based rather than assigning one global study-quality score."
  - "Distinguish systematic bias from imprecision/random error and explain why a very precise result can still be biased."
  - "Apply RoB 2 conceptually to an individually randomized parallel-group trial using the five current domains."
  - "Preserve the current RoB 2 version for individually randomized parallel-group trials: 22 August 2019."
  - "Reject randomized = automatically low risk of bias."
  - "Use ROBINS-I target-trial logic conceptually for non-randomized intervention-effect studies."
  - "Preserve the current ROBINS-I V2 status as a revised draft posted 20 November 2025 and subject to change."
  - "Reject observational/non-randomized = automatically unusable while still requiring explicit confounding and selection reasoning."
  - "Define GRADE certainty as confidence in an effect range/side of a decision threshold for a body of evidence and outcome/question, not as a prestige label for a paper."
  - "Recall the four GRADE certainty categories: High, Moderate, Low and Very low."
  - "Use the five core downgrading domains taught in F0.8: risk of bias, inconsistency, indirectness, imprecision and dissemination/publication/non-reporting bias."
  - "Explain basic versus structured-ROBINS-I starting approaches for randomized and non-randomized intervention evidence without turning starting level into a final verdict."
  - "Use F0.5 magnitude + CI + practical/decision thresholds to judge imprecision."
  - "Use F0.7 clinical/methodological/statistical heterogeneity reasoning to judge inconsistency rather than using I2 mechanically."
  - "Use F0.7 small-study/missing-evidence safeguards when considering dissemination/non-reporting bias."
  - "Assess indirectness/applicability by comparing evidence with the target population, intervention/exposure, comparator, outcome, time horizon, setting and decision context."
  - "Explain why every PICO difference does not automatically require a downgrade; the difference must plausibly matter for the effect or absolute impact."
  - "Distinguish internal validity from applicability: direct evidence can be biased, and low-bias evidence can be narrow for the target."
  - "Reject low certainty = no effect, high certainty = large/important effect and statistical significance = high certainty."
  - "Keep certainty of one outcome distinct from recommendation strength, which integrates the net effect and additional decision criteria."
  - "Compare two bodies with similar point estimates but different bias, precision, consistency, directness and target applicability."
  - "Audit an unfamiliar evidence body using all thirteen F0.8 fields in order."
  - "Defer full-paper F0.1-F0.8 integration to F0.9."

sources:
  - source_id: "F0-R08"
    priority: "CORE"
    citation: "Sports Nutrition Mastery. F0.8 — Risk of bias, certeza da evidência e aplicabilidade. Canonical project lesson, version current at manifest v1."
    url_or_doi: "https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.8-risk-of-bias-certainty-applicability/LESSON.md"
    why_included: "Primary instructional spine defining the exact project vocabulary, result-specific RoB reasoning, GRADE integration, applicability frame, critical fails, integrated two-body scenario and thirteen-field audit."
    limitation: "Project-authored teaching material, not an independent methodological authority. Material claims remain traceable to the external sources below."

  - source_id: "F0-S07"
    priority: "CORE"
    citation: "Risk of Bias Tools. RoB 2 and ROBINS-I official project website. Current tool pages."
    url_or_doi: "https://www.riskofbias.info/"
    why_included: "Primary operational anchor for result-specific/domain-based risk-of-bias reasoning, the current RoB 2 tool/version for randomized trials and the current ROBINS-I V2 draft/status for non-randomized intervention studies."
    limitation: "Tool use requires training and study-specific judgment. RoB 2/ROBINS-I are not total quality scores. ROBINS-I V2 is currently a draft and must not be presented as finalized. Tool documents are not republished in this public repository."

  - source_id: "F0-S18"
    priority: "CORE"
    citation: "Neumann I, Brennan S, Meerpohl J, et al. Overview of the GRADE approach. In: The GRADE Book. GRADE Working Group. Last modified 12 May 2026."
    url_or_doi: "https://book.gradepro.org/guideline/overview-of-the-grade-approach"
    why_included: "Primary external anchor for GRADE purpose, four certainty categories, five principal downgrading domains, outcome/body-level certainty and explicit separation between certainty of evidence and strength of recommendations."
    limitation: "GRADE is a structured framework requiring judgments; it is not a mechanical score. The overview does not replace domain-specific guidance or direct appraisal of the studies."

  - source_id: "F0-S19"
    priority: "SUPPORT"
    citation: "Goldkuhle M, Kreuzberger N, Neumann I, et al. Principles for assessing the certainty of interventions. In: The GRADE Book. GRADE Working Group. Last modified 21 August 2025."
    url_or_doi: "https://book.gradepro.org/guideline/principles-for-assessing-the-certainty-of-interventions"
    why_included: "Focused support for threshold/range-aware certainty, outcome/body-level assessment, absolute-effect reasoning and the basic versus structured-ROBINS-I starting approaches for non-randomized intervention evidence."
    limitation: "Advanced GRADE implementation is broader than F0.8. The package uses the conceptual decision logic and explicitly avoids teaching rating as a rote downgrade checklist."

  - source_id: "F0-S20"
    priority: "SUPPORT"
    citation: "Schünemann HJ, Neumann I, Brennan S, et al. Indirectness. In: The GRADE Book. GRADE Working Group. Last modified 12 May 2026."
    url_or_doi: "https://book.gradepro.org/guideline/indirectness"
    why_included: "Focused support for evidence-versus-target PICO comparison, applicability/generalizability/transferability reasoning, baseline-risk implications and the rule that not every difference warrants rating down."
    limitation: "Formal indirectness ratings still require domain knowledge and a defined decision target. F0.8 adds time horizon, setting and decision context as explicit operational prompts without pretending they are independent universal checklist domains."

  - source_id: "F0-S02"
    priority: "CONTRAST"
    citation: "von Elm E, Altman DG, Egger M, et al.; STROBE Initiative. STROBE statement: guidelines for reporting observational studies. J Clin Epidemiol. 2008;61(4):344-349. doi:10.1016/j.jclinepi.2007.11.008."
    url_or_doi: "https://www.strobe-statement.org/"
    why_included: "Deliberate contrast source showing the difference between reporting guidance and validity appraisal. STROBE explicitly states that its checklist is for reporting and is not an instrument to evaluate study quality."
    limitation: "Reporting guideline for cohort, case-control and cross-sectional studies; it does not perform causal identification, ROBINS-I appraisal, GRADE certainty assessment or target-context applicability judgment. Its role here is contrast, not authority for risk-of-bias categories."

claims_to_master:
  - "Reporting completeness answers whether methods/results are visible enough to audit; it does not answer whether the result is unbiased."
  - "Critical appraisal is broader than one checklist or tool and asks whether design, conduct, analysis, interpretation and applicability fit the question."
  - "Risk of bias is a judgment about systematic distortion of a specific result/effect estimate, not a global moral or prestige rating of a paper."
  - "Different outcomes or analyses from one study can have different risk-of-bias judgments."
  - "Bias and imprecision are different: greater sample size can narrow uncertainty while leaving systematic bias intact."
  - "RoB 2 for individually randomized parallel-group trials remains the 22 August 2019 version and evaluates five core domains."
  - "Randomization mainly protects the origin of the comparison against baseline confounding when correctly implemented; missing data, measurement, deviations and result selection can still bias a randomized result."
  - "ROBINS-I uses a target trial as a benchmark for appraising non-randomized intervention-effect studies; it does not retroactively randomize them."
  - "ROBINS-I V2 is currently a revised draft posted 20 November 2025 and subject to change."
  - "Non-randomized evidence is not automatically unusable; validity depends on the question, design, confounding/selection structure, measurement, data and assumptions."
  - "GRADE certainty is assessed for a body of evidence and outcome/question, not assigned as a single prestige label to a paper."
  - "The four certainty categories are High, Moderate, Low and Very low."
  - "High certainty can support confidence that an effect is trivial/near-null; high certainty does not mean a large effect."
  - "Low certainty means low confidence in where the true effect lies relative to the relevant range/threshold; it does not mean no effect."
  - "Statistical significance alone does not establish high certainty."
  - "GRADE risk-of-bias, inconsistency, indirectness, imprecision and dissemination-bias concerns matter only insofar as they create reasonable doubt about the target certainty range/threshold; domains are not automatic subtraction rules."
  - "Inconsistency is not equivalent to I2. Effect direction, magnitude, thresholds, clinical/methodological diversity and plausible explanations matter."
  - "Indirectness is a target-specific mismatch problem; compare evidence PICO with target PICO and ask whether differences plausibly alter relative or absolute effects."
  - "Imprecision must be judged against decision-relevant ranges/thresholds using estimates and confidence intervals, not p-values alone."
  - "Publication/non-reporting bias is not diagnosed by funnel asymmetry or symmetry; missing-evidence reasoning remains probabilistic and mechanism-based."
  - "Internal validity asks whether the estimate is credible in the studied conditions; applicability asks whether the inference transfers to the target."
  - "Direct evidence can still be biased; low-bias evidence can still be indirect for a target."
  - "Certainty of one outcome is not recommendation strength. Recommendations integrate multiple outcomes/net effects and can also consider values, resources, equity, acceptability and feasibility."
  - "Two evidence bodies can have nearly identical point estimates but very different certainty and applicability."

controversies_or_limits:
  - "Risk-of-bias tools structure judgment but do not eliminate judgment, uncertainty or the need to understand the target effect."
  - "A poorly reported method may yield insufficient information rather than proof that the method was poor; do not invent facts from silence."
  - "Overall RoB judgments should not be produced by adding arbitrary numeric domain scores."
  - "The appropriate RoB 2 variant depends on trial architecture; F0.8 focuses on individually randomized parallel-group trials and does not pretend cluster/crossover variants are identical."
  - "ROBINS-I V2 remains draft; domain structure/version language must be rechecked before later reuse."
  - "GRADE starting levels are starting conventions rather than final conclusions. The structured-ROBINS-I approach for NRSI is more advanced and does not imply observational evidence routinely stays high certainty."
  - "GRADE domains can overlap; double-counting the same underlying concern across domains should be avoided."
  - "Decision thresholds/ranges are contextual and must be justified; certainty cannot be interpreted independently of what effect distinctions matter to the decision."
  - "Indirectness is not a binary similarity checklist; some target differences are irrelevant while others materially alter effect transfer or baseline absolute impact."
  - "Applicability may depend on sport/training status, dose, comparator, outcome definition, duration, environment and implementation context; no single generic transport rule substitutes for domain knowledge."
  - "Recommendation strength involves a broader Evidence-to-Decision problem and remains only a boundary concept in F0.8; this unit does not train guideline-panel recommendation development."
  - "Synthetic athlete/intervention examples are methodological exercises, not evidence of intervention efficacy or nutrition recommendations."
  - "Full-paper integration across F0.1-F0.8 remains F0.9."

active_recall:
  basic:
    - "Define reporting completeness, critical appraisal, result-level risk of bias, certainty, applicability and recommendation strength as six separate objects."
    - "State the current individually randomized RoB 2 version and its five domains."
    - "State the current ROBINS-I V2 status and explain what a target trial contributes to appraisal."
    - "Name the four GRADE certainty categories."
    - "Name the five F0.8 downgrading domains."
    - "State why STROBE/CONSORT/PRISMA completeness is not a low-risk certificate."
  mechanism:
    - "Explain how a randomized result can still be biased after successful randomization."
    - "Explain why a precise estimate can be systematically wrong."
    - "Explain why result-level RoB can differ between two outcomes from the same study."
    - "Explain how confounding and selection enter target-trial/ROBINS-I reasoning."
    - "Explain how heterogeneity can create inconsistency concerns without reducing the problem to I2."
    - "Explain how evidence/target PICO mismatch can alter relative-effect transfer or baseline absolute impact."
    - "Explain why a CI crossing a decision threshold can create imprecision concerns even when p<0.05 or p>0.05."
  evidence_critique:
    - "Repair 'CONSORT/STROBE/PRISMA complete means low risk of bias'."
    - "Repair 'this study scored 8/10, so its result is trustworthy'."
    - "Repair 'randomized means low risk of bias'."
    - "Repair 'observational evidence is automatically unusable'."
    - "Repair 'low certainty means the intervention has no effect'."
    - "Repair 'high certainty means the effect is large and important'."
    - "Repair 'p<0.001 means high certainty'."
    - "Repair 'direct evidence is unbiased evidence'."
    - "Repair 'representative sample repairs internal bias'."
    - "Repair 'high certainty for one outcome means a strong recommendation'."
    - "Repair 'ROBINS-I V2 is a finalized 2025 standard'."
  integration:
    - "Given one randomized result, identify the effect of interest and map possible bias mechanisms to RoB 2 domains before making an overall judgment."
    - "Given one non-randomized intervention study, specify a target trial and identify confounding/selection/data gaps that prevent direct emulation."
    - "Given a body estimate, CI and decision threshold, judge whether imprecision could move the true effect across decision-relevant ranges."
    - "Given heterogeneous studies, decide whether inconsistency is decision-relevant using F0.7 reasoning rather than I2 alone."
    - "Given evidence and target PICOTS/context, identify which differences are plausibly effect-relevant and which are merely descriptive."
    - "Given small-study/funnel information, state what dissemination bias is plausible and what remains unproven."
    - "Compare the integrated Evidence Bodies A and B and explain why similar point estimates do not imply similar certainty/applicability."
    - "Complete all thirteen F0.8 audit fields before writing a final interpretation."

notebooklm_tasks:
  - "Act as a Socratic examiner. Whenever the learner says 'quality', force them to specify reporting, result-level RoB, certainty, applicability or recommendation strength."
  - "Generate paired studies with similar reporting quality but different bias mechanisms, and paired studies with different reporting completeness but unresolved true methods."
  - "Generate randomized-result cases for each RoB 2 domain and require a result-specific rationale rather than a numerical quality score."
  - "Generate one trial with an objective outcome and a subjective outcome so the learner must produce different RoB judgments for the two results."
  - "Generate non-randomized intervention scenarios and require a target-trial specification before discussing ROBINS-I domains."
  - "Ask the learner to state 'ROBINS-I V2 Nov-2025 is a draft' before any V2-specific domain exercise."
  - "Generate bodies with identical p-values but different bias, inconsistency, indirectness and imprecision to block significance-as-certainty reasoning."
  - "Generate high-certainty trivial-effect and low-certainty apparently large-effect cases to separate magnitude from certainty."
  - "Generate forest/evidence summaries where I2 is high but all effects remain within one decision category, and low-I2 examples with major clinical indirectness."
  - "Generate evidence-versus-target PICO tables and ask which mismatches plausibly change effect transfer or baseline absolute impact."
  - "Generate CIs around a practical threshold and require explicit imprecision reasoning from F0.5."
  - "Generate funnel/small-study scenarios and prohibit publication-bias diagnosis from symmetry/asymmetry alone."
  - "Generate cases with strong internal validity but poor target applicability, and direct target populations with substantial internal bias."
  - "Generate one-outcome certainty summaries and require the learner to list what additional information is needed before any recommendation-strength judgment."
  - "Use the integrated two-body scenario and require all thirteen audit fields in order before allowing a conclusion."

evidence_critique_task:
  title: "Integrated F0.8 two-body audit"
  target_question: "In trained adult endurance athletes, does Intervention X versus control improve a standardized performance score after about 12 weeks? Higher is better. Practical-benefit threshold = +1.0 point."
  body_A:
    design: "Four randomized parallel trials."
    context: "Predominantly trained adults; intervention/dose/duration close to target."
    conduct: "Adequate randomization/concealment; automated or blinded primary performance assessment; low differential missingness; primary analyses consistent with registrations."
    pooled_effect: "MD +1.5 [1.2, 1.8]."
    study_effects: "+1.2, +1.4, +1.6, +1.7."
    heterogeneity: "No material unexplained heterogeneity."
  body_B:
    design: "Five non-randomized cohort studies."
    context: "Mostly recreational/untrained adults; Intervention X self-selected; most follow-up 2-4 weeks rather than 12 weeks."
    bias_structure: "Higher baseline motivation/training volume predicts X use; training volume measured crudely; completers-only analysis after differential dropout; subjective performance proxy in three studies."
    pooled_effect: "Transformed MD-equivalent +1.6 [-0.2, 3.4]."
    study_effects: "Range -0.3 to +3.8; larger estimates concentrated in short-duration studies."
    moderator_status: "No prespecified moderator analysis."
  required_analysis:
    - "Use the same +1.0 decision threshold for both bodies."
    - "Do not call Body A trustworthy merely because it is randomized; identify result-level mechanisms."
    - "Do not dismiss Body B merely because it is non-randomized; identify target-trial/confounding/selection limitations."
    - "Separate risk of bias from precision."
    - "Judge inconsistency using effect pattern and decision ranges, not I2 alone."
    - "Judge indirectness against trained endurance athletes at about 12 weeks and the target performance construct."
    - "Judge imprecision from each CI relative to +1.0 and other plausible ranges."
    - "State what missing/dissemination evidence is or is not known; do not invent a funnel diagnosis."
    - "Produce a relative certainty judgment for each body with transparent reasons rather than treating categories as points."
    - "Produce a separate target applicability judgment for each body."
    - "State why certainty/applicability alone do not fully determine recommendation strength."
    - "Complete all thirteen audit fields before the final synthesis."

critical_fails:
  - "CONSORT/STROBE/PRISMA complete = low risk of bias/high quality."
  - "One total quality score substitutes for domain-specific bias reasoning."
  - "Randomized = automatically low risk of bias."
  - "Observational/non-randomized = automatically high risk or unusable without mechanism-specific appraisal."
  - "Low certainty = no effect."
  - "High certainty = large or practically important effect."
  - "Statistical significance = high certainty."
  - "Direct evidence = unbiased evidence."
  - "Representative sample repairs confounding/selection/measurement bias."
  - "Certainty is a global score for a paper."
  - "Certainty of one outcome = recommendation strength."
  - "ROBINS-I V2 Nov-2025 described as finalized rather than draft."
  - "I2 alone determines inconsistency/certainty."
  - "Funnel symmetry/asymmetry diagnoses absence/presence of publication bias."
  - "Imprecision judged from p-value alone rather than estimate + CI + decision threshold."

initial_corpus_exclusions:
  - "F0.8 EXERCISES.md — excluded to preserve independent assessment."
  - "F0.8 ANSWER_KEY.md — excluded to prevent answer contamination."
  - "F0.8 production QA_REPORT.md — excluded from learner retrieval because it documents production validation rather than the target concepts."
  - "F0.4 ENTRY_DIAGNOSTIC.md — excluded; remains UNOBSERVED."
  - "Full SOURCE_INDEX.md — excluded to avoid unnecessary retrieval noise."
  - "Full RoB 2/ROBINS-I downloadable tool documents — not committed or bundled; use official links and only if needed for later advanced practice."
  - "Full formal ROB-ME implementation — not required for first-pass F0.8."
  - "Exhaustive GRADE domain manuals, Evidence-to-Decision implementation and guideline-panel procedures — beyond first-pass scope."
  - "F0.9 full-paper practicum materials — deferred."
  - "Substantive sports-nutrition efficacy papers — not part of this methodological package."
```

## Source/version verification — 2026-09-09

External sources actually included in manifest v1 were rechecked before package creation:

1. **riskofbias.info / RoB 2** — official page identifies the current individually randomized parallel-group version as `22 August 2019`.
2. **riskofbias.info / ROBINS-I V2** — official page identifies a revised V2 posted `20 November 2025`, explicitly still a draft and subject to change.
3. **GRADE overview** — current GRADE Book chapter last modified `12 May 2026`; maintains four certainty categories, core downgrading domains and explicit separation of certainty from recommendation strength.
4. **GRADE intervention-certainty principles** — current chapter last modified `21 August 2025`; uses threshold/range-aware body/outcome reasoning and records both basic and structured-ROBINS-I approaches to NRSI starting certainty.
5. **GRADE indirectness** — current chapter last modified `12 May 2026`; uses PICO alignment and requires a plausible material effect/absolute-impact consequence rather than automatic downgrading for any difference.
6. **STROBE** — official site continues to state that its recommendations concern reporting and that the checklist is not an instrument for evaluating observational-study quality.

No external source-version change required modification of the approved F0.8 lesson before building this package.

## Setup instructions for NotebookLM

For the first study pass, add only the six approved sources above. Prefer official webpages/URLs rather than copying third-party PDFs into the public repository. If an official source cannot be imported directly, add it manually in NotebookLM using the official URL or a legally obtained local copy; do not commit that copy to this repository unless redistribution is clearly permitted.

Do **not** add `EXERCISES.md`, `ANSWER_KEY.md` or the F0.4 diagnostic to the first-pass notebook.

## Authority rule

If NotebookLM generates a claim that conflicts with the canonical F0.8 lesson or appears unsupported by the six approved sources, treat it as an unresolved claim. Verify independently before changing GitHub. NotebookLM is a retrieval/study layer, not the canonical source of project state or scientific truth.
