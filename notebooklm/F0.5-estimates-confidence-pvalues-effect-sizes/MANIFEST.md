# F0.5 — NotebookLM Manifest

**Package state:** `READY_FOR_STUDY`
**Manifest version:** `1`
**Built/verified:** `2026-09-09`
**Learner state affected:** none
**F0.4 quantitative diagnostic affected:** none; remains `UNOBSERVED`

This manifest defines the approved first-pass NotebookLM corpus for `F0.5 — Estimates, confidence intervals, p-values, effect sizes and practical relevance`. GitHub remains canonical; NotebookLM is a controlled study layer.

The corpus is intentionally limited to **six sources**. The required interpretation sequence is:

`Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`

F0.5 must not collapse interpretation to `significant / nonsignificant`, and it must not pull formal Type I/II error, power, multiplicity or analytical-flexibility machinery forward from F0.6.

```yaml
module_id: "F0.5"
module_title: "Estimates, confidence intervals, p-values, effect sizes and practical relevance"
version: 1
learning_objectives:
  - "Distinguish parameter, estimator, estimate, point estimate and interval estimate."
  - "Carry the F0.4 distinction SD ≠ SE into estimate precision without using SE as individual variability."
  - "Interpret a frequentist confidence interval as a repeated-sampling procedure result under assumptions, not as posterior probability for a fixed parameter."
  - "Use compatibility language cautiously: identify effect values relatively compatible with the data/model without treating all values inside a CI as equally probable or values outside as impossible."
  - "Identify the null value as 0 for difference measures and 1 for ratio measures."
  - "State and apply all six ASA p-value principles in the learner's own words."
  - "Repair common errors such as p<0.05 = true/important, p>0.05 = no effect, and p = probability that H0 is true."
  - "Separate direction, magnitude, precision and statistical output rather than using a significance label as the conclusion."
  - "Distinguish mean difference from standardized mean difference and reject universal practical-importance labels for SMD."
  - "Calculate and interpret risk difference, risk ratio and odds ratio at an applied level while keeping RR and OR distinct."
  - "Require absolute baseline context when interpreting relative effects for practical meaning."
  - "Use log-scale intuition for ratio measures at P1 level: null 1, reciprocal effects and symmetric visualization after logarithmic transformation."
  - "Use a smallest effect of interest / decision threshold to distinguish practically trivial, practically relevant and indeterminate ranges."
  - "Distinguish a precise near-null estimate that excludes meaningful effects from an imprecise nonsignificant estimate that leaves important benefit/harm compatible with the data."
  - "Interpret forest-plot rows and synthetic trial tables using the six-block sequence."
  - "Keep systematic bias, causal validity and applicability separate from statistical precision."
  - "Defer formal Type I/II error, power, multiplicity, FWER/FDR and analytical flexibility to F0.6."

sources:
  - source_id: "F0-R05"
    priority: "CORE"
    citation: "Sports Nutrition Mastery. F0.5 — Estimativas, intervalos de confiança, p-values, effect sizes e relevância prática. Canonical project lesson, version current at manifest v1."
    url_or_doi: "https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.5-estimates-confidence-pvalues-effect-sizes/LESSON.md"
    why_included: "Primary instructional spine defining the exact project sequence, formulas, worked synthetic examples, practical-threshold reasoning, anti-errors and F0.6 boundary."
    limitation: "Project-authored teaching material, not an independent methodological authority. Claims remain traceable to the external sources below."

  - source_id: "F0-S06"
    priority: "CORE"
    citation: "Higgins JPT, Li T, Deeks JJ, editors. Chapter 6: Choosing effect measures and computing estimates of effect. Cochrane Handbook for Systematic Reviews of Interventions, version 6.5. Cochrane; 2024. Chapter last updated August 2023."
    url_or_doi: "https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-06"
    why_included: "External anchor for effect-measure scale logic: mean difference, standardized mean difference, risk difference, risk ratio, odds ratio, difference versus ratio measures, null values, uncertainty and log-scale treatment of ratios."
    limitation: "Written for evidence synthesis and broader than F0.5. Do not import meta-analysis mechanics or advanced unit-of-analysis methods into this package."

  - source_id: "F0-S08"
    priority: "CORE"
    citation: "Wasserstein RL, Lazar NA. The ASA Statement on p-Values: Context, Process, and Purpose. The American Statistician. 2016;70(2):129-133. doi:10.1080/00031305.2016.1154108."
    url_or_doi: "https://www.amstat.org/asa/files/pdfs/P-ValueStatement.pdf"
    why_included: "Authoritative source for the six ASA principles and the core prohibition against treating a p-value as probability of a hypothesis, effect magnitude, practical importance or a standalone scientific decision rule."
    limitation: "Principles document, not a complete inferential-statistics course and not a replacement for effect-estimation or confidence-interval teaching."

  - source_id: "F0-S28"
    priority: "SUPPORT"
    citation: "Greenland S, Senn SJ, Rothman KJ, et al. Statistical tests, P values, confidence intervals, and power: a guide to misinterpretations. European Journal of Epidemiology. 2016;31:337-350. doi:10.1007/s10654-016-0149-3."
    url_or_doi: "https://pmc.ncbi.nlm.nih.gov/articles/PMC4877414/"
    why_included: "Focused misinterpretation safeguard for p-values and confidence intervals; supports repeated-sampling coverage logic, probability-reversal corrections and compatibility-oriented language."
    limitation: "Includes extensive power material beyond F0.5. Use CI/p-value interpretation only; formal power remains F0.6."

  - source_id: "F0-S13"
    priority: "SUPPORT"
    citation: "Lakens D. Sample Size Justification. Collabra: Psychology. 2022;8(1):33267. doi:10.1525/collabra.33267."
    url_or_doi: "https://online.ucpress.edu/collabra/article/8/1/33267/120491/Sample-Size-Justification"
    why_included: "Supports smallest-effect-of-interest and informativeness reasoning: effects that matter should be justified from theory/practical consequences rather than generated by a significance threshold."
    limitation: "Much of the article concerns sample-size justification and power. F0.5 uses only smallest-effect and decision-relevance concepts; design/power calculations remain F0.6."

  - source_id: "F0-S09"
    priority: "CONTRAST"
    citation: "ASA President's Task Force Statement on Statistical Significance and Replicability. American Statistical Association / IMS; 2021."
    url_or_doi: "https://magazine.amstat.org/blog/2021/08/01/task-force-statement-p-value/"
    why_included: "Contrast source preventing an overcorrection: p-values and significance tests can remain useful when properly applied and interpreted, but must sit within uncertainty, variability, replicability, multiplicity and context."
    limitation: "High-level statement rather than a technical manual. Multiplicity and replicability mechanics are not taught in detail until later modules."

claims_to_master:
  - "Parameter, estimator and estimate are different objects; an estimate is not the unknown parameter itself."
  - "A point estimate gives one observed magnitude; an interval adds uncertainty and should be interpreted with the estimate rather than replacing it."
  - "A frequentist 95% confidence level describes long-run coverage of a valid procedure under assumptions; it is not a 95% posterior probability that the fixed parameter lies in one observed interval."
  - "A CI can be used as a compatibility range under the model/assumptions, but points inside are not equally probable and points outside are not impossible."
  - "Null values depend on effect scale: 0 for differences and 1 for ratios."
  - "A p-value is conditional on a specified statistical model/test and does not equal P(H0|data)."
  - "P-values do not measure effect magnitude or practical importance."
  - "Crossing 0.05 is not a scientific phase transition; p=0.049 and p=0.051 should not automatically produce opposite substantive conclusions."
  - "A small p-value can accompany a practically trivial effect; a large p-value can accompany an imprecise estimate compatible with important effects."
  - "A precise interval near the null can be informative when it excludes prespecified effects that would matter."
  - "Mean difference preserves original units; standardized mean difference expresses the difference in SD units and has no universal practical-importance threshold."
  - "Risk difference is absolute; risk ratio and odds ratio are relative ratio measures and are not interchangeable."
  - "The practical meaning of a relative effect depends on baseline absolute risk."
  - "Ratio measures have null 1 and are naturally represented/analyzed on a log scale because reciprocal effects become symmetric."
  - "A smallest effect of interest is contextual and must be justified; it is not derived from the observed p-value."
  - "Precision is not validity: narrow CIs do not repair confounding, selection bias, measurement bias or model misspecification."
  - "The correct endpoint of interpretation is direction + magnitude + precision + statistical output + practical context + unsupported claims, not a binary significance label."

controversies_or_limits:
  - "Compatibility language is a pedagogical aid, not a posterior probability statement and not a claim that every value in the interval is equally plausible."
  - "CI construction depends on model, design and standard-error assumptions; the simple normal approximation is not universal."
  - "Effect-size labels such as small/medium/large are context dependent and cannot substitute for domain-specific thresholds."
  - "RR and OR may be numerically similar for rare events but can diverge substantially when events are common."
  - "A decision threshold may depend on benefits, harms, cost, burden, feasibility and target context; there is no universal sports-nutrition SESOI."
  - "Cochrane Chapter 6 is an evidence-synthesis chapter, not a first-principles statistics textbook."
  - "Greenland et al. and Lakens contain formal power/sample-size content that must not be pulled into F0.5."
  - "ASA 2021 is used to avoid the false binary 'p-values are good' versus 'p-values are useless'; F0.5 teaches conditional use rather than ideological acceptance/rejection."
  - "Synthetic sports/nutrition examples in the canonical lesson are methodological illustrations, not intervention evidence or recommendations."

active_recall:
  basic:
    - "Distinguish parameter, estimator, estimate, point estimate and interval estimate."
    - "What does 95% mean in a frequentist confidence interval procedure?"
    - "State the null value for MD/RD and for RR/OR."
    - "State all six ASA p-value principles in your own words."
    - "Define MD, SMD, RD, RR and OR."
    - "Define smallest effect of interest / decision threshold."
  mechanism:
    - "Explain why SE affects interval width but does not describe individual variability."
    - "Explain why a narrow CI can still surround a biased estimate."
    - "Explain why p can shrink with more information even when effect magnitude is unchanged."
    - "Explain why RR=0.50 can correspond to very different absolute effects at different baselines."
    - "Explain why OR should not be read as RR automatically."
    - "Explain why reciprocal ratio effects are symmetric on a log scale."
  evidence_critique:
    - "Repair 'p=0.03 means a 3% chance H0 is true'."
    - "Repair '95% CI means a 95% chance the true value is inside this observed interval'."
    - "Repair 'p>0.05 proves no effect'."
    - "Repair 'CI excludes zero, therefore the effect is important'."
    - "Repair 'SMD=0.8 is universally large and meaningful'."
    - "Repair 'RR=0.5 means large practical benefit' when baseline risk is absent."
  integration:
    - "For every forest-plot row output exactly: Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims."
    - "Compare a narrow CI fully inside a trivial-effect zone with a wide CI spanning harm, null and meaningful benefit."
    - "Given the same RR at two baselines, calculate/compare absolute effects before judging practical importance."
    - "Given MD and a pooled SD, compute SMD then explain why the standardized value alone cannot establish practical importance."
    - "Given a synthetic trial result, identify which conclusions require F0.2/F0.3 causal validity rather than F0.5 statistics."

notebooklm_tasks:
  - "Act as a Socratic examiner. Present one quantitative result at a time and wait for the learner's complete six-block interpretation before grading."
  - "Require the learner to name the effect measure and its null value before interpreting direction."
  - "Generate paired p-values around 0.05 with nearly identical estimates/intervals and require rejection of threshold discontinuity."
  - "Generate p-small/trivial-effect and p-large/imprecise-important-effect contrasts."
  - "Generate narrow near-null intervals that exclude the prespecified meaningful zone and ask why this can be informative."
  - "Generate MD/SMD conversion tasks and prohibit automatic Cohen-label practical conclusions."
  - "Generate paired binary examples with identical RR but different baseline risks and require RD/absolute interpretation."
  - "Generate RR versus OR traps, especially with common outcomes."
  - "Generate forest-plot rows on both difference and ratio scales and require correct null identification."
  - "Ask the learner to state exactly which assumptions/design information CI/p-value cannot repair or establish."
  - "Never teach formal alpha/beta, power formulas, post hoc observed power, FWER/FDR or multiplicity corrections in this package."
  - "Cite only the approved six-source corpus and explicitly state when a claim requires F0.6 or causal/risk-of-bias material outside this notebook."
```

