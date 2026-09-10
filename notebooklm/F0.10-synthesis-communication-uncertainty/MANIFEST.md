# F0.10 — NotebookLM Manifest

**Package state:** `READY_FOR_STUDY`
**Manifest version:** `1`
**Built/verified:** `2026-09-10`
**Learner state affected:** none
**F0.4 quantitative diagnostic affected:** none; remains `UNOBSERVED`

This manifest defines the approved first-pass NotebookLM corpus for `F0.10 — Synthesis and communication of uncertainty`. GitHub remains canonical; NotebookLM is a controlled study layer.

The corpus is intentionally limited to **six sources**. It contains the canonical F0.10 lesson plus only the minimum external methodological support needed to preserve p-value interpretation, threshold/range-aware certainty, indirectness/applicability and the certainty-versus-recommendation boundary.

The canonical workflow is:

`reconstructed evidence → invariant core → calibrated claim → audience translation → drift audit → update conditions`

The package must train **compression without epistemic loss**. It must not import the completed F0.10 assessment or its answer key into the initial corpus.

```yaml
module_id: "F0.10"
module_title: "Synthesis and communication of uncertainty"
version: 1
learning_objectives:
  - "Communicate an already reconstructed evidence judgment without strengthening or weakening it merely because the audience changes."
  - "Freeze an eight-field invariant core before drafting: target, direction, magnitude, precision, threshold, certainty, applicability and boundaries/update conditions."
  - "Preserve point estimate, confidence interval or compatible range, and practical/decision threshold together when they are material."
  - "Distinguish 'did not detect a clear effect', 'evidence compatible with no meaningful effect' and formal equivalence/non-inferiority."
  - "Use p-values as one statistical output rather than a truth, importance or absence detector."
  - "Separate uncertainty caused by imprecision, risk of bias, inconsistency, indirectness and missing/dissemination evidence."
  - "Avoid false balance by weighting evidence according to fit, design/bias, magnitude/precision, compatibility, directness and synthesis context rather than counting papers."
  - "Avoid the opposite error of applying a mechanical evidence pyramid without asking which source is informative for which claim."
  - "Distinguish directness/applicability from internal validity and risk of bias."
  - "Distinguish certainty of a body/outcome effect from recommendation direction or strength."
  - "Translate one evidence synthesis into technical, practitioner-facing and lay-facing versions while preserving the same epistemic content."
  - "Audit language drift after translation and repair any version that becomes broader, more causal or more certain than the technical synthesis."
  - "State explicit update conditions: what new evidence, changed assumption or changed threshold would materially alter the conclusion."

sources:
  - source_id: "F0-R10"
    priority: "CORE"
    citation: "Sports Nutrition Mastery. F0.10 — Synthesis and communication of uncertainty. Canonical project lesson, current at manifest v1."
    url_or_doi: "https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.10-synthesis-communication-uncertainty/LESSON.md"
    why_included: "Primary instructional spine defining the invariant core, calibrated-language workflow, false-balance safeguards, audience-translation rules, drift audit and update-condition requirement."
    limitation: "Project-authored teaching material, not an independent methodological authority. Material statistical/certainty claims remain anchored by the external sources below."

  - source_id: "F0-S19"
    priority: "CORE"
    citation: "Goldkuhle M, Kreuzberger N, Neumann I, et al. Principles for assessing the certainty of interventions. In: The GRADE Book. GRADE Working Group. Last modified 21 August 2025."
    url_or_doi: "https://book.gradepro.org/guideline/principles-for-assessing-the-certainty-of-interventions"
    why_included: "Primary external anchor for certainty as confidence that the true effect lies within a specified range or on a side of a decision threshold, assessed at body/outcome level rather than as a paper-quality score."
    limitation: "GRADE is a structured evidence-body framework. F0.10 uses its certainty/range/threshold logic to calibrate communication, not to turn the lesson into a full guideline-development exercise."

  - source_id: "F0-S18"
    priority: "SUPPORT"
    citation: "Neumann I, Brennan S, Meerpohl J, et al. Overview of the GRADE approach. In: The GRADE Book. GRADE Working Group. Last modified 12 May 2026."
    url_or_doi: "https://book.gradepro.org/guideline/overview-of-the-grade-approach"
    why_included: "Supports the four certainty categories, the separation of certainty of evidence from recommendation strength, and the use of structured evidence-to-decision processes beyond a single outcome statement."
    limitation: "It is an overview, not a substitute for reconstructing effect estimates, risk of bias, indirectness or decision context."

  - source_id: "F0-S20"
    priority: "SUPPORT"
    citation: "Schünemann HJ, Neumann I, Brennan S, et al. Indirectness. In: The GRADE Book. GRADE Working Group. Last modified 12 May 2026."
    url_or_doi: "https://book.gradepro.org/guideline/indirectness"
    why_included: "Anchors applicability/generalizability/transferability as evidence-versus-target alignment across population, intervention, comparator and outcome, including indirect comparisons."
    limitation: "PICO alignment is necessary but not sufficient for every real-world applicability judgment; domain expertise and decision context remain necessary."

  - source_id: "F0-S08"
    priority: "SUPPORT"
    citation: "Wasserstein RL, Lazar NA. The ASA Statement on p-Values: Context, Process, and Purpose. The American Statistician. 2016;70(2):129-133. doi:10.1080/00031305.2016.1154108."
    url_or_doi: "https://www.amstat.org/asa/files/pdfs/p-valuestatement.pdf"
    why_included: "Direct safeguard against converting p-values into probabilities that hypotheses are true, effect magnitude/importance, or a lone threshold for scientific conclusions."
    limitation: "The statement does not prescribe a single universal replacement inferential system. F0.10 therefore combines it with estimate/CI/threshold and evidence-quality reasoning rather than teaching 'never use p-values'."

  - source_id: "F0-S09"
    priority: "CONTRAST"
    citation: "Benjamini Y, et al. ASA President’s Task Force Statement on Statistical Significance and Replicability. American Statistical Association / IMS; 2021."
    url_or_doi: "https://magazine.amstat.org/blog/2021/08/01/task-force-statement-p-value/"
    why_included: "Contrast source against an oversimplified reaction to p-value misuse. It emphasizes that properly applied p-values/significance tests remain useful while uncertainty, variability, multiplicity and replicability require broader reasoning."
    limitation: "High-level task-force guidance rather than a detailed interval-estimation or evidence-synthesis manual. It is included to preserve balance in statistical communication, not to restore binary thresholding."

claims_to_master:
  - "Simplifying language may reduce jargon; it must not reduce scientific uncertainty."
  - "Before audience-specific drafting, freeze target, direction, magnitude, precision, threshold, certainty, applicability and boundaries/update conditions."
  - "The same invariant core must survive technical, practitioner-facing and lay-facing versions."
  - "p<0.05 is not a truth or importance threshold, and p>0.05 is not proof of no effect."
  - "A point estimate without its uncertainty can mislead, and an interval without a practical threshold may remain decision-ambiguous."
  - "'Did not detect a clear effect' is weaker than 'the compatible effect range excludes a meaningful effect'."
  - "Formal equivalence/non-inferiority is not established by a nonsignificant superiority test."
  - "Certainty concerns confidence in an effect range or threshold classification across a body of evidence for an outcome/question; it is not effect magnitude itself."
  - "High-certainty trivial effects and low-certainty large point estimates are both possible."
  - "Imprecision, bias, inconsistency, indirectness and missing/dissemination evidence are different uncertainty mechanisms and should be named separately."
  - "Direct evidence can still be biased; internally strong evidence can still be indirect for the target."
  - "Conflicting studies should not be synthesized by vote counting."
  - "Avoiding false balance does not justify a mechanical evidence pyramid; source weight depends on the claim being evaluated."
  - "Mechanistic evidence can support plausibility without establishing the magnitude of a chronic performance or health outcome."
  - "An evidence statement and a recommendation statement answer different questions."
  - "Certainty of one outcome does not determine recommendation strength because recommendation processes may also consider benefits/harms, values, resources, feasibility, acceptability, equity and decision context."
  - "Audience translation can change vocabulary, sentence length and statistical density, but cannot silently broaden the population, outcome, time horizon or causal claim."
  - "A lay or practitioner version that sounds more certain than the technical version has language drift."
  - "A useful uncertainty statement specifies what would materially change the conclusion rather than ending with a generic 'more research is needed'."

critical_repairs:
  - "p<0.05 = true/important → report estimate, uncertainty, threshold and context"
  - "p>0.05 = no effect → state what effect range remains compatible"
  - "non-significant = equivalent → require appropriate equivalence/non-inferiority design and margin"
  - "high certainty = large effect → separate confidence from magnitude"
  - "low certainty = no effect → separate uncertainty from effect direction/magnitude"
  - "direct evidence = unbiased → audit result-level bias separately from directness"
  - "four papers split 2–2 → weight evidence by claim fit and inferential contribution rather than vote counting"
  - "RCT always outranks everything → ask which design/result is informative for the target claim and what bias/directness problems remain"
  - "mechanistic biomarker moved → chronic performance benefit proven → preserve outcome/time-horizon boundary"
  - "evidence statement = recommendation → identify the additional decision criteria required"
  - "technical says 'may', lay says 'works' → repair audience drift"
  - "technical population becomes 'everyone' in lay version → restore target scope"
  - "CI omitted to make the message simpler → translate uncertainty rather than deleting it"
  - "more studies are needed → specify what new result, population, precision or threshold would change the conclusion"

notebooklm_tasks:
  - "Act as a calibration coach. For every learner synthesis, first require the eight-field invariant core before commenting on wording."
  - "Generate fresh synthetic estimates and ask the learner to classify whether the evidence merely failed to detect an effect, excludes a prespecified meaningful threshold, or comes from a formal equivalence/non-inferiority design."
  - "Generate paired statements with identical p-values but different estimates/CIs/thresholds and require different practical interpretations."
  - "Generate a high-certainty tiny effect and a low-certainty large point estimate; require the learner to separate magnitude from certainty."
  - "Generate one example each of imprecision, bias, inconsistency, indirectness and missing/dissemination uncertainty and require mechanism-specific wording."
  - "Generate a direct-but-biased study and an internally strong-but-indirect study; require two-axis appraisal."
  - "Generate four conflicting evidence sources with unequal fit/design/precision. Require a weighted synthesis and explicitly forbid paper counting."
  - "Generate a scenario where a small RCT is high risk and a carefully designed observational study answers a different claim better; require the learner to reject a mechanical evidence pyramid."
  - "Generate a mechanistic biomarker study plus chronic performance trials and require the learner to state what the mechanistic study does and does not add."
  - "Give one evidence statement and ask which additional decision inputs would be needed before issuing a recommendation."
  - "Require three translations—technical, practitioner-facing and lay-facing—and then compare them field-by-field for invariant-core preservation."
  - "Introduce deliberate drift into one simplified version (broader population, missing CI, stronger causal verb or deleted uncertainty) and require repair."
  - "Ask the learner to shorten a technical synthesis by 50% without deleting population, magnitude, uncertainty, certainty, applicability or inferential boundaries."
  - "Require a one-sentence update condition for each synthetic synthesis: what result or assumption change would materially alter the conclusion."
  - "At the end, require the canonical workflow and all eight invariant-core fields from memory, then produce a fresh three-audience synthesis without source consultation and audit it afterward."

fresh_guided_examples:
  - id: "G1"
    target: "trained adults, fictional intervention R versus placebo, 8-week standardized performance test"
    effect: "MD -9 s; 95% CI -27 to +9 s; lower is better"
    threshold: "-20 s"
    certainty_context: "moderate certainty, limited mainly by imprecision"
    teaching_goal: "Show that the estimate favors R but the compatible range crosses the null and the meaningful-benefit threshold; do not convert this into either 'works' or 'does not work'."
  - id: "G2"
    target: "same fictional target"
    effect: "MD -3 s; 95% CI -11 to +5 s"
    threshold: "-20 s"
    certainty_context: "high certainty for this outcome/body"
    teaching_goal: "Show high confidence that a large/meaningful benefit of at least 20 s is unlikely under the stated threshold while small effects remain possible; high certainty does not imply a large benefit."
  - id: "G3"
    target: "fictional chronic performance claim"
    evidence: "direct meta-analysis MD +0.3 [0.0,+0.6]; large direct RCT +0.2 [-0.1,+0.5]; observational cohort +1.4 [+1.0,+1.8] with residual confounding; acute mechanistic biomarker +40%"
    threshold: "+0.8"
    teaching_goal: "Train weighted synthesis without 2-versus-2 vote counting and without allowing the mechanistic result to establish chronic performance magnitude."

initial_corpus_exclusions:
  - "foundations/F0-scientific-literacy/F0.10-synthesis-communication-uncertainty/EXERCISES.md"
  - "foundations/F0-scientific-literacy/F0.10-synthesis-communication-uncertainty/ANSWER_KEY.md"
  - "foundations/F0-scientific-literacy/F0.10-synthesis-communication-uncertainty/QA_REPORT.md"
  - "foundations/F0-scientific-literacy/SOURCE_INDEX.md"
  - "foundations/F0-scientific-literacy/F0.4-descriptive-statistics/ENTRY_DIAGNOSTIC.md"

mastery_state_policy:
  - "Package production changes no learner state."
  - "F0.1–F0.10 remain pending/unvalidated until observed learning/performance."
  - "F0.4 quantitative diagnostic remains UNOBSERVED."
  - "NotebookLM practice is study support and does not itself authorize MASTERED."
  - "The cumulative F0 exit assessment remains deferred until this package is complete."
```

