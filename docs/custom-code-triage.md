# Custom code triage

## Triage dimensions

| Dimension | Questions |
|---|---|
| Business criticality | What process fails if this object is unavailable? |
| Usage | Is there reliable evidence it is used, and during which period? |
| Technical findings | What ATC, simplification, API, or data-model findings apply? |
| Dependency | Which jobs, interfaces, enhancements, and processes depend on it? |
| Remediation effort | What change and test effort is expected, with what uncertainty? |
| Strategic fit | Keep custom, use standard SAP, or redesign? |

## Suggested decisions
- **Retire:** usage and owner review support removal or archival.
- **Keep / validate:** no known blocker, but critical paths still need regression evidence.
- **Remediate:** targeted changes can resolve findings while preserving behavior.
- **Redesign:** architecture or API assumptions need replacement.
- **Replace with standard:** a standard capability meets the requirement after fit-gap validation.
- **Risk accepted:** accountable owner records impact, mitigation, and review date.

## Scoring
Use a 1–5 scale only after agreeing definitions with stakeholders. Keep business criticality separate from technical complexity. Document weights, rationale, confidence, and owner; the score is not an automatic go/no-go decision.

## Triage output
Record technical name/type, package, owner, business process, usage evidence, finding references, dependencies, proposed decision, rationale, effort/confidence, test strategy, status, and next action.
