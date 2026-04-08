# Architectural Decision Log

## 2026-04-08 — Keep V1 intentionally narrow
Decision: Prioritize a compact vertical slice over broad connector coverage.
Rationale: Increases reliability and keeps compliance review manageable.

## 2026-04-08 — Default FULL_AUTO only for explicitly permitted community surfaces
Decision: FULL_AUTO is allowed by default only when target metadata confirms permitted project/product posting.
Rationale: Aligns with strict anti-spam and policy compliance boundaries.

## 2026-04-08 — Deterministic harness before broad real-target expansion
Decision: Build local mock harness and fixture replay before adding many real connectors.
Rationale: Prevents unsafe behavior and improves regression coverage.
