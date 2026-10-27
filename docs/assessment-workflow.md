# Assessment workflow

## Phase 1 — Scope and baseline

- Identify source ECC release, enhancement packages, database, Unicode status, add-ons, and relevant business scope.
- Identify target S/4HANA release and deployment model.
- Establish owners for technical platform, custom code, integrations, security, data, and business processes.
- Capture backup, sandbox, and system-copy assumptions.

**Evidence:** approved scope, source/target baseline, responsibility matrix, and known constraints.

## Phase 2 — Discovery and usage

- Inventory custom namespaces, packages, reports, enhancements, interfaces, forms, jobs, and modifications.
- Identify active usage with approved usage data where available.
- Map custom objects to business capabilities and process owners.
- Identify integrations, batch windows, high-volume objects, and critical business flows.

**Evidence:** inventory with ownership, usage confidence, and business criticality.

## Phase 3 — Technical assessment

- Run applicable ATC checks using a variant suitable for the chosen target.
- Review relevant Simplification Items for the source/target release combination.
- Assess add-on and custom-object compatibility.
- Inspect interfaces, obsolete APIs, data model assumptions, and authorization behavior.
- Separate confirmed findings from hypotheses requiring proof.

**Evidence:** finding exports or references, triage decisions, and open questions.

## Phase 4 — Prioritization

Score each object using business criticality, technical risk, usage, remediation effort, and dependency impact. Keep the scoring method transparent and adjustable.

Typical decisions:
- retire or archive
- keep with no change after validation
- adapt or remediate
- redesign using released APIs or supported extension points
- replace with standard functionality
- defer with explicit risk acceptance

**Evidence:** reviewed remediation backlog and accountable owners.

## Phase 5 — Remediation and regression

- Implement in development using approved transport and code review processes.
- Run syntax checks, ATC, unit tests, and interface tests.
- Execute business regression for affected end-to-end processes.
- Validate performance and authorization where changes affect runtime behavior.

**Evidence:** test results, code review, transport references, and accepted defects.

## Phase 6 — Cutover readiness

- Rehearse technical conversion and business cutover.
- Validate data reconciliation, integrations, batch scheduling, monitoring, and support.
- Agree go/no-go criteria, rollback or recovery strategy, and business sign-off.

**Evidence:** rehearsal results, signed checklist, issue disposition, and support plan.

## Governance

Do not mark an object "S/4HANA compatible" based only on successful syntax checks. Record evidence, target release, tested path, known limitations, and the responsible reviewer.
