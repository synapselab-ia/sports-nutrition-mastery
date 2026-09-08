# F0.3 — QA report

**Unit:** `F0.3 — Bias, confounding, causal reasoning and validity`

**Reviewed:** 2026-09-08

**Production decision:** `APPROVED`

This report records production QA only. It does **not** record learner performance and does not change any mastery state.

---

## 1. Scope gate

### Required by COURSE_MAP / NEXT_ACTION

- systematic versus random error — covered;
- confounding as causal/common-cause structure — covered;
- residual confounding — covered;
- selection mechanisms — covered;
- information/measurement bias — covered;
- exposure/outcome/confounder measurement error — covered;
- misclassification, including differential versus non-differential intuition — covered;
- attrition/missingness as causal/selection mechanisms — covered;
- reverse causation — covered;
- counterfactual intuition — covered as P1 support without formal potential-outcome derivations;
- confounder versus mediator versus collider — covered;
- directed acyclic graphs (DAGs) — covered as assumption/communication tools, not proof generators;
- invalid adjustment strategies — covered, including overadjustment for mediators and conditioning on colliders/post-exposure selection;
- target-trial thinking — covered as a causal-design benchmark;
- internal validity versus external validity/generalizability/transportability/applicability — covered at introductory level;
- randomization as protection against baseline confounding without guarantee of total validity — covered;
- explicit separation of what can be prevented/mitigated versus what cannot be recovered from inadequate/unmeasured data — covered;
- sports-nutrition transfer scenarios — covered with hypothetical supplement, training, energy-intake and performance examples;
- applied response template requiring target question, causal structure, distortion mechanism, repairability and calibrated conclusion — mandatory in `EXERCISES.md` Part C and integrated again in Part E;
- simplified DAG performance task with invalid adjustment strategies — covered in Parts B and E.

### Intentionally deferred

The unit does **not** teach in full:

- RoB 2 algorithms/domains/signalling questions — F0.8;
- ROBINS-I/ROBINS-I V2 formal assessment — F0.8;
- ROBINS-E — later risk-of-bias work when relevant;
- GRADE certainty framework — F0.8;
- quantitative bias analysis — advanced/deeper methods;
- inverse-probability weighting mathematics — later quantitative/causal methods;
- multiple imputation mathematics and formal missingness taxonomies — later quantitative methods;
- g-methods/time-varying confounding — advanced causal inference;
- formal mediation analysis — advanced causal inference;
- instrumental variables/propensity-score methods — advanced causal inference;
- effect-estimate uncertainty, confidence intervals, p-values and power — F0.4–F0.6;
- systematic review/meta-analysis — F0.7.

This keeps F0.3 focused on structural causal reasoning rather than prematurely collapsing F0.4–F0.8 or advanced epidemiology into one lesson.

---

## 2. Source recheck — PASS

Authoritative/current resources were externally rechecked on 2026-09-08 before production.

### `F0-S16` — Hernán & Robins, *Causal Inference: What If*

- the authors' official page remains active and explicitly points users to the latest free online version;
- retained as the deeper foundation for counterfactual reasoning, exchangeability, confounding, selection and causal identification;
- used as teacher/method backbone rather than assigning formal later chapters to an entry learner.

### `F0-S17` — target-trial framework

- the 2025 *Annals of Internal Medicine* article was rechecked through PubMed/PMC;
- retained two-step logic: specify the hypothetical randomized target trial, then attempt emulation using observational data;
- the lesson preserves the source's central limitation: target-trial emulation does not create randomization and cannot repair unavailable/unmeasured information.

### `F0-S11` — Catalogue of Bias

- current site was rechecked and remains actively maintained in 2026;
- current entries relevant to F0.3 include confounding, collider bias, selection bias, attrition bias, information bias and misclassification bias;
- used for mechanism/examples, never as a memorization checklist or causal-proof authority.

### `F0-S07` — riskofbias.info

- current RoB 2 resources remain available for randomized trials;
- the site now exposes a revised draft of `ROBINS-I V2` announced 30 November 2025, including reorganized/expanded treatment of classification, selection and missing-data domains;
- F0.3 does **not** teach or score the formal tool; this update is relevant only as confirmation that contemporary operational risk-of-bias frameworks continue to separate causal/bias mechanisms rather than treating “study quality” as a single number.

### `F0-S26` — Feeney, Hartwig & Davies 2025 DAG guide

- added because it fills a direct instructional gap not covered as accessibly by the existing advanced causal textbook;
- *BMJ* 2025 guide explicitly treats DAGs as representations of causal assumptions and covers confounders, mediators, colliders, selection pathways and covariate-selection consequences;
- its own framing emphasizes subject-matter knowledge and transparent assumptions, consistent with the lesson's warning that a DAG is not empirical proof.

No additional source was added solely for decoration. No separate missing-data source was added because the conceptual F0.3 claims are adequately supported by the existing bias catalogue, causal foundation and current risk-of-bias hub; formal missing-data methods are deliberately outside this unit.

---

## 3. CONTENT_QA — PASS

Checked:

