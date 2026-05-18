# Manuscript and Results

## When to load

Load this file for whole-manuscript architecture, manuscript outline or draft audits, publication-readiness checks, aim-method-result-discussion alignment, Results writing, preliminary-data communication, abstract alignment, submission-readiness triage, high-level table/figure narrative discipline, and manuscript-level AI-assisted writing/source-work defensibility.

Use it first when the user asks for a full manuscript audit, manuscript coordination plan, or Results/preliminary-data help. If the task becomes primarily gap, literature-review, Discussion, peer-review, method-fit, meta-analysis, or language/outreach work, keep this file as the manuscript hub and hand off to the section-specific reference.

## Core roles

| Resource | Runtime role | Boundary |
|---|---|---|
| P014 | Manuscript-wide architecture and publication-readiness hub/integrator. Coordinates target audience/journal, authorship/work ownership planning when governed by local norms, Introduction, Methods, Results, Discussion, title, submission rules, and final checklist. | Not a cluster, not an abstract manual, not an authorship-ethics authority, and not a replacement for section-specific references or journal instructions. Use it to align sections, then load the relevant section file. |
| P006 | Local findings-communication resource for Results, Discussion-adjacent findings language, preliminary data, grant/qual materials, progress updates, and figure/table references. | Adjacent to Discussion but not a Discussion-cluster member. Keep Results reporting separate from Discussion interpretation. |
| P027 | Adjacent AI-assisted scientific writing/source-work quality-control gate for authorial ownership, evidence traceability, citation reliability, disclosure awareness, and submission defensibility. | Not a manuscript template, not a current journal-policy authority, and not a ban on source-grounded AI-assisted writing. Load `references/ai-assisted-source-work-quality.md` when AI use materially affects the manuscript. |

## Manuscript alignment workflow

Use P014 as an alignment engine, not as a universal template. Audit the manuscript as an evidence chain:

1. **Target audience/journal.** Identify the intended readers, genre, and journal or venue expectations if supplied. Do not invent journal-specific rules. If rules are missing, audit for general reader fit and say that journal-specific formatting needs supplied guidance.
2. **Central aim.** State the paper’s specific aim(s) in one or two sentences. The aim should answer the gap/problem, not merely name a topic.
3. **Introduction.** Check the narrowing argument: importance -> what is known -> what is not known -> why the missing knowledge matters -> specific aim. If the opening is a broad topic or unsupported problem statement, hand off to `references/cluster-gap-problem.md`; if it lacks synthesis, hand off to `references/cluster-literature-review.md`.
4. **Methods.** Check whether the Methods let readers understand how evidence was produced and how to interpret it: setting, participants/sample, design/timing, data source/collection, variables/measures, covariates, analysis aligned to each objective, and ethics where relevant. Require justification of choices. Provide method-fit and transparency guidance, not a full technical protocol, unless the user supplies standards; for high-level non-meta method fit, hand off to `references/method-fit-triage.md`; for meta-analysis/evidence-synthesis workflow, hand off to `references/method-meta-analysis.md`.
5. **Results.** Verify that each aim/objective has a corresponding result and that all reported results were made interpretable by the Methods.
6. **Discussion.** Check that the Discussion interprets key findings, compares with literature/theory, explains implications and limitations, and does not introduce new results. Hand off to `references/discussion-conclusion.md` for the actual Discussion build.
7. **Conclusion.** Check that the ending compresses the completed argument and stays within the design/data. Hand off to `references/discussion-conclusion.md` for Conclusion drafting.
8. **Title.** Check whether the title is informative, searchable, audience-appropriate, and aligned with variables, population/setting, design, timing, or main result where appropriate.
9. **AI/source-work quality if relevant.** If AI helped draft, summarize, outline, polish, translate, compare sources, or handle references, check authorial ownership, visible source support, citation accuracy, meaning preservation, claim scope, and target-rule/disclosure status.
10. **Final checklist.** Audit consistency across aim, Methods, Results, Discussion, title, citations, table/figure messages, limitations, implications, future steps, and any AI-assisted source-work claims.

### Pre-writing manuscript coordination

Use this as high-level coordination support before drafting or revising a paper. Do not decide authorship ethics, institutional policy, journal policy, contribution disputes, or author order without supplied rules. If local norms, PI instructions, contributor roles, or journal authorship criteria are missing, mark them as unresolved.

