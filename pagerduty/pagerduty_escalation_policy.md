---
description: PagerDuty Escalation Policy
---
pagerduty_escalation_policy
---------------------------

| **Name**                   | **Type**             | **Nullable** |
| -------------------------- | -------------------- | ------------ |
| description                | String               | &check;      |
| escalationRules            | List<EscalationRule> | &check;      |
| id                         | String               | &cross;      |
| name                       | String               | &check;      |
| numLoops                   | Int                  | &check;      |
| onCallHandoffNotifications | String               | &check;      |
| services                   | List<String>         | &check;      |
| summary                    | String               | &check;      |
| teams                      | List<String>         | &check;      |
| type                       | String               | &check;      |

#### EscalationRule
| **Name**                 | **Type**      | **Nullable** |
| ------------------------ | ------------- | ------------ |
| escalationDelayInMinutes | Int           | &check;      |
| id                       | String        | &check;      |
| targets                  | List<Targets> | &check;      |

#### Targets
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| type     | String   | &check;      |