- bias is defined technically as systematic distortion rather than researcher misconduct;
- random error and systematic bias are separated without prematurely teaching standard-error mathematics;
- sample-size increase is not presented as a cure for systematic bias;
- counterfactual reasoning is introduced conceptually without hidden formal-math prerequisites;
- exchangeability is translated into operational causal comparability rather than used as unexplained jargon;
- confounding is taught as causal structure/common-cause reasoning, not merely “associated with exposure and outcome”;
- residual confounding includes unmeasured, poorly measured, coarsened/proxy and structurally misspecified confounding;
- mediator adjustment is explicitly linked to the estimand; total-effect versus direct-effect distinction is preserved;
- collider bias is explained through conditioning on a common effect, including selection as a possible collider mechanism;
- DAG arrows and missing arrows are explicitly described as assumptions;
- DAGs are not represented as proof generators or automated truth discovery;
- covariate adjustment is not chosen by p-value, baseline imbalance or “adjust everything” logic;
- selection is separated into internal causal-selection threats versus external representativeness/applicability concerns;
- nonrepresentative samples are not automatically mislabeled as internally biased;
- information bias, measurement error and misclassification are separated from confounding while allowing measurement error to create residual confounding;
- non-differential misclassification is **not** falsely claimed to always bias toward the null;
- missingness/attrition are taught as mechanisms, not percentages;
- equal loss percentages are not treated as proof of unbiased follow-up;
- complete-case analysis is not treated as neutral by default;
- reverse causation is tied to temporal ordering and F0.2 design architecture;
- randomization is correctly limited to baseline assignment/comparability benefits in expectation;
- post-randomization selection, missingness, measurement and adherence problems remain explicit;
- target-trial thinking is not represented as retroactive randomization;
- internal validity and external validity/applicability are kept distinct;
- a repairability table explicitly distinguishes design/measurement/analysis mitigation from missing information that cannot be guaranteed recoverable.

No material internal contradiction identified.

---

## 4. EVIDENCE_QA — PASS

Evidence safeguards:

- methodological sources are matched to methodological claims;
- no observational association is promoted to causal effect without explicit assumptions;
- no amount of multivariable adjustment is treated as proof that confounding is eliminated;
- no causal DAG is treated as evidence that its arrows are true;
- target-trial emulation limitations are preserved;
- current risk-of-bias resources are used only to confirm domain structure and are not taught prematurely as scoring systems;
- the current `ROBINS-I V2` draft state is identified as a revised draft rather than silently represented as a finalized universal standard;
- formal GRADE certainty language is deferred to F0.8;
- no sports-nutrition hypothetical example is converted into a practical recommendation;
- no mechanism is treated as evidence of real-world benefit;
- missing-data correction methods are described as assumption-dependent rather than guaranteed recovery procedures.

### Anti-cherry-picking check

F0.3 is a methodological unit rather than a contested treatment-effect unit. The main relevant tension is whether statistical adjustment automatically improves causal validity. The lesson deliberately includes the contrary cases where adjustment can **increase** bias (mediator/collider/post-exposure selection), preventing a one-directional “more adjustment = better” narrative.

---

## 5. PEDAGOGICAL_QA — PASS

### Prerequisites

P2 dependencies are respected:

- F0.1 supplies question/estimand/operationalization;
- F0.2 supplies design, temporal ordering, randomization and observational architecture.

Local P0/P1 support includes:

- counterfactual intuition;
- exchangeability in plain language;
- simple DAG construction/interpretation;
- confounder/mediator/collider;
- selection node;
- measurement and missingness mechanisms;
- validity vocabulary.

No calculus, regression algebra or formal probability derivation is required to understand the unit.

### Progression

The lesson follows:

`question/estimand → counterfactual intuition → random vs systematic error → confounding → DAGs → confounder/mediator/collider → adjustment mistakes → selection → measurement → missingness → reverse causation → randomization limits → target trial → validity/applicability → repairability → integrated worked examples → causal audit algorithm`

### Autossuficiência

A capable learner who has F0.1/F0.2 does not need an external causal-inference textbook to perform the required F0.3 tasks. External sources provide traceability and deeper formal treatment rather than outsourcing essential definitions or mechanisms.

### Anti-memorization design

The exercises repeatedly require a five-part answer:

1. target causal question;
2. causal structure;
3. distortion mechanism;
4. repairability;
5. calibrated conclusion.

This makes named-bias recognition insufficient for passing.

---

## 6. MASTERY_QA — PASS

`EXERCISES.md` tests:

- `K1` — define random/systematic error, confounder, mediator, collider, validity concepts;
- `K3` — compare causal roles and internal versus external validity;
- `K4` — interpret observed association relative to causal structure;
- `K5` — predict what happens after conditioning on mediators/colliders or selecting completers;
- `K6` — choose adjustment/design responses for concrete scenarios;
- `K7` — integrate F0.1 estimand + F0.2 design + F0.3 causal-bias reasoning;
- `K8` — state what assumptions remain and what data limitations prevent confident causal claims.

The final sports-nutrition case requires all of the following in one response:

- estimand reconstruction;
- verbal/graphical causal model;
- confounder + mediator + selection node;
- invalid adjustment decisions;
- repairability distinction;
- uncertainty-calibrated conclusion.

Critical-fail conditions directly target structural misconceptions that would make later risk-of-bias/certainty appraisal unsafe.

Production approval alone does not mark `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED`.

---

## 7. Public-repository/privacy QA — PASS

- no personal/health-identifying learner data;
- no real individual case history;
- no copyrighted guideline/tool documents copied into repository;
- risk-of-bias tools are link/citation referenced only;
- examples are hypothetical research scenarios rather than individualized nutrition prescriptions;
- no professional credential or clinical-practice claim is implied.

---

## 8. Final gate

> Can a capable learner who has completed F0.1/F0.2 explain how confounding, selection, measurement, missingness, reverse causation and invalid adjustment can move an estimate away from its causal target; use a simple DAG without treating it as proof; distinguish what randomization solves from what remains; and state when inadequate data make a problem unrecoverable?

**Decision:** yes — `APPROVED`.

NotebookLM packaging is not part of `F0-A06`; it should be produced only under the subsequent canonical action.