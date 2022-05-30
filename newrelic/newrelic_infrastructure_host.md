---
description: New Relic Infrastructure Host
---
newrelic_infrastructure_host
----------------------------

| **Name**      | **Type**  | **Nullable** |
| ------------- | --------- | ------------ |
| accountId     | Int       | &cross;      |
| alertSeverity | String    | &check;      |
| entityType    | String    | &check;      |
| guid          | String    | &cross;      |
| indexedAt     | Date      | &check;      |
| name          | String    | &cross;      |
| reporting     | Boolean   | &check;      |
| tags          | List<Tag> | &cross;      |
| type          | String    | &cross;      |

#### Tag
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| key      | String       | &cross;      |
| values   | List<String> | &cross;      |
