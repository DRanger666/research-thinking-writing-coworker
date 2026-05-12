# Source Provenance Map

## When to load

Load this file when the user asks what the KB actually supports, when a task risks overclaiming source authority, or when source-local content must be separated from runtime transfer.

The installed runtime skill does not carry the full canonical v12 KB. Use this file as a compact provenance and caveat map. If a deep audit of original post wording is needed, inspect the canonical KB only if it is available in the workspace or supplied by the user.

## Runtime provenance rule

Keep four layers separate:

1. **Source-local content:** a post's own stated advice, examples, caveats, and visible limitations.
2. **User calibration:** explicit user guidance during curation that corrected or sharpened how a post should be treated.
3. **KB synthesis:** cluster membership, cross-post routing, and special-role interpretation created during curation.
4. **Runtime transfer:** using a post or cluster outside its source-local genre because the reasoning move is useful for the user's task.

Runtime transfer is allowed, but do not present it as if the original post explicitly named that target genre. Label the transfer only when the distinction matters for the user's decision, the task is high-stakes, or the user asks about source support.

When provenance matters, use compact labels: `source-local`, `user-calibrated`, `KB synthesis`, and `runtime transfer`. Do not clutter ordinary drafting with these labels.

## Calibration-sensitive items

| Resource | Calibration to preserve |
|---|---|
| P001/P009 | Treat as thinking-through-writing and reasoning-language resources, not mere polish or decorative phrasing. |
| P003 | Treat as a broad research-thinking heuristic for generating candidate routes, not a proof that a gap exists. |
| P006 | Treat as multi-role findings language: Results, preliminary data, combined Results/Discussion contexts, and Discussion-adjacent interpretation. Do not collapse it into the Discussion cluster. |
| P011 | Treat literature-review motifs as argument moves and local paragraph logic, not as a phrase bank. |
| P026 | Transfer by content-level front-end audit logic beyond thesis contexts when appropriate; do not present that transfer as source-local genre coverage. |

## Compact caveat table

| Resource | Caveat to preserve |
|---|---|
| P003 | Gap-search routes are candidate-generation routes, not proof that a gap exists. |
| P013 | Source coverage was partial in v12; use as an operational runtime search-loop scaffold, not source-local proof of a complete research-methods guide. |
| P014 | Manuscript-derived evidence extraction, not a slide transcript. Use as a manuscript-wide hub and publication-readiness integrator, not as exact post wording, journal-rule authority, or a replacement for section-specific references. |
| P016 | Supports AI/LLM-assisted literature interrogation and refinement; not authority to fabricate synthesis without supplied source material. |
| P018 | High-level meta-analysis / quantitative evidence-synthesis workflow only; not universal methods, statistics, PRISMA, software, or risk-of-bias authority. |
| P020 | Gap taxonomy is an operational runtime scaffold and is useful for triage, but preserve the v12 caveat about a likely inconsistency in the theoretical-gap row. |
| P024 | Reviewer-lens problem-statement guidance should be used as an audit lens, not as proof of a complete source transcript. |
| P026 | Transfers by content-level front-end audit logic, not as a rigid Chapter 1 template outside thesis contexts. |
| P010 | Outreach is person-to-person and fit-based; do not turn it into manuscript/proposal architecture. |
| P006 | Results-and-Discussion local findings language is adjacent to Discussion but not inside the Discussion cluster. |

## Reference support map

| Reference | Main source base | Runtime support level |
|---|---|---|
| `cluster-gap-problem.md` | P003/P020/P022/P024/P013/P017/P015 | Strong for gap/problem/RQ/aim logic; provisional until source evidence is supplied for a specific field claim. |
| `cluster-literature-review.md` | P012/P002/P011/P016 | Strong for review architecture and AI-assisted source interrogation; requires supplied/retrieved sources for literature claims. |
| `cluster-front-end-proposal.md` | P005/P007/P026 | Strong for proposal/front-end packaging; genre requirements and funder rules must be supplied or retrieved. |
| `manuscript-and-results.md` | P014/P006 | Strong for manuscript alignment and Results/preliminary-data communication; journal-specific rules are external. |
| `discussion-conclusion.md` | P004/P021/P019/P008 | Strong for Discussion, unexpected results, limitations, implications, and Conclusion architecture. |
| `peer-review-revision.md` | P023/P025 | Strong for reviewer-risk audit and revision-response planning; response locations must come from the actual revised manuscript. |
| `language-and-outreach.md` | P001/P009/P010 | Strong for reasoning-language and outreach structure; recipient-specific fit requires supplied or retrieved current evidence. |
| `method-fit-triage.md` | Runtime transfer from gap/problem, proposal/front-end, manuscript alignment, and P018 boundary logic | Partial support for high-level RQ/aim/evidence/design-family alignment; detailed protocol/statistics require external standards or expertise. |
| `method-meta-analysis.md` | P018 | Partial support for high-level meta-analysis planning; detailed technical methods need external standards or expertise. |

## Current-source rule

When the user asks for current papers, latest evidence, journal rules, reporting-standard compliance, professor/lab fit, job openings, software capability, or any time-sensitive fact, use supplied material or retrieve current sources when tools are available and not explicitly disallowed. If retrieval is unavailable or forbidden, produce a source-acquisition plan rather than a factual claim.
