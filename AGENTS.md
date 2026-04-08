# GitHub-First Rule (Mandatory)
Every single file creation, edit, deletion, or change must be committed immediately with a Conventional Commit message and pushed to `main`.

# DirectoryMesh Agent Instructions

## Product boundaries
- Do not build fake engagement, fake reviews, fake identities, captcha bypass, stealth abuse, or spam tooling.
- Build only automation that is explicitly permitted by target TOS/community rules.

## Build strategy
1. Maintain foundational product/decision docs first.
2. Keep V1 narrow and deterministic.
3. Prefer explicit schemas, typed interfaces, and testable workflows.
4. Capture deviations in `DECISIONS.md`.

## Required docs
Keep these files current:
- `SPEC.md`
- `PLANS.md`
- `IMPLEMENTATION.md`
- `DECISIONS.md`
- `TASKS.md`
- `TARGET_SELECTION_RULES.md`
- `CONNECTOR_MATURITY_MATRIX.md`
- `TARGET_REGISTRY_SCHEMA.md`

## Community automation policy
- Community actions are FULL_AUTO by default for eligible targets.
- Enforce heavy built-in rate limiting (default: 1 action/community/24h).
- Store full evidence for every action (screenshot + payload + response + metadata).
- Respect robots.txt, TOS, and community guidelines.

## Engineering standards
- Use deterministic local harnesses for connector testing.
- Require idempotency keys for external actions.
- Keep audit logs immutable and queryable.
