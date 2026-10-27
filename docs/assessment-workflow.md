# Assessment workflow

## Phase 1 — Scope and baseline
- Identify source ECC release, enhancement packages, database, Unicode status, add-ons, and business scope.
- Identify target S/4HANA release and deployment model.
- Assign owners for platform, custom code, integrations, security, data, and business processes.
- Capture sandbox, system-copy, backup, and recovery assumptions.

**Evidence:** approved scope, source/target baseline, responsibilities, and known constraints.

## Phase 2 — Discovery and usage
- Inventory custom namespaces, packages, reports, enhancements, interfaces, forms, jobs, and modifications.
- Identify active usage with approved usage data where available.
- Map custom objects to business capabilities and process owners.
- Identify integrations, batch windows, high-volume objects, and critical flows.

**Evidence:** inventory with ownership, usage confidence, and business criticality.

## Phase 3 — Technical assessment
- Run applicable ATC checks with a target-appropriate variant.
- Review relevant Simplification Items for the source/target release combination.
- Assess add-on and custom-object compatibility.
- Inspect interfaces, obsolete APIs, data-model assumptions, and authorization behavior.
- Separate confirmed findings from hypotheses requiring proof.

**Evidence:** finding references, triage decisions, and open questions.

## Phase 4 — Prioritization
Typical decisions: retire/archive, keep after validation, remediate, redesign, replace with standard functionality, or defer with formal risk acceptance.

Score transparently using business criticality, usage, technical severity, dependency impact, and effort. Do not let a numeric score replace accountable review.

## Phase 5 — Remediation and regression
- Implement through approved development and transport processes.
- Run syntax checks, ATC, unit tests, and interface tests.
- Execute business regression for affected end-to-end processes.
- Validate performance and authorization where runtime behavior changes.

**Evidence:** test results, code review, transport references, and accepted defects.

## Phase 6 — Cutover readiness
- Rehearse technical conversion and business cutover.
- Validate reconciliation, integrations, batch scheduling, monitoring, and support.
- Agree go/no-go criteria, recovery strategy, and business sign-off.

Do not mark an object compatible based only on syntax checks. Record target release, evidence, tested path, known limitations, and reviewer.
