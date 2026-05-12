# Research Thinking Writing Coworker

This repository is the public staging repo for a Codex/ChatGPT skill named `research-thinking-writing-coworker`.

The skill is intended to help with research-thinking and research-writing work: idea development, gap and problem-statement logic, literature-review construction, proposal/front-end framing, manuscript alignment, Results/Discussion/Conclusion support, reviewer-response planning, academic reasoning-language, high-level meta-analysis planning, and concise research outreach.

This repo is the staged development package, not the live installed `CODEX_HOME` copy. The installed runtime copy should contain the skill package files needed by Codex, not local workspace review notes or prompt-design artifacts.

## Package Layout

- `SKILL.md` is the runtime entrypoint.
- `agents/openai.yaml` contains UI-facing skill metadata.
- `references/` contains runtime reference files loaded selectively by the skill.

## Current Status

The package is structurally valid and ready for provisional review/testing. It should not yet be treated as a mature or final skill until behavior testing and review-driven patching are complete.

## Boundary

The skill should behave as a critical research coworker, not as a generic grammar editor or phrase bank. It should diagnose weak research logic before polishing prose, avoid fabricating sources or current facts, and distinguish runtime transfer from source-local claims when that distinction matters.
