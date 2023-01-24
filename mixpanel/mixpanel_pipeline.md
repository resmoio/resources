---
description: Mixpanel Pipeline
---
mixpanel_pipeline
-----------------

| **Name**  | **Type**       | **Nullable** |
| --------- | -------------- | ------------ |
| id        | String         | &cross;      |
| pipelines | List<Pipeline> | &check;      |

#### Pipeline
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| dispatcher     | String   | &check;      |
| frequency      | String   | &check;      |
| lastDispatched | String   | &check;      |
| name           | String   | &check;      |
| syncEnabled    | String   | &check;      |
