# Literature Review Construction

## Load when

Load this file when the user is planning, diagnosing, drafting, revising, or auditing a literature review, Chapter 2, background section, related-work section, proposal literature section, theme map, synthesis matrix, or AI/LLM-assisted paper comparison workflow. Load `references/routing-map.md` first if the user also asks about gap discovery, proposal framing, manuscript architecture, reviewer comments, or AI-assisted source-work defensibility.

Do not fabricate synthesis from topic names alone. If the task requires claims about what the literature says, ask for or rely on supplied papers, abstracts, notes, bibliographies, source summaries, search results, or the user's own reading notes. If those are absent, produce a structure, questions, and evidence-needed matrix rather than asserting field patterns as fact. For current, recent, or "latest" literature, retrieve current sources when tools are available and not explicitly disallowed; if retrieval is unavailable or forbidden, produce a search plan and synthesis matrix template rather than pretending to know the present field state.

## Key distinctions

| Form | What it does | Common failure |
|---|---|---|
| Summary | Reports what one source says. | Becomes a sequence of isolated author notes. |
| Synthesis | Connects sources to show patterns, tensions, methods, theories, gaps, and implications. | Claims patterns without source evidence. |
| Background | Narrows context enough for the reader to understand why the study matters. | Becomes a shallow topic overview or full Chapter 2 inside a front end. |
| Related work | Positions the study among adjacent approaches, debates, methods, or applications. | Lists studies without explaining relation to the present study. |
| Literature review | Builds a field-level argument that makes the study defensible, necessary, and logically connected to RQs/aims. | Author-by-author bibliography with commentary. |

P012 supplies the purpose and credibility frame: the review should show that the topic is defensible, the RQs make sense, and the study deserves to exist. P002 supplies macro architecture. P011 supplies local review motifs. P016 supplies an operational AI/LLM-assisted interrogation and refinement workflow. P027 is adjacent: use `references/ai-assisted-source-work-quality.md` when AI assistance raises source visibility, citation reliability, authorial ownership, or defensibility questions.

## Macro workflow

1. **Define the review job.** Identify genre and scale: thesis Chapter 2, manuscript background, proposal literature review, related work, or short rationale. Do not import Chapter 2 depth into a proposal front end unless the genre requires it.
2. **Set boundaries.** Define time frame, geography/context, disciplines, population/setting, theories, methods, and source types. Boundaries prevent the review from becoming everything ever written.
3. **Inventory source evidence.** Ask for papers, notes, abstracts, bibliography, or user summaries. Record for each source: topic, population/context, method, theory, findings, limitations, and relevance to the user's study.
4. **Group by intellectual function, not author order.** Build themes around debates, methods, theories, contexts, populations, variables, mechanisms, or chronological shifts.
5. **Extract cross-study patterns.** Look for consensus, contradiction, unresolved debate, repeated variables, missing variables, dominant methods, excluded populations/settings, theory limits, and outdated evidence.
6. **Create the review architecture.** Sequence sections so each one narrows or deepens the argument: field context -> major streams -> tensions and method/theory evaluation -> gap convergence -> transition to purpose/RQs.
7. **Build paragraph skeletons.** For each paragraph, state the synthesis claim first, then group evidence, contrast or evaluate sources, explain significance, and transition forward.
8. **Audit the gap bridge.** If the review does not clearly lead to a missing piece, load `references/cluster-gap-problem.md`.
9. **Draft or revise.** Only after source logic is clear, use concise academic prose. Avoid decorating weak synthesis with phrases.

## Source-grounded AI/LLM synthesis workflow

Use AI as a structured reading and comparison assistant, not as a source substitute.

- Ask the user to provide papers, abstracts, notes, bibliographies, or their summaries. If unavailable, generate a reading protocol and synthesis matrix rather than a literature claim.
- For each source, ask targeted questions: What is the research question? What population/context? What method? What theory? What finding? What limitation? What citation-worthy claim?
- Across sources, ask P016-style questions: What similarities exist? What patterns emerge? Which variables recur? Where are contradictions? What gaps remain? Which theories are used? How can studies be grouped into themes?
- Separate extraction from interpretation. Extraction captures what sources say; interpretation explains relationships across sources; writing turns relationships into paragraphs.
- Ask the model to show a claim-evidence table before drafting. If a claim lacks evidence, mark it as a hypothesis, assumption, or search target.
- Use AI for simplifying difficult papers, comparing authors, improving flow, academic paraphrasing, refining rough paragraphs, and structuring sections only after the source basis is visible.
- If AI summarizes, paraphrases, outlines, or drafts from source material, use P027 checks: verify references, preserve meaning, keep the user's interpretation primary, and do not let model memory become a substitute source.

