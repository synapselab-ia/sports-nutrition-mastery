# F0.3 — Practical NotebookLM Study Guide

**Package version:** `1`
**Module:** `F0.3 — Bias, confounding, causal reasoning and validity`
**Current learner state:** `UNSEEN`

This guide defines exactly how to build and use the approved NotebookLM corpus for F0.3. Completing setup, reading sources or having NotebookLM explain a concept does **not** change learner state. Progression requires observed performance under the mastery protocol.

## 1. Create the notebook

Create one NotebookLM notebook named:

`Sports Nutrition Mastery — F0.3 Causal Validity`

Keep F0.1 and F0.2 notebooks separate. Their concepts are prerequisites, but F0.3 needs a compact corpus focused specifically on causal structure and systematic error.

## 2. Add exactly six initial sources

Use only the following sources on the first pass.

### Source 1 — canonical F0.3 lesson — CORE

Repository file:

`foundations/F0-scientific-literacy/F0.3-bias-confounding-causal-validity/LESSON.md`

Preferred NotebookLM URL:

`https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.3-bias-confounding-causal-validity/LESSON.md`

Use it as the primary instructional spine for:

- target causal question and estimand;
- counterfactual/exchangeability intuition;
- random versus systematic error;
- confounding/residual confounding;
- simple DAG reasoning;
- confounder/mediator/collider roles;
- invalid adjustment;
- selection;
- measurement/information bias and misclassification;
- missingness/attrition;
- reverse causation;
- randomization limits;
- target-trial thinking;
- internal versus external validity/applicability;
- repairability versus unavailable information;
- calibrated causal conclusions.

If NotebookLM cannot ingest the raw Markdown URL, download/upload the exact canonical Markdown file. Do not replace it with an AI-generated summary.

### Source 2 — Causal Inference: What If — CORE

Open:

`https://miguelhernan.org/whatifbook`

Use the **latest version linked by the authors**. At package verification on 2026-09-09, the current linked PDF was dated `19aug26`.

For F0.3, use only introductory material needed for:

- counterfactual causal effects;
- exchangeability/comparability;
- why randomized assignment helps identify causal effects;
- why observational causal inference requires additional assumptions;
- confounding/selection intuition.

Do not attempt to study the entire advanced book in this unit. Later longitudinal causal-method chapters exceed F0.3 scope.

Practical NotebookLM setup:

1. open the authors' page;
2. click `Get the latest version of the book here`;
3. download the current PDF for personal NotebookLM study;
4. upload that PDF to NotebookLM;
5. do **not** commit the third-party PDF to this public repository.

### Source 3 — BMJ directed acyclic graph guide — CORE

Add as website:

`https://www.bmj.com/content/388/bmj-2023-078226`

Use it for:

- defining the target exposure/treatment and outcome before drawing a DAG;
- encoding assumed causal directions;
- confounders;
- mediators;
- colliders;
- selection processes;
- identifying variables that should and should not be adjusted for;
- explaining assumptions transparently.

Critical rule:

> A DAG represents an assumed causal structure. It helps reason about consequences of those assumptions; it does not prove the arrows are true.

### Source 4 — Catalogue of Bias — SUPPORT

Add as website:

`https://catalogofbias.org/biases/`

Use it selectively for concrete examples of:

- confounding;
- collider bias;
- selection bias;
- attrition bias;
- information/measurement bias;
- misclassification and related mechanisms.

Do not ask NotebookLM to memorize the catalogue alphabetically. For every bias name, force this translation:

`what process differs? → why does it differ? → what path/measurement/selection is created? → how could the estimate be distorted?`

### Source 5 — current ROBINS-I V2 page — SUPPORT / boundary source

Add as website:

`https://www.riskofbias.info/welcome/robins-i-v2`

As verified on 2026-09-09, the official page states that the revised V2 was posted on **20 November 2025** and is still a **draft version subject to change**.

Use this page only to observe that operational bias assessment separates domains such as:

- confounding;
- classification of intervention;
- selection into the study;
- missing data;
- measurement of outcome;
- selection of the reported result.

Critical scope rule:

> Do not download/use the full ROBINS-I V2 tool for formal grading in F0.3. Do not simulate signaling-question algorithms or assign an overall ROBINS-I judgment. Formal risk-of-bias tool use belongs to F0.8.

### Source 6 — target-trial framework — CONTRAST

Add the free full text:

