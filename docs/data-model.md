# Draft Data Model

This is a draft model for discussion. Field names and structure may change as the hardware, firmware, and interface are built.

```json
{
  "container": {
    "container_id": "container_001",
    "tag_uid": "04AABBCCDDEE",
    "name": "Glass meal prep container",
    "empty_weight_g": 420.0,
    "created_at": "2026-05-27T00:00:00Z",
    "last_seen_at": "2026-05-27T00:00:00Z",
    "notes": ""
  },
  "tag": {
    "tag_uid": "04AABBCCDDEE",
    "container_id": "container_001",
    "assigned_at": "2026-05-27T00:00:00Z",
    "notes": ""
  },
  "food_item_assignment": {
    "assignment_id": "assignment_001",
    "container_id": "container_001",
    "name": "Rice and vegetables",
    "category": "meal prep",
    "prep_date": "2026-05-27",
    "initial_contents_weight_g": 780.0,
    "servings_total": 4,
    "notes": ""
  },
  "reading": {
    "reading_id": "reading_001",
    "container_id": "container_001",
    "tag_uid": "04AABBCCDDEE",
    "current_total_weight_g": 940.0,
    "empty_weight_g": 420.0,
    "contents_weight_g": 520.0,
    "servings_remaining_estimate": 2.7,
    "created_at": "2026-05-27T00:00:00Z",
    "notes": ""
  },
  "session_history": {
    "session_id": "session_001",
    "container_id": "container_001",
    "readings": ["reading_001"],
    "started_at": "2026-05-27T00:00:00Z",
    "ended_at": "2026-05-27T00:05:00Z",
    "notes": ""
  }
}
```

Fields to keep visible as the model changes:

- `container_id`
- `tag_uid`
- `name`
- `empty_weight_g`
- `current_total_weight_g`
- `contents_weight_g`
- `initial_contents_weight_g`
- `servings_total`
- `servings_remaining_estimate`
- `last_seen_at`
- `created_at`
- `notes`
