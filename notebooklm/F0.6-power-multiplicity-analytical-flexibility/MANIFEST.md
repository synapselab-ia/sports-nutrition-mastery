# F0.6 — NotebookLM Manifest

**Package state:** `READY_FOR_STUDY`
**Manifest version:** `1`
**Built/verified:** `2026-09-09`
**Learner state affected:** none
**F0.4 quantitative diagnostic affected:** none; remains `UNOBSERVED`

This manifest defines the approved first-pass NotebookLM corpus for `F0.6 — Power, Type I/II error, multiplicity and analytical flexibility`. GitHub remains canonical; NotebookLM is a controlled study layer.

The corpus is intentionally limited to **eight sources**. The required study-audit sequence is:

`Target claims → Decision rules → Power/sample-size assumptions → Effective hypothesis family → Analytical paths → Prespecification evidence → Multiplicity control → Estimate/CI interpretation → Confirmatory vs exploratory → Transparent conclusion`

F0.6 must preserve the F0.5 rule that completed-study interpretation uses magnitude + confidence interval + practical threshold. It must not use observed/post hoc power calculated from the observed effect as an explanation of a completed result, and it must not pull full systematic-review/meta-analysis/heterogeneity machinery forward from F0.7.

```yaml
module_id: "F0.6"
module_title: "Power, Type I/II error, multiplicity and analytical flexibility"
version: 1
learning_objectives:
  - "Define Type I error and alpha in repeated-use/decision-rule terms without converting alpha into a posterior probability about H0."
  - "Define Type II error and beta relative to a specified alternative/effect, design and model assumptions."
  - "Define power as 1-beta for a specified true effect/design/model and reject power=P(H1 true)."
  - "Reject 1-power as the posterior probability that one nonsignificant result is a false negative."
  - "Interpret a power curve conceptually and explain why a power statement is incomplete without the assumed effect and design assumptions."
  - "Distinguish prospective power from observed precision and use estimate + CI + practical threshold for completed-study interpretation."
  - "Explain why observed/post hoc power calculated from the observed effect is generally redundant or misleading."
  - "Compare a-priori power, desired precision/accuracy, near-census, resource constraints and other transparent sample-size justifications."
  - "Tie sample-size planning to the inferential goal and to a justified smallest effect of interest/planning effect when appropriate."
  - "Define a family of hypotheses relative to intended confirmatory claims rather than mechanically counting every printed p-value."
  - "Recognize multiplicity arising from endpoints, time points, subgroups, alternative models/analytical paths and stopping/data-dependent choices."
  - "Calculate and interpret simple illustrative family-wise false-positive risk under explicitly stated independent-test assumptions."
  - "Explain endpoint hierarchy/gatekeeping, alpha allocation and adjusted outputs at a conceptual level without memorizing an exhaustive correction catalog."
  - "Distinguish hypothesis multiplicity from analytical-path multiplicity."
  - "Reject significant-in-A plus nonsignificant-in-B as proof of a subgroup interaction."
  - "Identify researcher degrees of freedom and explain how data-dependent selection can distort confirmatory inference."
  - "Distinguish trial registration, preregistration, protocol and statistical analysis plan (SAP)."
  - "Use timing, versioning and documented deviations to audit what was genuinely prespecified."
  - "Explain why preregistration improves auditability but does not guarantee low risk of bias, correct measurement, valid design or practical importance."
  - "Distinguish confirmatory from exploratory outputs without treating exploratory science as invalid."
  - "Audit an unfamiliar study using the ten-field F0.6 sequence while preserving F0.5 magnitude/CI interpretation."
  - "Defer full meta-analysis, heterogeneity/I2, publication-bias methods and meta-regression to F0.7."

sources:
  - source_id: "F0-R06"
    priority: "CORE"
    citation: "Sports Nutrition Mastery. F0.6 — Power, Type I/II error, multiplicidade e flexibilidade analítica. Canonical project lesson, version current at manifest v1."
    url_or_doi: "https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.6-power-multiplicity-analytical-flexibility/LESSON.md"
    why_included: "Primary instructional spine defining the exact project vocabulary, worked examples, critical fails, ten-field audit sequence and F0.5/F0.7 boundaries."
    limitation: "Project-authored teaching material, not an independent methodological authority. Material claims remain traceable to the external sources below."

  - source_id: "F0-S08"
    priority: "CORE"
    citation: "Wasserstein RL, Lazar NA. The ASA Statement on p-Values: Context, Process, and Purpose. The American Statistician. 2016;70(2):129-133. doi:10.1080/00031305.2016.1154108."
    url_or_doi: "https://www.amstat.org/asa/files/pdfs/P-ValueStatement.pdf"
    why_included: "Core safeguard for model-conditional p-value reasoning, threshold misuse, full reporting/transparency, effect-importance separation and selective-analysis awareness."
    limitation: "Not a complete power or multiplicity manual. Type I/II/power and multiplicity mechanics are integrated through the canonical lesson and the dedicated sources below."

  - source_id: "F0-S10"
    priority: "CORE"
    citation: "U.S. Food and Drug Administration. Multiple Endpoints in Clinical Trials: Guidance for Industry. Final Guidance. October 2022."
    url_or_doi: "https://www.fda.gov/regulatory-information/search-fda-guidance-documents/multiple-endpoints-clinical-trials"
    why_included: "Direct external anchor for why multiple endpoints can increase false-conclusion risk and for conceptual grouping, ordering/hierarchy and multiplicity-management strategies in confirmatory trials."
    limitation: "Regulatory guidance for human drug/biologic development. F0.6 transfers inferential principles cautiously and does not universalize FDA regulatory requirements to sports/exercise research."

  - source_id: "F0-S13"
    priority: "CORE"
    citation: "Lakens D. Sample Size Justification. Collabra: Psychology. 2022;8(1):33267. doi:10.1525/collabra.33267."
    url_or_doi: "https://online.ucpress.edu/collabra/article/8/1/33267/120491/Sample-Size-Justification"
    why_included: "Primary anchor for transparent sample-size justification, a-priori power as one possible design goal, desired accuracy/precision, finite-population/resource rationales and smallest-effect planning."
    limitation: "Broad methodological review. F0.6 does not require exhaustive software-specific power calculations or a universal target power convention."

  - source_id: "F0-S28"
    priority: "SUPPORT"
    citation: "Greenland S, Senn SJ, Rothman KJ, et al. Statistical tests, P values, confidence intervals, and power: a guide to misinterpretations. European Journal of Epidemiology. 2016;31:337-350. doi:10.1007/s10654-016-0149-3."
    url_or_doi: "https://pmc.ncbi.nlm.nih.gov/articles/PMC4877414/"
    why_included: "Probability-reversal safeguard for p-values, confidence intervals and power; also supports the warning that analysis-selection protocols can distort p-values and that frequentist error rates are not posterior probabilities about hypotheses."
    limitation: "Broad critical tutorial. Use it for misconception repair and conditional/repeated-use reasoning, not as a substitute for a full power-analysis textbook."

  - source_id: "F0-S29"
    priority: "SUPPORT"
    citation: "Heinsberg LW, Weeks DE. Post hoc Power is Not Informative. Genetic Epidemiology. 2022;46(7):390-394. doi:10.1002/gepi.22464."
    url_or_doi: "https://pmc.ncbi.nlm.nih.gov/articles/PMC9452450/"
    why_included: "Focused source demonstrating why observed/post hoc power computed after seeing the data is misleading/redundant for interpreting a completed study and why estimate/CI plus design reasoning should be used instead."
    limitation: "Methodological commentary with simulation, focused narrowly on post hoc power. It does not replace prospective planning guidance."

  - source_id: "F0-S01"
    priority: "SUPPORT"
    citation: "Hopewell S, Chan AW, Collins GS, et al. CONSORT 2025 statement: updated guideline for reporting randomised trials. BMJ. 2025;389:e081123."
    url_or_doi: "https://www.bmj.com/content/389/bmj-2024-081123"
    why_included: "Audit-trail source for trial registration, access to protocol/SAP, prespecified versus post hoc analyses, and transparent documentation of important changes after trial commencement."
    limitation: "Reporting guideline rather than a risk-of-bias score or proof that a prespecified design/analysis is scientifically correct."

  - source_id: "F0-S09"
    priority: "CONTRAST"
    citation: "ASA President's Task Force Statement on Statistical Significance and Replicability. American Statistical Association / Institute of Mathematical Statistics; 2021."
    url_or_doi: "https://magazine.amstat.org/blog/2021/08/01/task-force-statement-p-value/"
    why_included: "Contrast source preventing the false overcorrection that p-values/significance testing are intrinsically useless; emphasizes uncertainty, variability, multiplicity, replicability, model choice, selective reporting and transparent analysis."
    limitation: "High-level statement, not a technical multiplicity or sample-size manual."

claims_to_master:
  - "Alpha is a repeated-use Type I error property of a specified decision rule under null/model assumptions; it is not P(H0|data)."
  - "Beta and power depend on the alternative/effect and design assumptions; there is no context-free universal power value for a study."
  - "Power is P(reject H0 | specified true effect, design/model assumptions) before observing the data, not P(H1 true | data)."
  - "1-power is not the probability that one observed nonsignificant result is a false negative."
  - "Increasing n generally increases power and precision, but neither repairs systematic bias or confounding."
  - "A stricter alpha generally lowers power at fixed n/effect; greater true effect and lower residual variability generally increase power, all else comparable."
  - "After a study is completed, estimate + CI + practical threshold are the primary objects for judging observed precision/informativeness."
  - "Observed/post hoc power computed from the observed effect does not add independent evidence about whether an effect is present or absent."
  - "Sample-size justification should follow the inferential goal; a-priori power is one legitimate strategy, not the only legitimate strategy."
  - "A planning effect or smallest effect of interest must be justified independently of the observed p-value."
  - "Multiplicity is created by opportunities to select favorable claims/results, including endpoints, time points, subgroups, models and data-dependent stopping/analysis choices."
  - "A family of hypotheses is defined by intended claims/decision strategy, not by the physical layout of tables or every p-value printed in a paper."
  - "Under the simplified case of m independent tests with all relevant nulls true and per-test alpha .05, P(at least one Type I rejection)=1-.95^m; this is an illustration, not a universal formula for correlated outcomes."
  - "Endpoint hierarchy/gatekeeping, alpha allocation, multiplicity-adjusted outputs and explicit exploratory labeling are conceptual strategies for protecting confirmatory inference."
  - "Alternative models may be analytical paths for one scientific claim rather than separate hypotheses; choosing the most favorable path after seeing results can still distort inference."
  - "Significant in subgroup A and nonsignificant in subgroup B does not prove the subgroups differ; direct interaction reasoning is required."
  - "Trial registration, preregistration, protocol and SAP differ in purpose and detail; timing/versioning determine what evidence they provide about prespecification."
  - "Prespecification improves transparency/auditability but does not guarantee valid measurement, low bias, correct modeling, adequate precision or practical importance."
  - "Exploratory findings can be useful; the error is relabeling post hoc exploration as prespecified confirmation."
  - "The final interpretation of a completed result must still use the F0.5 chain: target/measure, direction, magnitude, CI/precision, statistical output, practical meaning and unsupported claims."

controversies_or_limits:
  - "Frequentist power/error rates are conditional on specified models, true effects and design assumptions; they are not posterior probabilities about hypotheses."
  - "There is no universal 80% power rule that automatically makes a study adequate; adequacy depends on the inferential goal and effect/precision target."
  - "Power analysis based on an inflated effect from a prior small study can itself be misleading; planning effects require defensible external justification."
  - "Observed power is distinct from a design-sensitivity calculation using an externally specified effect after data collection; neither should be converted into posterior evidence about the observed result."
  - "The simplified independent-test FWER formula overstates or understates real joint error when tests are correlated or when the testing procedure differs."
  - "Not every analysis in a paper belongs to one confirmatory family, but exploratory labeling does not erase selective-reporting concerns."
  - "Bonferroni is a simple illustration, not a universally optimal correction."
  - "Registration/protocol/SAP existence alone does not prove that analyses were finalized before relevant data were seen; timestamps, versions and deviations matter."
  - "CONSORT supports transparency but is not a quality/risk-of-bias score."
  - "FDA guidance is regulatory and context-specific; its inferential principles must not be presented as universal legal requirements."
  - "Synthetic sports/nutrition examples in the canonical lesson are methodological exercises, not intervention evidence or recommendations."
  - "Full systematic-review/meta-analysis, heterogeneity/I2, publication-bias methods and meta-regression belong to F0.7."

active_recall:
  basic:
    - "Define Type I error and alpha without using P(H0|data)."
    - "Define Type II error, beta and power for a specified effect/design."
    - "Why is '80% power' incomplete without the planning effect and assumptions?"
    - "Distinguish power from precision."
    - "List at least five sources of multiplicity."
    - "Define family of hypotheses, trial registration, preregistration, protocol and SAP."
  mechanism:
    - "Explain why increasing n can increase power while leaving systematic bias unchanged."
    - "Explain why stricter alpha tends to reduce power at fixed n/effect."
    - "Explain why observed power based on the observed effect is linked to the observed result and is not independent evidence."
    - "Explain why multiple endpoints/time points increase selection opportunities."
    - "Explain why alternative models can create analytical-path multiplicity without being separate scientific hypotheses."
    - "Explain why timing/versioning changes the evidentiary value of a protocol or SAP."
  evidence_critique:
    - "Repair '80% power means an 80% chance H1 is true'."
    - "Repair '1-power is the chance this nonsignificant result is a false negative'."
    - "Repair 'observed power of 25% proves the study missed a real effect'."
    - "Repair 'every p<.05 among 20 endpoints independently confirms efficacy'."
    - "Repair 'significant in men but not women proves an interaction'."
    - "Repair 'preregistered means low risk of bias'."
    - "Repair 'exploratory means scientifically invalid'."
  integration:
    - "Given a planned effect, alpha, n and power target, state exactly what the power statement means and does not mean."
    - "Given a completed estimate/CI and a practical threshold, interpret the result without observed power."
    - "Calculate 1-.95^5 and 1-.95^20, then state the assumptions and why the numbers are not universal."
    - "Reconstruct the effective confirmatory family from endpoints/time points/subgroups and distinguish it from model-path multiplicity."
    - "Audit whether a highlighted result was prespecified by comparing registry, protocol, SAP, timestamps and deviations."
    - "For an unfamiliar study, complete all ten F0.6 audit fields before writing a conclusion."

notebooklm_tasks:
  - "Act as a Socratic examiner. Require definitions of alpha/beta/power in conditional repeated-use terms and reject posterior-probability wording."
  - "Generate power-curve thought experiments varying effect size, n, variability and alpha one factor at a time."
  - "Generate completed-study cases with wide versus narrow CIs and forbid observed-power rescue."
  - "Contrast a-priori power, desired precision, near-census and resource-constrained sample-size justifications."
  - "Generate multiple-endpoint/timepoint designs and make the learner reconstruct the confirmatory family before discussing multiplicity control."
  - "Generate simple independent-test FWER calculations, always requiring assumptions and a warning against universal application to correlated outcomes."
  - "Generate endpoint-hierarchy, alpha-allocation and exploratory-labeling scenarios at conceptual level; do not require an exhaustive adjustment-method catalog."
  - "Generate analytical-flexibility scenarios with alternative covariates, outlier rules, transformations, time windows and subgroup definitions; require separation of scientific hypotheses from analysis paths."
  - "Generate subgroup traps where one subgroup is significant and another is not; require direct interaction reasoning."
  - "Present registry/protocol/SAP snippets with dates and deviations; require a prespecification audit rather than accepting labels at face value."
  - "Require the learner to state what preregistration cannot guarantee."
  - "Use ASA 2016 and ASA 2021 as a paired debate: reject both threshold ritualism and the claim that p-values must always be banned."
  - "Use the ten-field integrated audit on synthetic many-analysis studies."
  - "Cite only the approved eight-source corpus and explicitly label any question requiring F0.7 meta-analysis/heterogeneity as outside scope."
```