---

## External source/link verification — 2026-09-10

Every external source included in manifest v1 was rechecked before package creation.

### F0-S08 — ASA p-value statement

- The official ASA statement remains accessible.
- Its six core principles remain unchanged for this instructional use.
- It still states that p-values do not measure the probability that a hypothesis is true, should not alone determine scientific conclusions, and do not measure effect size/importance.
- F0.10 uses it as a safeguard against threshold-driven language, not as a prohibition on p-values.

### F0-S09 — ASA Task Force statement

- The ASA-hosted 2021 task-force statement remains accessible.
- It explicitly preserves a role for properly applied/interpreted p-values and significance tests while emphasizing uncertainty, variability, multiplicity and replicability.
- This makes it an appropriate `CONTRAST` source against the simplistic lesson that p-values are either all-powerful or useless.

### F0-S18 — GRADE overview

- The living GRADE Book overview remains available and shows `Last modified: 12 May 2026`.
- It retains four certainty categories and explicitly distinguishes certainty of evidence from recommendation processes.
- F0.10 uses this boundary when separating evidence statements from recommendations.

### F0-S19 — GRADE intervention-certainty principles

- The living chapter remains available and shows `Last modified: 21 Aug 2025`.
- It defines certainty as confidence that the true effect lies within a specific range or above/below a defined threshold of interest.
- It explicitly applies certainty at outcome/body level rather than per individual study.
- This source anchors the F0.10 range/threshold communication logic.

