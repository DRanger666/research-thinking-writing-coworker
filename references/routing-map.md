# Routing Map

## Purpose

Use this file as the central dispatch layer after the skill has triggered. Route by the user’s task, stage, document genre, and needed intellectual move before choosing a post or cluster. Do not route by post ID first.

This file tells the runtime agent what reference to load first, what handoff may be needed, whether to ask a clarifying question, what output form to produce, and what boundary risk to watch for.

## Route Priority Stack

Use this stack before selecting a reference:

1. **Genre and stage:** identify whether the user is doing idea work, proposal/front-end work, literature review, manuscript writing, revision response, outreach, meta-analysis planning, or high-level method-fit triage.
2. **Failure signal:** identify the main problem: weak gap, missing synthesis, aim-method mismatch, method-design mismatch, Results/Discussion confusion, overclaiming, defensive response, unsupported source claim, AI-substituted source work, fabricated/source-invisible references, or only surface language.
3. **Evidence availability:** decide whether the task has supplied papers, notes, data, reviewer comments, target guidance, or recipient details. Missing evidence should trigger a fail-soft output, not fabrication.
4. **Boundary gate:** check whether the request is only partially supported by the KB: abstracts, submission packages, reporting standards, full figure/table design, current literature, current lab fit, or detailed methods/statistics.
5. **Output form:** choose the smallest useful artifact: diagnosis, route map, matrix, outline, scaffold, draft, or revision.
6. **Handoff:** load a second reference only when the task crosses layers.

## Core Resource Legend

### True clusters

| Cluster | Members | Runtime role |
|---|---|---|
| Academic reasoning-language | P001/P009 | Cross-paper academic phrasing and reasoning anchors. |
| Literature-review construction | P012/P002/P011/P016 | Literature review purpose, macro architecture, local motifs, and AI-assisted synthesis workflow. |
| Gap and problem development | P003/P020/P022/P024/P013/P017/P015 | Gap discovery, taxonomy, quality check, problem statement, and gap-statement formulation. |
| Discussion construction | P004/P021/P019 | Discussion structure, sequence, and unexpected-results reasoning. |
| Peer-review readiness and revision response | P023/P025 | Pre-submission red flags and major-revision response logic. |
| Study setup / front-end presentation | P005/P007/P026 | Concept paper, proposal, Chapter 1, specific-aims-like front-end, and research-idea presentation. |

### Special non-cluster roles

| Resource | Runtime role |
|---|---|
| P014 | Manuscript-wide architecture and publication-readiness hub/integrator. |
| P006 | Results-and-Discussion findings communication; adjacent to Discussion but not inside the Discussion cluster. |
| P008 | Conclusion architecture. |
| P010 | Scientific correspondence / research outreach. |
| P018 | Meta-analysis / quantitative evidence-synthesis workflow; not universal methods guidance. |
| P027 | AI-assisted scientific writing/source-work quality-control gate; adjacent to P016, P014, and P023, not a cluster member or current policy authority. |

## Quick Route Table

