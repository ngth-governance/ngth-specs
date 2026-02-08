# Skill Declaration Decision Rules

This document defines when a capability **MUST** be implemented as a
declared skill within NGTH systems.

The objective is to prevent opaque or non-attributable intelligence
in public governance contexts.

---

## Prohibition of Opaque Intelligence

NGTH does not permit opaque or non-attributable intelligence in any
public governance context.

Any capability that is reusable, error-prone, auditable, or replaceable
**MUST** be implemented as a declared skill with:

- Explicit input and output interfaces
- Documented constraints and limitations
- Traceable evidence and data references
- Clear responsibility attribution

This requirement exists to prevent black-box decision-making and to
ensure accountability, auditability, and public trust.

---

## Skill Declaration Decision Gate

A capability **MUST** be implemented as a declared skill if it satisfies
**any two or more** of the following conditions:

1. **Cross-domain reuse**  
   Used across multiple governance domains (e.g. health, education,
   transport, safety)

2. **Auditability or accountability requirements**  
   Subject to public explanation, legislative inquiry, or oversight review

3. **Expected iteration or evolution**  
   Likely to change due to model updates, methodological revisions, or
   threshold adjustments

4. **Replaceability requirements**  
   Intended to support multiple vendors, jurisdictions, or implementations

5. **High-risk or high-impact outputs**  
   Outputs that may influence public interpretation, media coverage,
   or political discourse

6. **Benchmarking or comparative evaluation requirements**  
   Participation in public KPIs, performance comparison, or transparent
   evaluation

---

## Non-Skill Capabilities

The following are **not** required to be implemented as skills:

- User interface rendering and presentation
- Data ingestion pipelines and storage layers
- Deterministic rule execution and state machines
- Legally mandated approval or publication workflows
- Simple query or CRUD APIs without interpretive logic

These capabilities are considered platform infrastructure rather than
governance intelligence.

---

## Normative Status

This document is normative.

All NGTH implementations and integrations **MUST** comply with these
rules when designing or deploying intelligent capabilities.