Check:

- target reader, journal, venue, or audience if known;
- author list, order, responsibilities, and corresponding author only as governed by supplied/local norms;
- section ownership for Introduction, Methods, Results, Discussion, Conclusion, tables/figures, references, abstract, cover letter, and submission materials;
- who owns data, analysis, figure/table generation, citation checking, response-to-reviewers, and final proofreading;
- timeline, review checkpoints, decision owner, and unresolved dependencies;
- missing guidance: author-contribution rules, journal requirements, ethics/data/reporting statements, funding or acknowledgment rules.

Default output:

| Decision | Current status | Owner | Dependency | Next action |
|---|---|---|---|---|

### Submission-readiness and abstract scope

Use this section for high-level triage only. Do not invent journal-specific rules, reporting standards, editor preferences, cover-letter requirements, word limits, or abstract structure.

For submission readiness, check:

- target journal/venue and author guidance supplied or missing;
- title, abstract, Introduction, Methods, Results, Discussion, limitations, and Conclusion alignment;
- claim scope, citation support, table/figure messages, ethics/data/reporting statements, and supplementary material consistency;
- AI-assisted prose, source summaries, citation handling, or disclosure/compliance questions when relevant;
- cover letter or submission-package requirements only if supplied by the user or retrieved from current sources.

For abstracts, build or audit a compact chain: problem/gap -> aim/objective -> design/method -> key result(s) -> scoped contribution/implication. If the target journal specifies a structured abstract, use the supplied structure; otherwise provide a generic alignment scaffold and say that journal-specific abstract requirements are external.

### Manuscript alignment table

Use this table when the user has an outline, draft, or reviewer concern:

| Element | Check | Failure signal | Repair move |
|---|---|---|---|
| Aim | Specific, gap-facing, researchable | Vague “explore X” aim with no gap | Rewrite aim after gap/problem audit |
| Introduction | Narrows to known/unknown/stakes/aim | Background dump or citation list | Rebuild with gap/literature handoff |
| Methods | Explains and justifies evidence production | Methods omit variables, sampling, analysis per aim | Add traceable method-to-aim details |
| Results | Answers aims without interpretation | Statistical-test dump; missing non-significant findings | Build aim-by-aim result map |
| Discussion | Interprets, compares, scopes implications | Repeats Results or overclaims | Use Discussion sequence handoff |
| Conclusion | Compresses contribution and scope | Grand claim beyond design/data | Reduce scope and tie to findings |
| Title | Signals paper content and audience fit | Generic, unsearchable, acronym-heavy | Name population/variables/design/result as useful |

## Results discipline

Results report what the study found. They do not explain why the findings happened except where the genre explicitly combines Results and Discussion.

Use these guardrails:

- Answer the stated aim(s) and objectives directly.
- Report associations, relationships, group differences, patterns, trends, frequencies, themes, or lack of associations as appropriate to design.
- Include non-significant or null findings when they are relevant to an aim, hypothesis, safety signal, feasibility claim, or interpretation boundary.
- Prefer relationship language over test-dumping: say what changed, differed, correlated, predicted, varied, or did not vary, not just which test was significant.
- Avoid causal language unless the design supports causal inference. Use “associated with,” “related to,” “higher among,” “predicted,” or “was observed” when causality is not supported.
- Avoid literature citations in Results unless a specific genre or journal convention requires brief contextual anchoring. Normally save literature connection for Discussion.
- Avoid interpretation, mechanisms, implications, recommendations, or explanations of unexpected findings in Results. Route those to `references/discussion-conclusion.md`.

### Aim-method-result-discussion map

Use this compact map for audits:

| Aim/objective | Method/analysis that produces evidence | Result that answers it | Discussion meaning needed? | Scope limit |
|---|---|---|---|---|
| Aim 1 |  |  |  |  |
| Aim 2 |  |  |  |  |
| Aim 3 |  |  |  |  |

A missing cell indicates a manuscript alignment problem. Do not hide the problem by polishing prose.

## P006 local findings language

Use P006 to choose the local move, then adapt the wording to the user’s data and genre. Do not paste stock phrases mechanically.

