---
description: Tenable.io WAS Scan
---
tenable_was_scan
----------------

| **Name**         | **Type**       | **Nullable** |
| ---------------- | -------------- | ------------ |
| asset_id         | String         | &check;      |
| config_id        | String         | &check;      |
| config_metadata  | ConfigMetadata | &check;      |
| created_at       | String         | &check;      |
| metadata         | MetadataInf    | &check;      |
| parent_id        | String         | &check;      |
| requested_action | String         | &check;      |
| scan_id          | String         | &cross;      |
| scanner          | Scanner        | &check;      |
| status           | String         | &check;      |
| target           | String         | &check;      |
| template_name    | String         | &check;      |
| updated_at       | String         | &check;      |
| user_id          | String         | &check;      |

#### ConfigMetadata
| **Name**      | **Type**                    | **Nullable** |
| ------------- | --------------------------- | ------------ |
| template      | ConfigMetadata.Template     | &check;      |
| user_template | ConfigMetadata.UserTemplate | &check;      |

#### ConfigMetadata.Template
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| name        | String   | &check;      |
| template_id | String   | &check;      |

#### ConfigMetadata.UserTemplate
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| description      | String   | &check;      |
| name             | String   | &check;      |
| owner_id         | String   | &check;      |
| user_template_id | String   | &check;      |

#### MetadataInf
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

#### Scanner
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| group_name | String   | &check;      |
| version    | String   | &check;      |