## Anti-patterns to catch

- **Author-by-author listing:** "Smith found..., Jones found..., Chen found..." without a synthesis claim.
- **Bibliography with commentary:** Each paragraph is a mini annotation, not an argument.
- **Evidence dumping:** Too many citations attached to a broad statement with no explanation of pattern or contrast.
- **Gap by assertion:** The review ends with "more research is needed" without showing where knowledge stops.
- **Method blindness:** The review ignores whether methods dominate, limit, or bias the evidence base.
- **Theory decoration:** Theory is named but not used to explain, organize, challenge, or interpret findings.
- **Overloaded front end:** A Chapter 1/proposal introduction becomes a full literature review. Hand off to `references/cluster-front-end-proposal.md` for genre fit.
- **False currency:** Claims that the literature is current or outdated without field-sensitive evidence. Ask for supplied sources or retrieve current sources when appropriate.
- **Source-invisible AI synthesis:** AI-produced review claims, themes, or references cannot be traced to visible papers, notes, abstracts, or retrieved sources. Hand off to `references/ai-assisted-source-work-quality.md`.

## Compact paragraph motifs

Use these as reasoning skeletons, not phrase banks.

| Motif | Skeleton |
|---|---|
| Topic-to-field | Establish why the topic matters, then narrow to the field conversation. |
| Trend synthesis | Name the pattern across several studies, then cite grouped evidence and explain what the pattern shows. |
| Consensus | Identify where studies agree, specify the shared conclusion, and state why it matters for the user's study. |
| Tension/debate | Contrast findings or interpretations, then identify what remains unresolved. |
| Method critique | Describe dominant methods, what they reveal, and what they leave unanswered. |
| Context/population shift | Show where evidence is concentrated and why another setting or group may require study. |
| Theory lens | State how a theory explains the phenomenon and where it may be limited or contested. |
| Gap transition | Move from known pattern -> missing piece -> consequence -> present study response. |
| Section synthesis | Close a section by naming the accumulated insight and linking it to the next section. |

## Output selector

| User asks for | Produce | Include |
|---|---|---|
| "Organize my literature" | Theme map | Themes, source clusters, debates, methods, theories, gap relevance. |
| "Compare papers" | Synthesis matrix | Study, context, method, theory, findings, limitations, relation to other studies. |
| "Build the review" | Review architecture | Section order, purpose of each section, evidence needed, gap bridge. |
| "Write a paragraph" | Paragraph motif skeleton | Synthesis claim, grouped evidence slots, evaluation move, transition. |
| "Check my claims" | Claim-evidence map | Claim, supporting sources, strength, missing support, revision action. |
| "Fix my review" | Revision audit | Summary-vs-synthesis issues, structure gaps, missing debates, weak transitions. |

## Handoffs

- Use `references/cluster-gap-problem.md` when the review lacks a clear gap, uses absence-only novelty, or needs RQ/aim/problem alignment.
- Use `references/ai-assisted-source-work-quality.md` when AI assistance, citation reliability, source visibility, disclosure/compliance awareness, or submission defensibility is part of the literature-review task.
- Use `references/cluster-front-end-proposal.md` when the literature material must be compressed into a concept paper, proposal, Chapter 1, specific-aims-like page, qual proposal, or supervisor memo.
- Use `references/manuscript-and-results.md` when the review/background must align with the full manuscript's aim, methods, Results, and Introduction.
- Use `references/peer-review-revision.md` when the user is avoiding reviewer red flags or responding to comments that the review is a list, outdated, unsynthesized, or missing key literature.
- Use `references/language-and-outreach.md` for academic phrasing, hedging, transitions, and outreach only after the review's source logic is sound.
