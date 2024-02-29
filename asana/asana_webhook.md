---
description: Asana Webhook
---
asana_webhook
-------------

| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| active               | Boolean  | &cross;      |
| created_at           | String   | &cross;      |
| gid                  | String   | &cross;      |
| last_failure_at      | String   | &cross;      |
| last_failure_content | String   | &cross;      |
| last_success_at      | String   | &cross;      |
| resource             | Resource | &cross;      |
| resource_type        | String   | &cross;      |
| target               | String   | &cross;      |
| workspaceId          | String   | &cross;      |

#### Resource
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| gid           | String   | &cross;      |
| name          | String   | &cross;      |
| resource_type | String   | &cross;      |
