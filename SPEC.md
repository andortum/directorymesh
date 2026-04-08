# DirectoryMesh Specification (V1)

## Problem
Teams repeatedly rewrite company/product/project details across many public surfaces. Manual updates are error-prone, inconsistent, and hard to audit.

## Canonical solution
DirectoryMesh stores a canonical profile and orchestrates compliant sync/refresh/posting workflows to permitted surfaces through typed connectors.

## V1 target classes
- `PRODUCT_DIRECTORY`
- `PROFILE_SURFACE`
- `CLAIM_REFRESH_SURFACE`
- `COMMUNITY_DISCOVERY_SURFACE` (discovery + draft only)
- `COMMUNITY_ENGAGEMENT_SURFACE` (full automatic topic/comment/reply)

## V1 connector patterns
- `API_SUBMISSION`
- `PUBLIC_FORM_SUBMISSION`
- `PROFILE_UPDATE`
- `CLAIM_REFRESH`
- `DISCOVERY_DRAFT_ONLY`
- `COMMUNITY_TOPIC_CREATE`
- `COMMUNITY_COMMENT_POST`
- `COMMUNITY_REPLY_SEND`

## Hard constraints
- No deceptive automation.
- No captcha bypass or anti-bot evasion.
- No fake engagement.
- Only act where rules permit.

## Community automation defaults
- `automation_mode = FULL_AUTO` for eligible `COMMUNITY_ENGAGEMENT_SURFACE` targets.
- Max 1 action per community per 24 hours by default.
- Require evidence package for every action.

## Required evidence payload
- Request payload (redacted secrets)
- Response payload
- Timestamp + actor/service identity
- Connector version
- Screenshot artifact path
- Rule snapshot/TOS note

## Definition of done (V1)
1. App runs locally.
2. Migrations + seed succeed.
3. Mock harness passes.
4. Connector SDK works.
5. At least one FULL_AUTO real Tier-1 directory target works.
6. At least one FULL_AUTO community engagement target works end-to-end.
7. Every community action stores evidence/audit trail.
8. Tests pass.
9. Core docs are complete.