| User task or signal | Load first | Optional handoff | Typical output | Main boundary risk |
|---|---|---|---|---|
| Vague idea / early research direction | `cluster-gap-problem.md` | `cluster-front-end-proposal.md`, `cluster-literature-review.md` | Idea map, candidate gap routes, next-step table | Prematurely drafting prose before clarifying the research logic. |
| Gap discovery / originality | `cluster-gap-problem.md` | `cluster-literature-review.md` | Gap taxonomy, originality-combination table, search plan | Treating “no exact prior study” as sufficient novelty. |
| Problem statement | `cluster-gap-problem.md` | `cluster-front-end-proposal.md`, `manuscript-and-results.md` | Problem-statement audit, rewrite, population/setting/gap/stakes map | Polishing a vague topic statement instead of diagnosing it. |
| RQs, aims, objectives, hypothesis shaping | `cluster-gap-problem.md` | `cluster-front-end-proposal.md`, `manuscript-and-results.md` | RQ/aim alignment table, hypothesis logic, measurable objective draft | Making aims untestable or disconnected from the gap. |
| Literature review / background / related work | `cluster-literature-review.md` | `cluster-gap-problem.md`, `language-and-outreach.md` | Review architecture, theme map, paragraph motif skeleton | Author-by-author summary instead of synthesis. |
| AI-assisted literature synthesis | `cluster-literature-review.md` | `ai-assisted-source-work-quality.md`, `cluster-gap-problem.md` | LLM paper-questioning workflow, synthesis matrix, theme plan, source-control check | Fabricating synthesis without source papers/notes. |
| AI-assisted scientific writing or source-work audit | `ai-assisted-source-work-quality.md` | `cluster-literature-review.md`, `manuscript-and-results.md`, `peer-review-revision.md`, `language-and-outreach.md` | AI-use risk table, source-control audit, defensibility checklist | Treating AI output as evidence, citations, interpretation, or compliance without human/source verification. |
| Concept paper / early research memo | `cluster-front-end-proposal.md` | `cluster-gap-problem.md`, `cluster-literature-review.md` | Concept scaffold, idea memo outline | Overformalizing before the idea is coherent. |
| Proposal / qual / grant-like front end / specific aims | `cluster-front-end-proposal.md` | `cluster-gap-problem.md`, `cluster-literature-review.md`, `manuscript-and-results.md` | Proposal route map, aims page skeleton, significance/rationale audit | Treating one genre’s format as universal. |
| Thesis Chapter 1 / front-end setup | `cluster-front-end-proposal.md` | `cluster-gap-problem.md`, `cluster-literature-review.md` | Chapter 1/front-end audit, paragraph plan | Using P026 as a rigid template outside thesis contexts. |
| High-level non-meta method/design fit | `method-fit-triage.md` | `cluster-gap-problem.md`, `cluster-front-end-proposal.md`, `manuscript-and-results.md` | Gap/RQ/aim-to-evidence design-fit table | Overclaiming detailed methods, statistics, protocol, or reporting-standard authority. |
| Full manuscript architecture or audit | `manuscript-and-results.md` | task-specific references as needed; `ai-assisted-source-work-quality.md` if AI assistance affected source work, citations, or prose | Manuscript alignment audit, section route map | Flattening all sections into one generic template. |
| Results / preliminary data | `manuscript-and-results.md` | `language-and-outreach.md`, `discussion-conclusion.md` if interpretation is requested | Results paragraph, preliminary-data framing, figure/table narrative | Interpreting too much in Results; causal overreach. |
| Discussion / unexpected results | `discussion-conclusion.md` | `manuscript-and-results.md`, `language-and-outreach.md` | Discussion outline, interpretation map, unexpected-results explanation | Repeating Results or ignoring surprising findings. |
| Conclusion | `discussion-conclusion.md` | `language-and-outreach.md`, `manuscript-and-results.md` | Conclusion structure, final synthesis, closing paragraph | Overclaiming or repeating detailed Results. |
| Peer-review red-flag audit | `peer-review-revision.md` | `manuscript-and-results.md`, relevant section file, `ai-assisted-source-work-quality.md` if AI/source-control risk is visible | Reviewer-risk audit, red-flag list, repair plan | Generic encouragement instead of reviewer-facing critique. |
| Major revisions / reviewer response | `peer-review-revision.md` | `cluster-literature-review.md`, `discussion-conclusion.md`, `manuscript-and-results.md` | Response strategy, revision matrix, evidence-backed rebuttal plan | Defensive response or vague “addressed” language. |
| Meta-analysis / quantitative evidence synthesis | `method-meta-analysis.md` | `cluster-gap-problem.md`, `cluster-literature-review.md`, `manuscript-and-results.md` | Meta-analysis workflow checklist, feasibility questions, methods scaffold | Treating P018 as a full technical protocol. |
| Academic reasoning-language refinement | `language-and-outreach.md` | task-specific file if logic is weak; `ai-assisted-source-work-quality.md` if AI polish may have altered meaning, evidence, or claim scope | Reasoning-move labels, revised prose, tone/hedging suggestions | Decorative phrasing over weak reasoning. |
| Research outreach email | `language-and-outreach.md` | none unless research fit needs gap/literature logic | Fit audit, concise cold email, direct ask | Generic flattery or manuscript-style verbosity. |
| Abstract | `manuscript-and-results.md` | `language-and-outreach.md`, section-specific reference if logic is weak | Aim-method-result-contribution scaffold or abstract alignment audit | Pretending the KB contains abstract-specific or journal-specific abstract rules. |
| Cover letter / submission package | `manuscript-and-results.md` | `language-and-outreach.md` | Submission-readiness checklist or generic cover-letter scaffold with placeholders | Inventing journal fit, editor expectations, or submission requirements. |
| Reporting-standard compliance | task-specific reference | external/supplied standard required | Compliance evidence-needed checklist; retrieve current standard if tools are available and not disallowed | Treating the KB as PRISMA/CONSORT/STROBE/JBI/etc. authority. |
| Current literature / latest citations | `cluster-literature-review.md` | `cluster-gap-problem.md` | Retrieve current sources when tools are available and not disallowed; otherwise source-acquisition plan, search strategy, or synthesis matrix template | Fabricated currency or citation claims. |
| Professor/lab fit or current openings | `language-and-outreach.md` | none unless research idea needs gap logic | Retrieve current recipient evidence when tools are available and not disallowed; otherwise fit-audit checklist or email with explicit placeholders | Inventing recipient-specific projects, papers, openings, or lab priorities. |
| Figure/table design | `manuscript-and-results.md` | `language-and-outreach.md` | Message-focused table/figure narrative and claim-scope check | Providing full visual, statistical, or journal-specific design without source guidance. |
| Pure grammar-only edit | none or `language-and-outreach.md` if reasoning/tone matters | task-specific file only if logic is weak | Minimal edit or note that the skill is not needed for pure grammar | Turning a simple grammar request into an unnecessary research audit. |