## Evidence-critique task

Use only the approved F0.5 corpus to appraise this synthetic report:

> Trial A reports `MD = +0.20`, `95% CI = +0.05 to +0.35`, `p=0.01`; a prespecified smallest effect of interest is `+1.0`. Trial B reports `MD = +1.40`, `95% CI = −0.84 to +3.64`, `p≈0.22`; the same threshold applies. Authors summarize: “A clearly works because it is significant; B does not work because it is nonsignificant.”

Required outputs:

1. identify the target effect measure and null value;
2. interpret Trial A by direction, magnitude and precision;
3. compare Trial A's entire interval to the practical threshold;
4. interpret what `p=0.01` does and does not say;
5. interpret Trial B's direction, magnitude and precision;
6. identify which practical zones remain compatible with Trial B;
7. explain why `p≈0.22` is not evidence of no effect;
8. state one bounded conclusion for A and one for B;
9. state which causal-validity questions remain outside F0.5.

## Corpus exclusions

Do **not** add to the initial NotebookLM corpus:

- `foundations/F0-scientific-literacy/F0.5-estimates-confidence-pvalues-effect-sizes/EXERCISES.md` — independent assessment;
- `foundations/F0-scientific-literacy/F0.5-estimates-confidence-pvalues-effect-sizes/ANSWER_KEY.md` — answer leakage;
- F0.5 production `QA_REPORT.md` — metadata, not study evidence;
- `foundations/F0-scientific-literacy/F0.4-descriptive-statistics/ENTRY_DIAGNOSTIC.md` — prerequisite diagnostic remains uncontaminated and `UNOBSERVED`;
- full `SOURCE_INDEX.md` — retrieval noise;
- FDA multiplicity guidance / F0-S10 — F0.6;
- formal power chapters/calculators — F0.6;
- GRADE and risk-of-bias tools — later modules;
- sports-nutrition intervention papers — this package teaches statistical interpretation, not substantive nutrition efficacy.

