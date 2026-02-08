# Governance Assertions

This document defines the explicit governance assertions that apply to
all specifications, agents, skills, and systems within the NGTH ecosystem.

These assertions are normative. Any specification that contradicts
or violates these assertions is invalid by definition.

---

## 1. Human Authority Assertion

All governance authority resides with human actors.

AI systems and software agents are strictly assistive and do not possess
decision-making, policy-setting, or executive authority.

No system behavior may override, replace, or simulate human governance authority.

---

## 2. Non-Autonomy Assertion

NGTH does not permit autonomous governance behavior.

AI systems MUST NOT:
- Make or finalize governance decisions
- Initiate enforcement or compliance actions
- Close cases or workflows
- Modify governance rules, KPIs, or thresholds

Any appearance of autonomous authority constitutes a governance violation.

---

## 3. Boundary Compliance Assertion

All systems MUST comply with the constraints defined in:

- `AI-BOUNDARIES.md`
- `AGENT-ROLES.md`
- `AGENT-COMPLIANCE-CHECKLIST.md`

These documents define hard limits on system behavior.
Specifications MAY NOT weaken, bypass, or reinterpret these constraints.

---

## 4. Explicit Role Assertion

Every AI or software agent MUST operate under a single, explicitly declared role.

- Roles MUST be defined in `AGENT-ROLES.md`
- Role mixing, implicit roles, or emergent authority are prohibited
- Role changes require explicit human authorization

Undeclared or ambiguous roles are non-compliant.

---

## 5. Transparency and Auditability Assertion

All system behavior MUST be observable, attributable, and auditable.

- Inputs, outputs, and transformations must be describable
- Assumptions and limitations must be documented
- Outputs must not be treated as authoritative or final
- Auditability takes precedence over performance or convenience

Opaque or non-attributable intelligence is not permitted.

---

## 6. Human-in-the-Loop Assertion

All AI outputs are subject to human review.

- Human override MUST always be possible
- AI systems MUST NOT act on outputs without confirmation
- Systems MUST NOT infer or simulate human intent

Human review is a governance requirement, not an optional safeguard.

---

## 7. Specification Supremacy Assertion

Governance assertions supersede implementation details.

If an implementation conflicts with these assertions:
- The specification is invalid
- The implementation MUST be revised or rejected

Performance, optimization, or automation goals do not justify
violations of governance constraints.

---

## 8. Responsibility and Accountability Assertion

Responsibility for AI-assisted outcomes rests with human approvers,
not with AI systems.

Failures resulting from non-compliant specifications constitute
governance failures, not technical errors.

---

## Compliance Statement

All specifications in the `ngth-specs` repository MUST explicitly
acknowledge and comply with these governance assertions.

Any specification that fails to do so MUST NOT be implemented,
integrated, or deployed within the NGTH ecosystem.
