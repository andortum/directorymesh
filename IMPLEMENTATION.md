# Implementation Blueprint

## Proposed stack (V1)
- Frontend: Next.js + TypeScript
- Backend/API: Next.js route handlers (or modular service layer)
- Database: PostgreSQL + Prisma
- Queue: lightweight DB-backed job queue for deterministic local runs
- Automation: Playwright for compliant browser flows
- Validation: Zod schemas
- Testing: Vitest + Playwright integration tests

## Core modules
1. `canonical-profile`
2. `target-registry`
3. `connector-sdk`
4. `orchestrator`
5. `community-engine`
6. `evidence-store`
7. `audit-log`

## Evidence storage model
- Store metadata in relational tables.
- Store payload snapshots and screenshots in structured filesystem/object abstraction.
- Reference immutable hashes from audit events.

## Safety and compliance gates
- Target-level permission metadata required before execution.
- Robot/TOS policy checks before any network action.
- Per-community cooldown gate before topic/comment/reply actions.
