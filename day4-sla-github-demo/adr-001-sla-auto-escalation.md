# ADR 001: Trigger SLA Escalation Only Once Per Case

## Decision
Repeated SLA breach on the same case triggers escalation only once.

## Why
Repeated triggers could create duplicate escalation events and confuse the support workflow.

## Trade-off
If the case remains unresolved, later SLA breach checks will not trigger a second escalation in this version.

## Consequence
The system needs to clearly store whether a case was already escalated.

## Where this applies
This applies to the SLA auto-escalation logic in `app.js`.