## Version/access integrity — verified 2026-09-09

- Canonical F0.5 lesson exists on `main` and is `APPROVED`.
- Cochrane Chapter 6 remains the current Chapter 6 of Handbook version 6.5; page states last updated August 2023 and currently exposes MD/SMD/RD/RR/OR and difference-versus-ratio scale logic.
- Official ASA p-value statement remains accessible with its six principles.
- Greenland et al. remains available open access through PMC under CC BY 4.0.
- Lakens 2022 remains available through University of California Press and explicitly discusses justification of smallest effects of interest.
- ASA Task Force 2021 remains accessible and explicitly states that properly applied p-values/significance tests remain useful tools rather than methods that must be abandoned.
- No source-version change found on 2026-09-09 requires modification of the approved F0.5 lesson.

## Copyright/public-repository rule

The public GitHub repository stores only project-authored Markdown, citations and links. Do not commit third-party PDFs/articles/chapters unless redistribution permission is explicit. Open-access status does not require copying a source into GitHub; linking is preferred.

## Completion criterion

The package is correctly configured when:

- exactly six approved sources are loaded;
- exercises, answer key, production QA and F0.4 diagnostic are absent;
- all six ASA principles can be explained and applied;
- frequentist CI is never expressed as posterior probability;
- p-value is never treated as effect magnitude, practical importance or probability of H0;
- MD/SMD and RD/RR/OR are kept distinct;
- baseline absolute risk accompanies practical interpretation of relative effects;
- practical thresholds distinguish trivial, meaningful and unresolved effect ranges;
- narrow near-null intervals can be recognized as informative when they exclude meaningful effects;
- wide intervals are not converted into 'no effect';
- forest/trial interpretation follows the six-block sequence;
- F0.6 power/multiplicity machinery is not pulled forward;
- no learner state or F0.4 diagnostic state changes without observed performance.