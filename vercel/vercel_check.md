---
description: Vercel Check
---
vercel_check
------------

| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| completedAt   | Long     | &check;      |
| conclusion    | String   | &check;      |
| createdAt     | Long     | &check;      |
| deploymentId  | String   | &check;      |
| detailsUrl    | String   | &check;      |
| id            | String   | &cross;      |
| integrationId | String   | &check;      |
| name          | String   | &check;      |
| output        | Metrics  | &check;      |
| path          | String   | &check;      |
| rerequestable | Boolean  | &check;      |
| startedAt     | Long     | &check;      |
| status        | String   | &check;      |
| updatedAt     | Long     | &check;      |

#### Metrics
| **Name** | **Type**                   | **Nullable** |
| -------- | -------------------------- | ------------ |
| metrics  | Map<String,Metrics.Metric> | &check;      |

#### Metrics.Metric
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| previousValue | Long     | &check;      |
| source        | String   | &check;      |
| value         | Long     | &check;      |
