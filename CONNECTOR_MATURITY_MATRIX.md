# Connector Maturity Matrix

| Level | Name | Requirements |
|---|---|---|
| M0 | Draft | Schema drafted, no executable flow |
| M1 | Harnessed | Deterministic mock harness scenarios pass |
| M2 | Sandbox Validated | Tested against non-production/safe test surface |
| M3 | Production Ready | Idempotent, observable, evidence capture complete |
| M4 | Tier-1 Trusted | Stable production success and low incident rate |

## Promotion gates
- M1→M2: policy checks + retry/idempotency tests pass
- M2→M3: real execution with evidence and audit records validated
- M3→M4: sustained success SLO met for defined window