`https://pmc.ncbi.nlm.nih.gov/articles/PMC11936718/`

Use it for:

- specifying a hypothetical randomized target trial;
- eligibility;
- intervention/treatment strategies;
- assignment concept;
- `time zero`;
- follow-up;
- outcomes;
- causal contrast/estimand;
- separating design-induced bias from data limitations;
- understanding why observational emulation does not create randomization.

Critical rule:

> Better target-trial emulation can prevent some self-inflicted design bias. It cannot recover an unmeasured confounder, create unavailable time-varying measurements or retroactively randomize treatment assignment.

## 3. Do NOT add these yet

Keep the following outside the initial NotebookLM corpus:

- F0.3 `ANSWER_KEY.md` — answer leakage;
- F0.3 `EXERCISES.md` — independent assessment must remain independent;
- F0.3 production `QA_REPORT.md` — production metadata;
- full `SOURCE_INDEX.md` — registry noise;
- RoB 2 full documents;
- ROBINS-I V2 PDF/template — formal tool mechanics belong to F0.8 and the current V2 remains draft;
- GRADE Book certainty chapters — formal certainty belongs later;
- F0.4–F0.6 statistical references — random variation, CI, p-values, effect sizes, power and multiplicity are not the target of F0.3;
- extra DAG tutorials — one current practical DAG guide plus the canonical lesson is enough initially;
- dozens of individual Catalogue of Bias pages — select only examples needed to understand mechanisms.

## 4. Universal F0.3 reasoning template

Before the detailed passes, memorize this output structure:

1. `Target causal question/estimand:`
2. `Causal structure:`
3. `Distortion mechanism:`
4. `Adjustment/conditioning:`
5. `Repairability/data limitation:`
6. `Calibrated conclusion:`

Every unfamiliar scenario in F0.3 should eventually be answerable in this format.

The key shift from F0.2 is:

`what can this design answer?`

becomes:

`what would have to be true for this observed estimate to represent the target causal effect, and how could those conditions fail?`

## 5. Study sequence

Follow the passes in order. Do not begin by asking NotebookLM to summarize all six sources.

### Pass 1 — random error versus systematic error

Study the canonical lesson section on error.

Ask NotebookLM:

> Using only the canonical F0.3 lesson, teach random error versus systematic error with three sports-science examples. Do not teach confidence intervals, p-values or power yet. For every example, state whether increasing sample size directly repairs the mechanism.

Then answer without help:

1. Why can a study be extremely precise and still causally wrong?
2. Why does large N not reconstruct an unmeasured confounder?
3. Why does repeated use of a systematically miscalibrated measurement not automatically remove the systematic component?
4. Which later modules will quantify random uncertainty?

Create one original analogy different from the lesson's scale/balance analogy.

### Pass 2 — counterfactuals and exchangeability

Use the canonical lesson plus selected introductory `What If` material.

Ask:

> Explain the counterfactual problem for strategy A versus strategy B without advanced notation. Then explain exchangeability as a causal comparability condition. Contrast randomized assignment with observational comparison without claiming that covariate adjustment automatically makes them equivalent.

Then, without notes, write:

- the outcome observed under A;
- the unobserved alternative under B for the same person/time;
- why comparing different people requires comparability assumptions;
- what randomization changes about treatment assignment;
- what observational analysis must assume/measure instead.

Critical trap:

> `adjusted for many covariates` is not synonymous with `exchangeability established`.

### Pass 3 — confounding and residual confounding

Ask NotebookLM:

> Generate five observational nutrition/performance associations. For each, wait for me to propose a plausible common cause before grading. Require a text DAG and an explanation of how the backdoor/non-causal path generates association.

For each scenario, use:

`C → A`

`C → Y`

`A → Y` (target causal path, if assumed)

Then explain whether controlling C is conceptually appropriate for the specified target effect.

Next ask:

> Give me four studies that claim to have 'adjusted for confounding'. Make each one leave a different residual-confounding problem: unmeasured confounder, noisy measurement, coarse categorization/proxy, or structurally wrong adjustment model. Present one at a time.

You must distinguish:

- `measured confounding addressed under assumptions`;
- `residual confounding remains plausible`;
- `unmeasured confounding cannot be guaranteed repaired by sample size`.

### Pass 4 — confounder versus mediator versus collider

Use the BMJ DAG guide heavily here.

Ask NotebookLM:

