# AUDIT LOG — CAMERA & MICROPHONE EVENTS

## Fields
| Field | Type | Description |
|-------|------|-------------|
| event_id | UUID | Unique event |
| user_id | UUID | User initiating |
| seller_id | UUID | If applicable |
| timestamp_start | DateTime | Activation time |
| timestamp_end | DateTime | Deactivation time |
| camera_active | Boolean | True/False |
| microphone_active | Boolean | True/False |
| consent_given | Boolean | Explicit user consent |
| activation_method | Enum | UI button / system prompt |
| session_id | UUID | Communication session |
| notes | Text | Optional metadata |

---

## Rules
- No camera event may occur without `consent_given = true`.
- Logs must be immutable.
- Logs must be exportable for compliance review.
