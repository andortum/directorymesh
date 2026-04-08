# DirectoryMesh Plan

## Phase 0 — Repository + governance baseline
- Initialize repository files.
- Create required docs and initial architecture decisions.
- Define explicit scope boundaries and compliance guardrails.

## Phase 1 — Core platform skeleton
- Create backend service with DB schema + migrations.
- Build canonical profile model and target registry model.
- Implement connector runtime interfaces and orchestrator skeleton.

## Phase 2 — Connector SDK + deterministic harness
- Implement SDK contracts and lifecycle hooks.
- Build mock target server and fixture-driven test scenarios.
- Add idempotency, retry policy, and evidence capture pipeline.

## Phase 3 — V1 product features
- Canonical profile CRUD UI/API.
- Sync/claim workflows for selected Tier-1 targets.
- Community discovery, scoring, drafting, and FULL_AUTO posting.
- Community post history/evidence views.

## Phase 4 — Harden and validate
- Security/compliance checks.
- Integration tests and smoke tests.
- Demo script and runbook.