> Give me three variables X, M and C around exposure A and outcome Y. Present three different plausible DAGs where one variable changes role across questions. Do not label confounder, mediator or collider until I classify it.

You must be able to recognize:

#### Confounder pattern

`C → A`

`C → Y`

#### Mediator pattern

`A → M → Y`

#### Collider pattern

`A → K ← U → Y`

or another common-effect structure.

For each graph answer:

1. what is the target estimand — total effect or something else?
2. which path should remain open?
3. which non-causal path should be blocked?
4. what happens if you condition on the mediator?
5. what happens if you condition on the collider?

Critical rule:

> Predictive value is not a sufficient reason to adjust for a variable.

### Pass 5 — DAG construction and assumption challenge

Ask:

> Give me a causal question involving supplement use and performance. Wait for me to draw a DAG. Then challenge exactly one arrow or missing node and ask me to redraw the graph and reconsider the adjustment set.

Your graph should contain at least:

- exposure/intervention;
- outcome;
- one baseline confounder;
- one possible mediator;
- one possible selection/collider variable;
- one unmeasured cause.

After drawing, state:

- which arrows are subject-matter assumptions;
- which nodes are measured;
- which nodes are unmeasured;
- which covariates you would adjust for and why;
- which variable you would deliberately **not** adjust for and why.

Then ask NotebookLM to critique only after your answer.

### Pass 6 — selection and collider bias

Use the canonical lesson, BMJ DAG guide and Catalogue of Bias.

Ask:

> Generate six selection scenarios across recruitment, eligibility restriction, loss to follow-up, complete-case analysis and analytical exclusion. At least three scenarios must involve conditioning on a common effect/collider. Present one at a time.

For each scenario answer:

1. what determines selection/inclusion?
2. is selection before or after exposure/intervention?
3. what causes selection?
4. what causes the outcome?
5. does conditioning on selected people open a non-causal path?
6. can design prevent it?
7. can existing data repair it?
8. what cannot be known from the given information?

Do not equate:

- non-representative sample = automatically internally biased;
- representative sample = automatically internally valid.

### Pass 7 — measurement, information bias and misclassification

Ask NotebookLM:

> Create five measurement scenarios involving exposure, outcome or confounder measurement. Mix calibration error, recall differences, knowledge of intervention, coarse categorization and a noisy proxy. Do not tell me whether the error is differential.

For each, identify:

- what is being measured;
- what the target construct is;
- whether error can differ by exposure/outcome status;
- what causal comparison could be distorted;
- whether repeated measurement/calibration could help;
- what information is permanently absent.

Then ask:

> Challenge the statement 'non-differential misclassification always biases toward the null'. Give examples showing why direction depends on structure and effect measure rather than a universal slogan.

You do not need advanced measurement-error mathematics in F0.3. You do need to stop using universal directional rules without justification.

### Pass 8 — missingness and attrition as causal processes

Ask:

> Give me four studies with exactly 20% missing outcome data. Make the causal mechanism of missingness different in each case. Present one at a time and require me to explain why the same percentage can imply different bias risks.

For each use:

`Who is missing? → why missing? → does missingness depend on treatment/exposure? → does it depend on outcome/prognosis or their causes? → what does complete-case selection condition on?`

Then compare:

- equal 20% attrition in both arms with outcome-dependent loss;
- unequal 10% versus 25% loss for reasons unrelated to outcome under strong assumptions;
- missingness related to post-treatment adverse effects;
- missingness driven by an unmeasured prognostic factor.

Critical rule:

> Percentage missing is descriptive; the bias question is causal.

### Pass 9 — reverse causation and temporal structure

Connect back to F0.2.

Ask:

> Generate four associations where reverse causation is plausible. Include one cross-sectional, one retrospective-measurement and one longitudinal scenario where the outcome process may already have started before exposure measurement.

For each:

- identify temporal ambiguity;
- describe the reverse arrow;
- state what additional design/measurement could strengthen directionality;
- avoid claiming that temporal ordering alone solves all confounding.

### Pass 10 — randomization: what it buys and what survives

Use the lesson plus `What If`.

Ask:

> Compare the causal-validity pathway of a well-randomized trial with a non-randomized observational intervention comparison. Separate baseline assignment/confounding from post-assignment adherence, selection, missingness, outcome measurement and reporting/analysis.

Create a two-column table from memory:

