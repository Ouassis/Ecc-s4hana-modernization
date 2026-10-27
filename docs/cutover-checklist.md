# Cutover and recovery checklist

Tailor this checklist to the selected SAP conversion method, landscape, and business calendar. It is not a substitute for the official procedure for the target release.

## Before rehearsal
- [ ] Approved cutover plan, timeline, and responsibility matrix.
- [ ] Source/target release and add-on compatibility confirmed.
- [ ] Backup, recovery, and rollback/restart assumptions documented.
- [ ] Critical interfaces, batch jobs, certificates, and technical users inventoried.
- [ ] Data reconciliation rules and expected totals agreed.
- [ ] Monitoring, escalation, and support coverage assigned.

## During rehearsal
- [ ] Record actual durations for each step.
- [ ] Capture warnings, errors, manual actions, and dependencies.
- [ ] Validate key business transactions and reconciliations.
- [ ] Verify integrations, queues, batch jobs, output, and authorizations.
- [ ] Test recovery procedures where safe and supported.
- [ ] Track deviations with owners and due dates.

## Go/no-go review
- [ ] Critical business flows pass agreed acceptance tests.
- [ ] Reconciliation differences are explained and approved.
- [ ] Critical incidents are resolved or formally accepted.
- [ ] Operations dashboards and alerts are active.
- [ ] Business, technical, and support owners sign off.

## Recovery planning
Document the supported recovery path for the selected conversion method. Do not assume rollback is a simple database restore or that the old system can resume without reconciliation. Define data divergence handling, interface suspension/resumption, and decision authority.

## After go-live
- [ ] Monitor critical jobs, interfaces, queues, and business KPIs.
- [ ] Reconcile key business objects and totals.
- [ ] Track hypercare incidents and known limitations.
- [ ] Review accepted risks and transition to steady-state support.
