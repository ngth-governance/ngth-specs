# Skill Contract v1.0

This document defines the **mandatory interface and governance contract**
for all declared skills used within NGTH and PAPP systems.

A skill is a bounded, auditable capability that produces structured outputs
without holding decision authority.

This contract exists to ensure transparency, accountability, replaceability,
and public trust.

---

## Normative Language

The key words **MUST**, **SHOULD**, and **MAY** in this document are to be
interpreted as described in RFC 2119.

---

## Definition of a Skill

A declared skill:

- Performs a clearly defined capability
- Accepts structured inputs
- Produces structured outputs
- Provides traceable evidence
- Operates without executive or policy authority

A skill **MUST NOT** make final decisions or close governance actions.

---

## Skill Identification

Each skill **MUST** be uniquely identified by:

- `skill_id` — stable, namespaced identifier  
  (e.g. `observe.kpi_monitor`)
- `skill_version` — semantic version  
  (e.g. `1.0.0`)

Skill versions **MUST** be immutable once released.

---

## Skill Request (Input Contract)

A skill **MUST** accept a request containing the following fields:

### Required Fields

- `task_id`  
  Unique identifier for the governance task or case

- `skill_id`  
  Identifier of the invoked skill

- `skill_version`  
  Version of the skill implementation

- `jurisdiction`  
  Applicable governance scope  
  (e.g. state, city, district)

- `domain`  
  Governance domain  
  (e.g. health, education, transport, safety)

- `inputs`  
  References to data snapshots, indicators, or documents

- `constraints`  
  Explicit limitations including:
  - policy neutrality
  - data sensitivity
  - prohibited actions

- `output_spec`  
  Required output structure and format

---

## Skill Response (Output Contract)

A skill **MUST** return a response containing:

### Required Fields

- `task_id`
- `skill_id`
- `skill_version`
- `outputs`  
  Structured results defined by the skill type

- `confidence`  
  Declared confidence level or range

- `evidence[]`  
  One or more evidence objects supporting the outputs

- `audit`  
  Metadata required for traceability and reproducibility

- `safety`  
  Explicit statements of limitations, uncertainty, and compliance

---

## Evidence Requirements

Each evidence object **MUST** include:

- `source_type`  
  (e.g. KPI snapshot, public report, dataset, policy document)

- `source_ref`  
  URI, identifier, or reference pointer

- `timestamp`

- `extract`  
  Relevant fields, sections, or excerpts

- `integrity` (SHOULD)  
  Hash or signature for verification

Evidence **MUST** be sufficient for an independent reviewer to
understand the basis of the output.

---

## Audit Metadata

The `audit` object **MUST** include:

- Model or method identifier
- Version or configuration reference
- Data snapshot identifier or hash
- Generation timestamp

This information **MUST NOT** be omitted or obscured.

---

## Authority and Responsibility

- Skills **MUST NOT**:
  - Make policy decisions
  - Approve or reject actions
  - Trigger enforcement or sanctions
  - Generate political or persuasive messaging

- Skills **MAY**:
  - Describe observations
  - Explain patterns or correlations
  - Propose options with constraints
  - Simulate potential impacts

Responsibility for action remains with human authorities.

---

## Failure and Uncertainty Handling

Skills **MUST** explicitly signal:

- Data insufficiency
- Low confidence conditions
- Methodological limitations
- Potential sources of bias

Silent failure or overconfident output is prohibited.

---

## Benchmark Compatibility

All skills **MUST** be designed to support:

- Unit-level testing
- Comparative benchmarking
- Independent reimplementation

Benchmarking criteria are defined separately.

---

## Versioning and Evolution

This contract defines **v1.0**.

Backward-incompatible changes **MUST** increment the major version.

All implementations **MUST** declare the contract version they comply with.

---

## Normative Status

This document is normative.

All declared skills within NGTH and PAPP systems **MUST** comply with this
contract unless explicitly exempted by published specification.
