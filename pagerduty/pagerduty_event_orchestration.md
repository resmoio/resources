---
description: PagerDuty Event Orchestration
---
pagerduty_event_orchestration
-----------------------------

| **Name**    | **Type**          | **Nullable** |
| ----------- | ----------------- | ------------ |
| createdAt   | String            | &check;      |
| createdBy   | String            | &check;      |
| description | String            | &check;      |
| id          | String            | &cross;      |
| integration | List<Integration> | &check;      |
| name        | String            | &check;      |
| routes      | Int               | &check;      |
| team        | String            | &check;      |
| updatedAt   | String            | &check;      |
| updatedBy   | String            | &check;      |
| version     | String            | &check;      |

#### Integration
| **Name**   | **Type**               | **Nullable** |
| ---------- | ---------------------- | ------------ |
| id         | String                 | &check;      |
| parameters | Integration.Parameters | &check;      |

#### Integration.Parameters
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| routingKey | String   | &check;      |
| type       | String   | &check;      |
