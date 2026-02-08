# NGTH Specifications

This repository contains the **technical and governance specifications**
used by the National Governance Transparency Hub (NGTH) and its core
platform, the Public Accountability & Performance Platform (PAPP).

The specifications defined here govern how capabilities are structured,
declared, audited, and benchmarked within NGTH systems.

---

## Scope

This repository defines standards for:

- Declared skills and capability boundaries
- Skill interfaces and evidence requirements
- Auditability and attribution rules
- Benchmarking and comparative evaluation
- Technical governance constraints for public-interest intelligence

These specifications are designed to be:
- Public by default
- Politically neutral
- Jurisdiction-agnostic
- Implementable by multiple vendors or institutions

---

## Design Principle

NGTH prohibits opaque intelligence in public governance systems.

Capabilities that require reuse, auditability, or replacement are
implemented as declared skills with explicit interfaces and evidence.

---

## Structure

- `skills/`
  - Skill declaration rules
  - Skill interface contracts
  - Skill governance constraints

Additional directories may be introduced as specifications evolve.

---

## Relationship to Other Repositories

- **ngth-charter**  
  Defines institutional purpose, public-interest principles, and governance
  boundaries.

- **ngth-specs** (this repository)  
  Defines how those principles are implemented in technical and operational
  systems.

If any conflict arises, the charter prevails over specifications.

---

## License

This repository is licensed under the **Apache License 2.0**.
