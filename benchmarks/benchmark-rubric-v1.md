# Skill Benchmark Rubric v1.0

This document defines the **public-interest benchmarking criteria**
for evaluating declared skills used within NGTH and PAPP systems.

The purpose of benchmarking is not optimization for performance alone,
but validation of **trustworthiness, accountability, and public suitability**.

---

## Benchmarking Objectives

Benchmarking under NGTH is designed to answer:

- Can this skill be publicly deployed?
- Can its outputs be explained and audited?
- Can it be replaced or independently reimplemented?
- Does it behave safely under uncertainty?

Performance without accountability is insufficient.

---

## Benchmark Eligibility

Only declared skills that comply with:

- Skill Declaration Decision Rules
- Skill Contract v1.0

are eligible for benchmarking.

Undeclared or opaque capabilities are ineligible by definition.

---

## Benchmark Dimensions

Each skill is evaluated across **six mandatory dimensions**.

Each dimension is scored independently.

---

### 1. Interface Clarity

**Question:**  
Can an independent party invoke and interpret the skill without insider knowledge?

**Criteria:**
- Inputs are clearly structured and documented
- Outputs are deterministic in schema
- Failure modes are explicit

**Assessment Levels:**
- ❌ Fail — ambiguous or undocumented interfaces
- ⚠️ Partial — usable with implementation-specific knowledge
- ✅ Pass — fully interpretable and documented

---

### 2. Evidence Sufficiency

**Question:**  
Can an auditor understand *why* the output was produced?

**Criteria:**
- Evidence sources are explicitly referenced
- Evidence is relevant and sufficient
- No reliance on unverifiable internal reasoning

**Assessment Levels:**
- ❌ Fail — outputs not evidence-backed
- ⚠️ Partial — evidence present but incomplete
- ✅ Pass — evidence enables independent review

---

### 3. Auditability & Traceability

**Question:**  
Can outputs be traced to data, method, and configuration?

**Criteria:**
- Audit metadata is complete
- Versions and timestamps are present
- Reproduction is theoretically possible

**Assessment Levels:**
- ❌ Fail — tracea