## Integrated evidence-critique task

Use only the approved F0.6 corpus to audit this synthetic report.

A randomized study enrolls 120 athletes. Before recruitment, the registry lists time-trial performance at week 12 as the primary outcome, three secondary outcomes at week 12, bilateral alpha `0.05`, planning effect `+2.0%` and target power `80%`. The registry gives no multiplicity strategy for secondary claims, and the paper does not link a SAP.

The paper reports the primary result as `+0.6%`, 95% CI `-0.5% to +1.7%`, `p=0.28`. It also reports having examined 20 outcomes at four time points, six subgroup definitions across the 20 week-12 outcomes and several alternative covariate models. It highlights mood at week 8 (`p=0.008`) and recovery in a high-baseline-fitness subgroup (`p=0.03`) as “confirmatory evidence,” does not provide the complete result set, and calculates observed power from the observed primary effect to explain the nonsignificant primary result.

Required output — exactly these ten fields:

1. **Target claims** — identify the documented primary confirmatory claim and status of secondary claims.
2. **Decision rules** — interpret alpha `.05` without probability reversal.
3. **Power/sample-size assumptions** — explain what 80% power for +2.0% means and does not mean.
4. **Effective hypothesis family** — reconstruct the relevant confirmatory multiplicity problem without mechanically treating every model as an independent hypothesis.
5. **Analytical paths** — identify model/timepoint/subgroup selection opportunities.
6. **Prespecification evidence** — state what the registry establishes and what missing SAP/timing leaves unresolved.
7. **Multiplicity control** — identify absent or unclear hierarchy/adjustment/alpha allocation and propose a transparent strategy.
8. **Estimate/CI interpretation** — interpret the primary result using F0.5; do not use observed power.
9. **Confirmatory vs exploratory** — classify mood-week8 and subgroup results from the information available.
10. **Transparent conclusion** — state what is supported, what is unresolved and what additional documentation/reporting is needed.

