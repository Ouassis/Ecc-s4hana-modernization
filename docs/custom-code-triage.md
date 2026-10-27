# Custom code triage

## Triage dimensions

Evaluate each custom object using evidence and agreed scoring definitions.

| Dimension | Questions |
|---|---|
| Business criticality | What process fails if this object is unavailable? |
| Usage | Is there reliable evidence it is used, and during which period? |
| Technical findings | What ATC, simplification, API, or data-model findings apply? |
| Dependency | Which jobs, interfaces, enhancements, and downstream processes depend on it? |
| Remediation effort | What change and test effort is expected, with what uncertainty? |
| Strategic fit | Should the capability remain custom, use standard SAP, or be redesigned? |

## Suggested decision categories

- **Retire:** usage and owner review support removal or archival.
- **Keep / validate:** no known blocker, but critical paths still need regression evidence.
- **Remediate:** targeted changes can resolve findings while preserving behavior.
- **Redesign:** architecture or API assumptions need replacement.
- **Replace with standard:** a standard capability can meet the requirement after fit-gap validation.
- **Risk accepted:** accountable owner records impact, mitigation, and review date.

## Example scoring rubric

Use a 1–5 scale only after agreeing definitions with stakeholders. Keep business criticality separate from technical complexity so a high-risk but small change is not deprioritized.

A useful prioritization score can combine criticality, usage confidence, technical severity, dependency breadth, and effort. Document weights, score rationale, and confidence. Avoid treating a numeric score as an automatic go/no-go decision.

## Triage output

For every object, record:
- technical name and type
- package/component and owner
- usage evidence and confidence
- relevant finding references
- dependent processes/interfaces
- proposed decision and rationale
- effort estimate and confidence
- test strategy and acceptance owner
- status, blocker, and next action
