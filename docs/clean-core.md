# Clean Core and extension strategy

## Goal

Reduce unnecessary coupling to SAP internals and improve upgradeability. The right strategy depends on the target release, available released APIs, deployment model, and business requirements.

## Review questions

- Does standard SAP functionality already meet the requirement?
- Is the custom implementation using released APIs and supported extension points?
- Does it depend on direct table updates, unreleased function modules, internal classes, or implicit assumptions about standard data?
- Can the requirement be implemented with a supported in-app or side-by-side extension?
- What are the data consistency, latency, security, and operational implications?
- Is the custom object still used and owned by a business process?

## Candidate modernization paths

- Retire redundant or unused custom functionality after usage and owner validation.
- Adopt standard functionality after fit-gap and regression analysis.
- Adapt custom ABAP code to supported APIs and target data models.
- Use supported enhancement techniques where in-stack extension is appropriate.
- Consider side-by-side extension for decoupled capabilities when justified by requirements and platform fit.

Do not recommend a side-by-side or cloud architecture by default. Evaluate total complexity, integration failure modes, security, and lifecycle ownership.

## Evidence and governance

For each decision record the target release, API release status, ATC findings, tests performed, design rationale, and reviewer. Re-check assumptions when the target release or architecture changes.
