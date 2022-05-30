---
description: New Relic Workload
---
newrelic_workload
-----------------

| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| accountId      | Int            | &cross;      |
| alertSeverity  | String         | &cross;      |
| createdAt      | Date           | &cross;      |
| createdByUser  | Int            | &check;      |
| entityType     | String         | &cross;      |
| guid           | String         | &cross;      |
| name           | String         | &cross;      |
| reporting      | Boolean        | &cross;      |
| tags           | List<Tag>      | &check;      |
| type           | String         | &cross;      |
| updatedAt      | Date           | &check;      |
| workloadStatus | WorkloadStatus | &cross;      |

#### Tag
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| key      | String       | &cross;      |
| values   | List<String> | &cross;      |

#### WorkloadStatus
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| description  | String   | &check;      |
| statusSource | String   | &cross;      |
| statusValue  | String   | &cross;      |
| summary      | String   | &check;      |
