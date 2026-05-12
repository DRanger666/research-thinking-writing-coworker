# Method Meta-Analysis

## When to load

Load this file when the user asks about planning or auditing a meta-analysis, quantitative evidence synthesis, effect-size planning, meta-analysis feasibility, literature search for a meta-analysis, inclusion/exclusion criteria for a meta-analysis, coding quantitative study information, or drafting/auditing meta-analysis Methods, Results, or proposal methods language.

This file covers P018 only: high-level meta-analysis / quantitative evidence-synthesis planning, feasibility checking, positioning, and reporting structure. It is not universal methods guidance, not general statistics tutoring, not a complete technical protocol, and not authority for field-specific reporting standards or risk-of-bias procedures. Use `references/method-fit-triage.md` for high-level non-meta design-family fit. Use supplied or retrieved external standards for PRISMA, risk-of-bias tools, registration, field-specific reporting, or software-specific implementation.

## First gate: is meta-analysis feasible?

Before planning a meta-analysis, check whether the topic has an evidence base suitable for quantitative synthesis. Do not infer feasibility from the topic name alone.

| Feasibility question | Why it matters | If weak or unknown |
|---|---|---|
| Is there a focused research question or relationship/intervention to synthesize? | Meta-analysis needs a bounded quantitative target, not just a broad theme. | Use `references/cluster-gap-problem.md` to narrow the problem, RQ, and scope. |
| Are there enough relevant primary studies? | Some topics lack sufficient evidence for meta-analysis. | Consider an integrative/narrative review route via `references/cluster-literature-review.md`. |
| Are studies comparable enough? | Constructs, populations, interventions, outcomes, and designs must be meaningfully related. | Re-scope, split into subquestions, or avoid quantitative synthesis. |
| Are quantitative effects extractable or convertible? | Meta-analysis requires effect sizes or data that can support effect-size calculation/conversion. | Ask for study tables, reported statistics, or methods expertise; do not invent effects. |
| Do prior meta-analyses already exist? | The project may need an update, moderator angle, new scope, or different rationale. | Use the prior synthesis as positioning, not automatic novelty. |

If the evidence base is insufficient, recommend an integrative review, narrative synthesis, scoping-style review, or literature-review positioning task only at a high level, unless the user supplies an external standard.

## P018 high-level workflow

Use this as a planning and audit scaffold, not as a statistical recipe.

| Step | Planning question | Runtime output |
|---|---|---|
| 1. Research question and scope | What relationship, intervention, outcome, construct, population, setting, period, or literature boundary is being synthesized? | Focused RQ, scope statement, and boundary notes. |
| 2. Literature search | Where will relevant studies be found, and how will prior reviews/meta-analyses seed the search? | Search-source plan and query/record-keeping checklist. |
| 3. Inclusion/exclusion logic | Which studies count, which do not, and why? | Inclusion/exclusion planning table. |
| 4. Effect-size choice | What common quantitative measure best matches the question and reported evidence? | Effect-size decision prompt, with “needs methods/statistics confirmation” when necessary. |
| 5. Analytical method choice | Does the question concern an overall relationship, intervention effect, moderators, mediators, or model structure? | High-level analysis-route options, not formulas. |
| 6. Software/implementation planning | What tool environment will be used, and who will validate the implementation? | Non-prescriptive implementation plan and expertise checkpoint. |
| 7. Coding/extraction | What variables, effects, study features, moderators, and non-target variables must be coded? | Coding-plan sketch and extraction-sheet fields. |
| 8. Analysis and reporting | What decisions, results, uncertainty, heterogeneity, and limitations must be transparent? | Reporting outline for Methods, Results, and limitations. |

P018 mentions software as part of the workflow, but do not make current software capability claims or tool-specific instructions unless the user supplies standards, code, or external methods sources. Keep implementation guidance non-prescriptive.

## Scope, moderators, mediators, and heterogeneity prompts

Ask only as needed; otherwise state assumptions and proceed.