| Move | Use in Results when... | Use in Discussion/preliminary-data contexts when... | Safe language pattern |
|---|---|---|---|
| Stating findings | Reporting the direct answer | Opening interpretation from a finding | “The findings indicate/reveal/show...” |
| Patterns/trends | Describing directional regularities | Explaining broader meaning of a pattern | “A consistent pattern was...” / “The data showed a trend toward...” |
| Significance | Reporting statistical or practical importance | Scoping importance cautiously | “This difference was statistically significant...” / “The effect size suggests...” |
| Relationships | Describing associations | Connecting association to possible mechanism | “X was positively/negatively associated with Y...” |
| Comparisons | Contrasting groups, conditions, time points | Explaining why the contrast matters | “Compared with..., Group A showed...” |
| Tables/figures | Anchoring text in visible evidence | Pointing readers to support for interpretation | “As shown in Table/Figure X...” |
| Unexpected result | Naming surprise without explanation | Explaining possible reasons | “Contrary to expectations...” |
| Cautious claim | Avoiding overreach | Moving from finding to implication | “These findings may indicate...” |

### Results paragraph pattern

For a Results paragraph, use:

1. claim sentence answering the aim;
2. direction/magnitude/pattern sentence;
3. key comparison or relationship sentence;
4. table/figure anchor if useful;
5. null/non-significant result if relevant;
6. no mechanism, implication, recommendation, or literature explanation.

## Preliminary-data guidance

For proposals, qual documents, grant-like pages, committee updates, and progress reports, preliminary data usually supports feasibility, promise, measurement adequacy, recruitment viability, or rationale. It is not a full manuscript Results section unless the user asks for that genre.

Use cautious framing:

- Say what the preliminary evidence suggests, not what it proves.
- Tie the evidence to feasibility, rationale, or the next study aim.
- Distinguish observed patterns from explanations.
- Avoid population-wide claims from small, local, pilot, partial, or convenience samples.
- Mention uncertainty or incompleteness when it affects interpretation.
- If the user wants proposal packaging, hand off to `references/cluster-front-end-proposal.md`.

Preliminary-data paragraph pattern:

1. context of the preliminary source/sample;
2. observed finding or pattern;
3. cautious meaning for feasibility/rationale;
4. how it supports the proposed next step;
5. limitation/scope note if needed.

## Output selector

Choose the smallest useful output:

| User need | Output |
|---|---|
| “Audit my manuscript/outline” | Manuscript alignment audit + section-specific handoff list |
| “Plan who writes what” | Pre-writing coordination table with unresolved authorship/policy questions |
| “Do my sections line up?” | Aim-method-result-discussion map |
| “Write Results” | Results paragraph(s) with boundary note if interpretation is requested |
| “Explain this table/figure” | Figure/table narrative: message, key pattern, non-redundant text |
| “Describe preliminary data” | Cautious preliminary-data paragraph tied to feasibility/rationale |
| “Make it publication-ready” | Publication-readiness repair plan: alignment, scope, evidence, section handoffs |
| “Write/check my abstract” | Abstract alignment scaffold or draft with journal-specific placeholders |
| “Prepare a cover letter/submission package” | High-level readiness checklist or generic scaffold only with explicit missing-source notes |

## Handoffs

- `references/cluster-gap-problem.md`: weak gap, vague aim, problem statement, novelty, research questions/objectives.
- `references/cluster-literature-review.md`: background/literature synthesis, citation patterns, related-work structure.
- `references/discussion-conclusion.md`: interpretation, unexpected results, implications, limitations, future work, Conclusion.
- `references/peer-review-revision.md`: reviewer red flags, revise-and-resubmit, major revision strategy, claim-scope audit.
- `references/method-fit-triage.md`: high-level non-meta design-family fit for RQs, aims, objectives, hypotheses, and evidence type.
- `references/method-meta-analysis.md`: meta-analysis or quantitative evidence-synthesis workflow; do not treat P014 as a full methods protocol.
- `references/language-and-outreach.md`: academic phrasing, hedging, tone, concise local wording after the logic is sound.
- `references/ai-assisted-source-work-quality.md`: AI-assisted manuscript/source-work audit, citation reliability, authorial ownership, disclosure awareness, or submission defensibility.
