---
description: Tenable.io WAS Configuration
---
tenable_was_configuration
-------------------------

| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| config_id        | String       | &cross;      |
| container_id     | String       | &check;      |
| created_at       | String       | &check;      |
| description      | String       | &check;      |
| is_shared        | Boolean      | &check;      |
| last_scan        | Scan         | &check;      |
| name             | String       | &check;      |
| owner_id         | String       | &check;      |
| schedule         | Schedule     | &check;      |
| target           | String       | &check;      |
| target_count     | Int          | &check;      |
| targets          | String       | &check;      |
| updated_at       | String       | &check;      |
| user_permissions | String       | &check;      |
| user_template    | UserTemplate | &check;      |

#### Scan
| **Name**         | **Type**         | **Nullable** |
| ---------------- | ---------------- | ------------ |
| asset_id         | String           | &check;      |
| config_id        | String           | &check;      |
| created_at       | String           | &check;      |
| metadata         | Scan.MetadataInf | &check;      |
| parent_id        | String           | &check;      |
| requested_action | String           | &check;      |
| scan_id          | String           | &check;      |
| status           | String           | &check;      |
| target           | String           | &check;      |
| updated_at       | String           | &check;      |
| user_id          | String           | &check;      |

#### Scan.MetadataInf
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| audited_pages      | Int      | &check;      |
| crawled_urls       | Int      | &check;      |
| finalized_children | Int      | &check;      |
| queued_pages       | Int      | &check;      |
| queued_urls        | Int      | &check;      |
| request_count      | Int      | &check;      |
| response_time      | Int      | &check;      |
| total_children     | Int      | &check;      |

#### Schedule
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| enabled   | Boolean  | &check;      |
| rrule     | String   | &check;      |
| starttime | String   | &check;      |
| timezone  | String   | &check;      |

#### UserTemplate
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| name             | String   | &check;      |
| user_template_id | String   | &check;      |