## Ask-vs-Proceed Heuristics

Ask a clarifying question only when correctness depends on missing information. Clarify:

- document genre: manuscript, thesis, proposal, grant-like page, qual, memo, outreach, reviewer response
- stage: idea exploration, outline, draft, revision, final audit
- audience: advisor, committee, journal reviewer, PI, funder, collaborator
- available evidence: papers, notes, abstracts, bibliography, preliminary data, reviewer comments
- desired output: diagnosis, route map, table, outline, prose, audit, or revision plan

Proceed with explicit assumptions when the request is exploratory, general, or already gives enough context. State the assumption briefly and continue.

When key information is absent, fail softly: produce a placeholder scaffold, assumptions list, evidence-needed matrix, source request, or search plan. Do not fabricate the missing evidence.

If the user asks for prose but the reasoning is visibly weak, diagnose first, then offer a revised version.

If the user asks for current or recent sources, journal rules, reporting standards, software capability, professor/lab fit, openings, or another time-sensitive fact, treat that as retrieval intent unless the user forbids retrieval. When retrieval tools are available and not disallowed, retrieve current sources before synthesizing. When retrieval is unavailable or forbidden, produce a source-acquisition plan and a reusable synthesis or compliance template.

## Output-Form Selector

| User stage | Prefer output forms |
|---|---|
| Early idea | Diagnostic questions, route map, idea tree, gap search plan |
| Gap/problem | Gap taxonomy, weak/strong gap audit, problem-statement map |
| RQs/aims/hypotheses | Alignment table, decision table, hypothesis logic map |
| Method/design fit | Evidence-needed map, design-family triage, scope/cannot-support table |
| Literature review | Theme map, section architecture, paragraph motifs, synthesis matrix |
| Proposal/front end | Concept scaffold, specific-aims-like outline, Chapter 1 audit |
| Manuscript | Section alignment audit, aim-method-result-discussion map |
| Results/preliminary data | Results paragraph, figure/table narrative, cautious claim map |
| Discussion | Interpretation route, implication/limitation map, Discussion outline |
| Conclusion | Compressed synthesis, contribution/limitation/recommendation check |
| Peer review | Red-flag audit, revision matrix, reviewer-response plan |
| Outreach | Fit audit, concise email draft, direct-ask refinement |
| Language refinement | Reasoning-move labels, precise rewrite, hedging/tone adjustment |
| AI-assisted source work | AI-use risk table, source-visibility check, citation/claim audit, defensibility checklist |
| Partial-support task | Scope note, source-needed checklist, high-level scaffold |

## Partial-Support Default Artifacts

Partial support should not become a refusal. Use this default pattern:

`scope note -> generic scaffold or audit matrix -> missing-source checklist -> retrieval/search plan or next decision`

| Partial-support task | Default artifact |
|---|---|
| Abstract without journal guidance | Problem/gap -> aim/objective -> design/method -> key result slot -> scoped contribution scaffold; request journal structure or word limit if needed. |
| Cover letter or submission package | Generic cover-letter or submission-readiness skeleton with placeholders; list missing journal/editor/submission requirements. |
| Reporting-standard compliance | Evidence-needed compliance matrix; retrieve the current standard if tools are available and not disallowed, otherwise provide a standards lookup plan. |
| Current literature or latest citations | Retrieve current sources when possible; otherwise provide database/query plan, inclusion boundaries, and a synthesis matrix template. |
| Professor/lab fit or current openings | Retrieve current recipient evidence when possible; otherwise provide fit-evidence checklist and placeholder email. |
| Figure/table design | Message, claim scope, reader task, and caption/narrative scaffold; avoid full statistical, visual, or journal-specific design rules without sources. |
| Detailed methods/statistics | High-level method-fit triage plus missing expertise/source list; do not invent protocols, formulas, software commands, or reporting rules. |
| AI-use disclosure or target policy | Retrieve current journal, funder, committee, supervisor, institutional, or publisher rules when tools are available and not disallowed; otherwise provide a missing-policy checklist and placeholder disclosure/compliance plan. |

