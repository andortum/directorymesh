# Target Registry Schema (V1)

## Required fields
- `target_id` (string)
- `name` (string)
- `base_url` (string)
- `target_class` (enum)
- `automation_mode` (enum; default FULL_AUTO for community engagement targets)
- `connector_pattern` (enum)
- `community_rules_summary` (text, required for community classes)
- `tos_url` (string)
- `robots_url` (string)
- `allowed_actions` (string[])
- `cooldown_policy` (json)
- `status` (enum: ACTIVE, PAUSED, DEPRECATED)
- `maturity_level` (enum: M0..M4)

## Enums
### target_class
- PRODUCT_DIRECTORY
- PROFILE_SURFACE
- CLAIM_REFRESH_SURFACE
- COMMUNITY_DISCOVERY_SURFACE
- COMMUNITY_ENGAGEMENT_SURFACE

### automation_mode
- FULL_AUTO
- ASSISTED
- MANUAL_ONLY

### connector_pattern
- API_SUBMISSION
- PUBLIC_FORM_SUBMISSION
- PROFILE_UPDATE
- CLAIM_REFRESH
- DISCOVERY_DRAFT_ONLY
- COMMUNITY_TOPIC_CREATE
- COMMUNITY_COMMENT_POST
- COMMUNITY_REPLY_SEND