| Stage | What randomization helps | What can still go wrong |
|---|---|---|
| baseline assignment | ... | ... |
| adherence/deviation | ... | ... |
| follow-up/missingness | ... | ... |
| outcome measurement | ... | ... |
| analysis/reporting | ... | ... |
| applicability | ... | ... |

The required conclusion is not `RCTs are perfect` or `randomization does nothing`.

It is:

> randomization addresses a powerful causal-identification problem at assignment, while other bias mechanisms require their own protections.

### Pass 11 — target trial: design bias versus data limitation

Read the target-trial article sections on why/when the framework helps.

Ask:

> Give me an observational causal intervention question. Require me to specify eligibility, strategies, assignment, time zero, follow-up, outcome and causal contrast before I see any data. Then give me a dataset description with deliberate limitations.

For the scenario, separate into four boxes:

1. `Design bias prevented by target-trial alignment`;
2. `Measured limitation potentially addressable under assumptions`;
3. `Unmeasured/unavailable information not guaranteed recoverable`;
4. `Residual causal assumption after analysis`.

Critical trap:

> target-trial emulation is a design framework, not a statistical spell and not retroactive randomization.

### Pass 12 — internal versus external validity

Ask NotebookLM:

> Give me four study descriptions with different combinations of internal validity and applicability. Include: narrow but internally strong study; broad but internally biased study; internally strong trial with indirect intervention/dose for the target question; and observational study with strong real-world representativeness but unresolved confounding.

For each, write separately:

- `Internal-validity conclusion:`
- `Applicability/transportability conclusion:`

Do not use one to substitute for the other.

### Pass 13 — full mixed causal-validity examination

Use this prompt exactly:

> Act as an examiner for F0.3. Generate unfamiliar causal-validity scenarios one at a time in nutrition/exercise research. Randomly vary confounding, residual confounding, mediator adjustment, collider conditioning, selection, measurement bias, misclassification, attrition/missingness, reverse causation, randomized versus observational assignment, target-trial design bias and applicability. Do not name the bias in the scenario. Wait for my answer. Require exactly these six fields before grading: Target causal question/estimand; Causal structure; Distortion mechanism; Adjustment/conditioning; Repairability/data limitation; Calibrated conclusion. Require a text DAG whenever confounder/mediator/collider/selection structure is relevant. Grade only with citations to the approved six-source corpus. Do not perform formal RoB 2/ROBINS-I/GRADE scoring.

Continue until you can explain mechanisms without relying on trigger words.

## 6. Source-comparison tasks

These tasks are required because the corpus contains different source types.

### Task A — canonical lesson versus What If

Ask:

> Which causal concepts does the project lesson simplify for F0.3, and how does What If provide the deeper foundation? Identify at least one advanced concept from the book that should remain outside F0.3.

Expected distinction:

- lesson = pedagogical F0.3 translation;
- What If = deep causal-inference foundation;
- selected use, not whole-book mastery.

### Task B — BMJ DAG guide versus statistical covariate selection

Ask:

> Why does the BMJ DAG guide recommend defining the causal question and causal assumptions before choosing covariates? Contrast that with selecting every variable associated with exposure or outcome.

Required conclusion:

- causal role comes from assumed structure and estimand;
- association/prediction alone does not determine adjustment.

### Task C — Catalogue of Bias versus causal mechanism

Ask:

> Pick four entries from the Catalogue of Bias that are relevant to F0.3. For each, strip away the label and explain the exact selection/measurement/causal process that distorts the estimate.

If you can name the bias but cannot explain the mechanism, the task is incomplete.

### Task D — ROBINS-I V2 page versus F0.3 scope

Ask:

> What does the current ROBINS-I V2 webpage reveal about how non-randomized intervention bias is divided into domains? Why are we not applying the tool formally in F0.3, and what is its current version status?

Required points:

- current November 2025 V2 is still draft;
- domain separation is informative;
- formal algorithm/judgment belongs to F0.8;
- risk-of-bias tool is not a total quality score.

### Task E — target-trial paper versus unmeasured confounding

Ask:

> Give two examples of bias that target-trial alignment can prevent through better design specification and two examples of data limitations it cannot guarantee to repair. Explain why the distinction matters.

The target-trial article explicitly separates preventable design bias from data limitations such as unmeasured confounding.

## 7. Required integrated evidence-critique task

Use the exact hypothetical case from `MANIFEST.md`:

> Among resistance-trained adults beginning a 12-week training block, does starting nutrition strategy A rather than strategy B improve a prespecified performance outcome at week 12?