## Boundary Gates

Before drafting, check whether a boundary gate applies:

- Do not polish weak gap logic; route to `cluster-gap-problem.md`.
- Do not treat P010 as manuscript/proposal writing; outreach must stay fit-based and concise.
- Do not treat P018 as universal methods/statistics guidance; it is meta-analysis/evidence-synthesis only.
- Do not treat high-level method-fit triage as a full protocol, statistical plan, or software workflow.
- Do not merge P006 into the Discussion cluster; it also supports Results and preliminary data.
- Do not use P026 as a rigid universal Chapter 1 template; transfer its content-level audit only.
- Do not treat phrase resources as solutions to reasoning problems.
- Do not fabricate literature synthesis from topic names alone. Ask for papers, notes, abstracts, a bibliography, or mark assumptions.
- Do not read P027 as a ban on source-grounded AI-assisted literature work, an ethics doctrine for the whole skill, a seventh cluster, or current journal/funder/publisher policy authority.
- Do not let AI substitute for literature judgment, citation verification, source support, primary data interpretation, ethics/plagiarism certification, or target-specific compliance decisions.
- Do not route every manuscript problem to P014 alone. P014 is a hub; load section-specific references when needed.
- Do not treat proposal, manuscript, thesis, and outreach genres as interchangeable.
- Do not invent current evidence, lab fit, journal instructions, reporting standards, or software/methods rules.
- Treat abstracts, cover letters/submission packages, reporting-standard compliance, full figure/table design, current-source checks, and detailed methods/statistics as partial-support tasks unless external source material is supplied or retrieved; still return the default partial-support artifact.
- If provenance or source-vs-transfer status matters, load `source-provenance-map.md`.

## Handoff Rules

Use handoffs when a task crosses layers:

- **Gap/problem → front-end/proposal:** after identifying a gap or problem, load `cluster-front-end-proposal.md` to package it into a concept memo, proposal, Chapter 1, specific aims, or qual-style front end.
- **Gap/problem → method fit:** when the question becomes whether the RQ, aim, objective, or hypothesis can be answered by a plausible design family, load `method-fit-triage.md`.
- **Literature review → gap/problem:** if the review lacks a clear gap, load `cluster-gap-problem.md`.
- **AI-assisted literature synthesis → source-work quality:** when P016-style AI help is used on papers, notes, or review drafts, load `ai-assisted-source-work-quality.md` if source visibility, citation reliability, authorial ownership, disclosure, or defensibility is in question.
- **Gap/problem → literature review:** if the gap must be justified in the field, load `cluster-literature-review.md`.
- **Manuscript hub → section-specific:** start with `manuscript-and-results.md` for whole-paper alignment, then hand off to gap/problem, literature review, Results, Discussion, or Conclusion references as needed.
- **Results/preliminary data → Discussion:** stay in `manuscript-and-results.md` for reporting; load `discussion-conclusion.md` only when interpretation, implications, limitations, or unexpected results are requested.
- **Discussion → Conclusion:** use `discussion-conclusion.md`; keep Discussion interpretation broader and Conclusion compressed.
- **Peer-review/revision → manuscript/section repair:** load `peer-review-revision.md` first, then load the section-specific reference tied to the reviewer criticism.
- **Meta-analysis → gap/literature/manuscript:** use `method-meta-analysis.md` for the workflow, then hand off to gap discovery, literature positioning, or manuscript architecture as needed.
- **Non-meta method fit → proposal/manuscript:** use `method-fit-triage.md` for alignment, then hand off to front-end packaging or manuscript alignment as needed.
- **Language refinement → task-specific logic:** if prose is weak because the underlying reasoning is weak, load the relevant task reference before rewriting.
- **AI-assisted polish → source-work quality:** if polishing, summarizing, outlining, or translation may have changed meaning, claim strength, citation fit, source support, or disclosure/compliance status, load `ai-assisted-source-work-quality.md`.
