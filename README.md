# DirectoryMesh

DirectoryMesh is a compact, operations-focused SaaS for maintaining one canonical company/product profile and synchronizing it to allowed public listing, profile, claim/refresh, and community surfaces.

## Current status

This repository is initialized with a production-oriented planning and governance baseline:

- Product specification and scope boundaries
- Architecture and stack decisions
- Connector SDK and harness plan
- Target registry schema and maturity model
- Task tracking and implementation roadmap

## V1 intent

V1 is intentionally narrow:

- Deterministic connector SDK + local mock harness
- Core orchestration for profile sync and claim/refresh
- Community discovery + drafting + full-auto posting on explicitly permitted surfaces
- Per-community cooldown/rate-limit enforcement
- Full evidence/audit artifacts for every community action

## Safety boundaries

DirectoryMesh explicitly prohibits:

- Fake engagement/reviews/identities
- Captcha bypass or anti-bot evasion
- Deceptive/spam automation

DirectoryMesh only automates where robots.txt, TOS, and community guidelines permit actions.