### F0-S20 — GRADE indirectness

- The living chapter remains available and shows `Last modified: 12 May 2026`.
- It continues to define indirectness through applicability/generalizability/transferability concerns and alignment between evidence and target PICO, plus indirect comparisons.
- F0.10 uses this source to prevent silent scope expansion during audience translation.

No source-version change required revision of the approved F0.10 lesson. No new external source ID is required for this package.

---

## Copyright/public-repository controls

- Only project-authored Markdown, citations and links are persisted in GitHub.
- No third-party PDF, article full text, GRADE chapter text or ASA document is copied into the repository.
- The manifest identifies external resources so the learner can add/access them through NotebookLM-supported source mechanisms.
- The package contains no personal or private health information.
- All exercise examples in the package are fictional and educational, not nutrition prescriptions.

---

## Initial NotebookLM corpus — exact six-source set

Add **exactly these six sources** for the first pass:

1. `F0-R10` — canonical F0.10 lesson — `CORE`;
2. `F0-S19` — GRADE intervention-certainty principles — `CORE`;
3. `F0-S18` — GRADE overview — `SUPPORT`;
4. `F0-S20` — GRADE indirectness — `SUPPORT`;
5. `F0-S08` — ASA p-value statement — `SUPPORT`;
6. `F0-S09` — ASA Task Force statement — `CONTRAST`.

Do not add the F0.10 exercises or answer key during first-pass study.
