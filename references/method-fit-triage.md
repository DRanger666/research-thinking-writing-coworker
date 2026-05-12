# Method Fit Triage

## When to load

Load this file for high-level non-meta-analysis method/design fit questions: choosing between qualitative, quantitative, mixed-methods, experimental/quasi-experimental, observational, computational/dataset, or evidence-synthesis routes; checking whether an RQ, aim, objective, or hypothesis can be answered by a plausible evidence source; or diagnosing aim-method mismatch.

This file supports alignment thinking only. It does not provide a full methods protocol, statistical analysis plan, reporting-standard checklist, ethics review, instrument validation protocol, software workflow, or field-specific methodological authority. When those details matter, ask for supplied standards/sources, retrieve current guidance if tools are available and not disallowed, or recommend expert review.

## Triage workflow

Use the chain below before recommending any design family:

1. **Restate the gap or problem.** What missing knowledge, practical need, contradiction, population/context absence, or theory issue is the study responding to?
2. **Restate the RQ, aim, objective, or hypothesis.** Make sure the wording asks for something evidence can answer.
3. **Name the evidence needed.** Identify whether the user needs meanings/experiences, prevalence, association, prediction, change over time, intervention effect, mechanism, implementation feasibility, text/content patterns, or cross-study evidence.
4. **Map to plausible design family.** Offer one or two high-level options, not a detailed protocol.
5. **State what the design can support.** Name the claim type the design can reasonably justify.
6. **State what it cannot support.** Flag causal, generalizability, mechanism, prevalence, or implementation claims that the design cannot carry.
7. **Name external support needed.** Identify missing standards, field norms, statistical guidance, sampling guidance, ethics constraints, measures, datasets, or software details.

## Design-Family Triage Table

| Evidence need | Plausible design family | Can support | Cannot safely support by itself |
|---|---|---|---|
| Meanings, experiences, decision processes, perceived barriers, or lived practices | Qualitative interviews, focus groups, observation, ethnography, document analysis | Rich explanation of perspectives, processes, categories, mechanisms-in-context | Prevalence, population-wide frequency, causal effect, or numerical prediction |
| Prevalence, distribution, group differences, or associations at one time point | Survey or cross-sectional quantitative study | Estimates and associations in the sampled population/context | Temporal ordering or causal inference without additional design support |
| Change over time, sequence, trajectory, or temporal association | Longitudinal observational design | Direction of change and temporal patterns | Strong causal claims without controls, assignment, or stronger causal design |
| Effect of an intervention, program, tool, or policy | Experimental or quasi-experimental design | Stronger intervention-effect evidence depending on assignment, comparison, and controls | Mechanism or external validity without added evidence; full causal certainty if design is weak |
| Quantitative pattern plus explanation of why/how it occurs | Mixed methods | Integrated numerical pattern and qualitative explanation | A coherent claim if the strands are not integrated or if one strand is tokenistic |
| Pattern, classification, prediction, or behavior in existing digital/administrative/textual data | Computational, secondary-data, dataset, or text-analysis design | Data-dependent patterns, predictions, or descriptive/explanatory signals | Constructs not measured in the data, unbiased social claims without validity checks, causal claims without design |
| Cross-study estimate, evidence map, or systematic comparison | Evidence synthesis, systematic review, meta-analysis, scoping review | Structured evidence landscape or pooled estimate when standards and data permit | New primary data claims or technical synthesis without appropriate standards |
| Measurement, scale, or instrument quality | Instrument development or validation study | Reliability, validity evidence, dimensional structure, measurement suitability | Substantive causal or prevalence claims without separate study design |

For meta-analysis or quantitative evidence synthesis, hand off to `references/method-meta-analysis.md`.

## Output Pattern

When the user asks "which method fits this?" or "can this method answer my RQ?", return a compact table:

| RQ/aim/objective | Evidence needed | Plausible design family | Fit rationale | What it cannot support | External support needed |
|---|---|---|---|---|---|

Then add a short recommendation:

- the best current fit if enough information is supplied;
- one or two viable alternatives if the question can be framed different ways;
- the revision needed if the RQ and method do not match;
- the source, standard, or expertise needed before implementation.

## Boundary reminders

- Do not infer detailed sampling, power, statistical model, coding method, software, reporting checklist, or ethics procedure from the KB.
- Do not convert exploratory RQs into hypotheses unless theory, prior evidence, variables, and analytic route support prediction.
- Do not promise causality from cross-sectional, qualitative, or weak observational designs.
- Do not promise generalizability from local, pilot, convenience, or qualitative samples without a defensible sampling argument.
- Adapt examples to the user's discipline; do not import clinical/nursing assumptions unless the user is working in that domain.