## Corpus exclusions

Do **not** add to the initial NotebookLM corpus:

- `foundations/F0-scientific-literacy/F0.6-power-multiplicity-analytical-flexibility/EXERCISES.md` — independent assessment;
- `foundations/F0-scientific-literacy/F0.6-power-multiplicity-analytical-flexibility/ANSWER_KEY.md` — answer leakage;
- F0.6 production `QA_REPORT.md` — production metadata, not study evidence;
- `foundations/F0-scientific-literacy/F0.4-descriptive-statistics/ENTRY_DIAGNOSTIC.md` — prerequisite diagnostic must remain uncontaminated and `UNOBSERVED`;
- full `SOURCE_INDEX.md` — retrieval noise;
- exhaustive multiplicity-correction catalogs or software manuals — beyond F0.6 target;
- formal sequential/adaptive-trial theory — beyond F0.6 target;
- systematic-review/meta-analysis/heterogeneity/I2/publication-bias corpora — F0.7;
- RoB 2/ROBINS-I/GRADE corpora — formal use belongs later;
- substantive sports-nutrition intervention papers — this notebook teaches methodology, not efficacy recommendations.

## Version/access integrity — verified 2026-09-09

- Canonical F0.6 lesson exists on `main` and is `APPROVED`.
- ASA 2016 official PDF remains accessible and explicitly presents six principles, including threshold, transparency and effect-importance safeguards.
- FDA `Multiple Endpoints in Clinical Trials` remains the current **Final Guidance**, dated October 2022, and explicitly addresses false-conclusion risk from multiple endpoints plus grouping/ordering/multiplicity-management strategies.
- Lakens 2022 remains accessible at University of California Press and presents sample-size justification as a design decision tied to what the study aims to learn, including multiple defensible justification approaches.
- Greenland et al. 2016 remains accessible in PMC and continues to provide probability-reversal and p-value/CI/power-misinterpretation safeguards.
- Heinsberg & Weeks 2022 remains accessible in PMC and explicitly concludes that post hoc power should not be used for interpretation of completed-study results.
- CONSORT 2025 remains the current general CONSORT statement, supersedes CONSORT 2010, consists of a 30-item checklist, and includes trial registration, protocol/SAP access and reporting of important non-prespecified changes.
- ASA Task Force 2021 remains accessible on the ASA-hosted page and explicitly states that properly applied p-values/significance tests remain useful while uncertainty, multiplicity, replicability, model choice and selective reporting require attention.
- No source-version change identified on 2026-09-09 requires modification of the approved F0.6 lesson.

## Authority rule

If NotebookLM generates a claim that cannot be traced to this approved corpus, treat it as unverified. Do not promote it to the repository, learner state or later teaching material without independent verification under the project research protocol.
