# Clean Core and extension strategy

## Goal
Reduce unnecessary coupling to SAP internals and improve upgradeability. The right strategy depends on target release, released APIs, deployment model, and business requirements.

## Review questions
- Does standard SAP functionality already meet the requirement?
- Does the custom implementation use released APIs and supported extension points?
- Does it depend on direct table updates, unreleased function modules, internal classes, or assumptions about standard data?
- Could a supported in-app or side-by-side extension meet the requirement?
- What are the consistency, latency, security, and operational implications?
- Is the object still used and owned by a business process?

## Candidate paths
- Retire redundant or unused functionality after usage and owner validation.
- Adopt standard functionality after fit-gap and regression analysis.
- Adapt custom ABAP code to supported APIs and target data models.
- Use supported enhancement techniques where in-stack extension is appropriate.
- Consider side-by-side extension for decoupled capabilities when justified.

Do not recommend cloud or side-by-side architecture by default. Evaluate total complexity, integration failure modes, security, and lifecycle ownership.

## Governance
Record target release, API release status, ATC findings, tests, design rationale, and reviewer. Re-check assumptions when the target release or architecture changes.