Dataset includes:

- baseline age;
- sex;
- baseline performance;
- training volume;
- prior supplement use;
- self-selected A/B strategy;
- week-12 performance;
- follow-up status;

Not measured:

- sleep duration;
- coaching quality.

Before NotebookLM critiques you, produce all 12 outputs required in the manifest evidence-critique task.

The decisive question is not whether you listed enough covariates. It is whether you can explain:

- why each variable has its assumed role;
- which backdoor paths are addressed;
- what selection is introduced by follow-up/complete-case analysis;
- what remains unmeasured;
- what target-trial specification fixes at design level;
- what the data still cannot identify without assumptions.

## 8. Independent assessment outside NotebookLM

After completing the study sequence:

1. open `foundations/F0-scientific-literacy/F0.3-bias-confounding-causal-validity/EXERCISES.md`;
2. answer the entire assessment **without NotebookLM and without `ANSWER_KEY.md`**;
3. draw/text-describe all requested causal structures independently;
4. only after the first attempt, use `ANSWER_KEY.md` or submit your answers to ChatGPT for correction;
5. apply the local gate: `>=80/100` plus no critical fail can support progression evidence;
6. this does not automatically mean `MASTERED`; later cumulative retesting is required.

The package itself leaves the learner state at `UNSEEN`.

## 9. F0.3 critical-fail patterns to prevent

Treat these as structural failures even if terminology recall is otherwise strong:

- claiming that a large sample eliminates systematic bias;
- calling any variable associated with exposure and outcome a confounder without causal reasoning;
- adjusting for every measured variable by default;
- conditioning on a mediator while still claiming to estimate the unmodified total effect;
- conditioning on a collider/selection variable without recognizing that a non-causal path can open;
- treating a DAG as empirical proof of its arrows;
- claiming measured-covariate adjustment guarantees no residual/unmeasured confounding;
- inferring bias from missing percentage alone without asking why observations are missing;
- treating complete-case analysis as neutral by default;
- assuming non-differential misclassification universally biases toward the null;
- treating temporal ordering as sufficient proof of causality;
- treating randomization as protection against every later bias mechanism;
- treating target-trial emulation as actual randomization;
- using ROBINS-I V2 formally in F0.3 or calling the current V2 draft a finalized standard;
- conflating internal validity with generalizability/applicability.

## 10. What to send back to ChatGPT after study

For honest learning-state updates, provide one of:

- completed F0.3 `EXERCISES.md` answers;
- or confirmation that the full study sequence was completed **plus** answers to a fresh F0.3 assessment administered in chat.

Statements such as `li tudo`, `entendi`, `o NotebookLM disse que acertei` or source-ingestion completion are not sufficient to mark `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED`.

## 11. When NotebookLM disagrees with GitHub

Use this order:

1. inspect the exact approved external source cited by NotebookLM;
2. inspect the canonical F0.3 lesson and manifest;
3. determine whether the disagreement is caused by source version, different causal assumptions, different estimand or repository error;
4. if the DAG differs, identify which arrow/assumption changed before calling one answer wrong;
5. if a living source changed materially, research and update GitHub;
6. do not silently promote NotebookLM output to canonical state.

For `ROBINS-I V2`, always verify the official page before treating a future version as final/current because the verified November 2025 revision is explicitly draft.

## 12. Package completion criterion

The F0.3 notebook is correctly configured when:

- exactly six approved initial sources are loaded;
- `ANSWER_KEY.md` and `EXERCISES.md` are absent from the study corpus;
- the learner can distinguish random from systematic error without using later inferential-statistics shortcuts;
- every causal appraisal begins with a target question/estimand;
- confounder/mediator/collider roles are justified from a causal structure rather than variable names;
- simple DAGs are constructed and critiqued as assumption maps, not proof;
- invalid adjustment strategies are recognized;
- selection, measurement and missingness are explained by mechanism;
- residual/unmeasured confounding is not declared solved merely because adjustment occurred;
- randomization is correctly understood as powerful but stage-specific protection;
- target-trial emulation is distinguished from actual randomized assignment;
- internal validity is separated from applicability;
- every applied scenario includes repairability/data limitation and a calibrated conclusion;
- the ROBINS-I V2 webpage is used only as a current boundary/domain source, not for formal scoring;
- independent assessment occurs only after source-guided study and outside NotebookLM.
