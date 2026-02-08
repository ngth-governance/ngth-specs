# Agent Orchestration Boundary v1.0

This document defines the **mandatory boundaries and constraints**
for agent orchestration within NGTH and PAPP systems.

Agents may coordinate skills and information flow, but they do not
possess authority, intent, or decision rights.

---

## Definition of an Agent

Within NGTH systems, an agent is defined as:

- A coordinating entity that sequences tasks
- A consumer and integrator of declared skill outputs
- A facilitator of human understanding

An agent is **not** a decision-making authority.

---

## Permitted Agent Functions

Agents **MAY** perform the following functions:

1. **Skill Orchestration**
   - Invoke multiple declared skills
   - Sequence skill execution
   - Route inputs and outputs between skills

2. **Aggregation**
   - Combine multiple skill outputs
   - Align results across domains or time windows
   - Normalize outputs for comparison

3. **Explanation and Summarization**
   - Summarize skill outputs
   - Translate technical results into plain language
   - Explain observed patterns and constraints

4. **Option Framing (Non-Prescriptive)**
   - Present multiple possible interpretations
   - Describe trade-offs and uncertainties
   - Explicitly state that no recommendation is made

---

## Prohibited Agent Functions

Agents **MUST NOT** perform any of the following:

- Make policy recommendations
- Select or endorse a preferred option
- Approve or reject actions
- Trigger enforcement, allocation, or sanctions
- Persuade, advocate, or influence political outcomes
- Override or suppress skill outputs
- Generate conclusions without cited skill evidence

Any attempt to bypass these constraints constitutes a violation of NGTH
governance principles.

---

## Evidence and Attribution Requirements

All agent-generated outputs **MUST**:

- Reference the underlying skill identifiers and versions
- Preserve evidence links provided by skills
- Maintain traceability to original data sources

Agents MUST NOT introduce new evidence or inference beyond what is
explicitly supported by invoked skills.

---

## Confidence and Uncertainty Handling

Agents **MUST**:

- Propagate uncertainty signals from skills
- Avoid artificial confidence amplification
- Clearly state when outputs are inconclusive

If constituent skill outputs conflict, the agent MUST surface the
disagreement explicitly.

---

## Human Authority Boundary

Agents **MUST** terminate their operation when:

- A policy choice is required
- A legal or ethical judgment is needed
- Trade-offs require value-based prioritization
- Accountability cannot be algorithmically resolved

At these boundaries, responsibility transitions to designated
human authorities.

---

## Public Disclosure Constraints

Any agent output intended for public release MUST comply with:

- Public Disclosure Schema v1.0
- KPI Schema v1.0 (where applicable)
- Skill Benchmark Rubric v1.0

Agents MUST NOT generate public disclosures independently of these rules.

---

## Replaceability and Auditability

Agent implementations MUST be:

- Replaceable without changing governance outcomes
- Auditable through recorded orchestration steps
- Reproducible in principle by independent reviewers

Opaque or non-reproducible agent behavior is prohibited.

---

## Normative Status

This document is normative.

All agents operating within NGTH and PAPP systems MUST comply with
these orchestration boundaries.