- **Scope boundary**: Are the included studies similar enough in construct, intervention, outcome, population, context, study design, and time frame?
- **Prior synthesis boundary**: Is the contribution an updated sample of primary studies, a different population/context, a moderator/mediator question, or a correction of unresolved inconsistency?
- **Moderator prompts**: Does the effect differ by population, measurement approach, intervention type, setting, design, time period, publication status, geography, or discipline?
- **Mediator prompts**: Is the user asking why or through what mechanism an effect occurs? If yes, mark this as a higher-complexity route needing stronger methodological support.
- **Heterogeneity prompts**: Are differences among studies expected, meaningful, and planned for conceptually? Do not reduce heterogeneity to a number before the constructs and scope are clear.
- **Boundary risk**: A moderator idea is not automatically justified. It must connect to theory, prior inconsistencies, measurement differences, or a practical/study-design rationale.

## Using meta-analysis inside larger research-writing tasks

P018 can support several document stages, but it should hand off when the task moves outside evidence-synthesis workflow.

| User goal | Use this file for... | Then hand off to... |
|---|---|---|
| Gap/problem rationale | Feasibility, prior meta-analysis check, evidence-base suitability, possible moderator/update rationale | `references/cluster-gap-problem.md` |
| Literature positioning | How the evidence base is grouped, what prior reviews show, where quantitative synthesis fits | `references/cluster-literature-review.md` |
| Proposal or concept method | High-level methods scaffold, inclusion logic, extraction plan, feasibility caveats | `references/cluster-front-end-proposal.md` |
| Manuscript Methods/Results | Workflow transparency, method-section scaffold, results-reporting outline | `references/manuscript-and-results.md` |
| Discussion or conclusion | Interpreting synthesized findings, heterogeneity, limitations, implications | `references/discussion-conclusion.md` |
| Reviewer comments or revision | Response strategy when reviewers challenge search, inclusion, effect choice, overclaims, or reporting | `references/peer-review-revision.md` |

## Output selector

| User asks for... | Produce... |
|---|---|
| “Should I do a meta-analysis?” | Feasibility audit with evidence-base questions and an integrative-review alternative if needed. |
| “What are the steps?” | High-level workflow checklist aligned to P018. |
| “Help write proposal methods” | Methods scaffold with scope, search, inclusion/exclusion, effect-size plan, extraction, analysis, reporting caveats. |
| “Define inclusion/exclusion criteria” | Planning table with criterion, include, exclude, rationale, and evidence needed. |
| “What should I code?” | Coding-plan sketch: study ID, sample, design, constructs, outcomes, effect data, moderators, notes. |
| “How should I report it?” | Reporting outline for transparent methods decisions, study flow at a general level, effect summaries, heterogeneity, limitations, and interpretation boundaries. |
| “Reviewer challenged my meta-analysis” | Reviewer-facing issue map, then hand off to `references/peer-review-revision.md`. |

## Compact templates

### Feasibility audit

| Gate | Status | Evidence needed | Decision |
|---|---|---|---|
| Focused quantitative question | Known / unclear / weak | RQ, constructs, intervention/outcome | Proceed / narrow / reroute |
| Sufficient primary studies | Known / unclear / weak | Search results, prior reviews, bibliography | Proceed / search more / integrative review |
| Comparable studies | Known / unclear / weak | Study table by design, population, outcome | Combine / subgroup / split scope |
| Extractable effects | Known / unclear / weak | Reported statistics or raw summaries | Proceed / request data / methods help |
| Clear contribution | Known / unclear / weak | Prior meta-analyses, moderator/update rationale | Proceed / reposition / gap repair |

### Methods scaffold

1. State the research question and quantitative synthesis target.
2. Define the scope boundaries: population, construct/intervention, outcome, study type, time/context where relevant.
3. Describe the literature search plan at a high level.
4. Specify inclusion/exclusion logic and why it matches the question.
5. Identify the planned effect-size family or state that effect-size choice needs methods confirmation.
6. Sketch coding/extraction categories, including possible moderators or non-target variables.
7. Name the analysis route only at a conceptual level.
8. State how decisions and results will be reported transparently, including heterogeneity and limitations.

## Non-negotiables

- Do not provide detailed statistical recipes, formulas, or software commands from P018 alone.
- Do not claim PRISMA, risk-of-bias, field-specific reporting-standard, or software authority unless the user supplies external standards or attached source material supports it.
- Do not treat P018 as experimental, computational, qualitative, survey, interview, ethnographic, or general methods design coverage.
- Do not fabricate methodological feasibility, effect sizes, comparable evidence, or novelty from a vague topic.
- Do not let a meta-analysis label replace gap logic, literature synthesis, proposal rationale, manuscript alignment, Discussion interpretation, or reviewer-response strategy.
