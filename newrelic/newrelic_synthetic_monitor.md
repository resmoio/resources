---
description: New Relic Synthetic Monitor
---
newrelic_synthetic_monitor
--------------------------

| **Name**      | **Type**  | **Nullable** |
| ------------- | --------- | ------------ |
| accountId     | Int       | &cross;      |
| alertSeverity | String    | &check;      |
| entityType    | String    | &check;      |
| guid          | String    | &cross;      |
| monitorId     | String    | &check;      |
| monitorType   | String    | &check;      |
| monitoredUrl  | String    | &check;      |
| name          | String    | &check;      |
| period        | Int       | &check;      |
| permalink     | String    | &check;      |
| reporting     | Boolean   | &check;      |
| tags          | List<Tag> | &check;      |
| type          | String    | &check;      |

#### Tag
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| key      | String       | &cross;      |
| values   | List<String> | &cross;      |
