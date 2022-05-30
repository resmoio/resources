---
description: New Relic Alert Policy
---
newrelic_alert_policy
---------------------

| **Name**           | **Type**                     | **Nullable** |
| ------------------ | ---------------------------- | ------------ |
| accountId          | Int                          | &cross;      |
| conditions         | List<ConditionConfiguration> | &cross;      |
| id                 | String                       | &cross;      |
| incidentPreference | String                       | &cross;      |
| name               | String                       | &cross;      |

#### ConditionConfiguration
| **Name**                  | **Type**                          | **Nullable** |
| ------------------------- | --------------------------------- | ------------ |
| description               | String                            | &check;      |
| enabled                   | Boolean                           | &cross;      |
| expiration                | ConditionConfiguration.Expiration | &cross;      |
| id                        | String                            | &cross;      |
| name                      | String                            | &cross;      |
| nrql                      | String                            | &cross;      |
| policyId                  | String                            | &cross;      |
| runbook                   | String                            | &check;      |
| signal                    | ConditionConfiguration.Signal     | &cross;      |
| terms                     | List<ConditionConfiguration.Term> | &cross;      |
| type                      | String                            | &cross;      |
| violationTimeLimitSeconds | Number                            | &check;      |

#### ConditionConfiguration.Expiration
| **Name**                    | **Type** | **Nullable** |
| --------------------------- | -------- | ------------ |
| closeViolationsOnExpiration | Boolean  | &check;      |
| expirationDuration          | Boolean  | &check;      |
| openViolationOnExpiration   | Boolean  | &check;      |

#### ConditionConfiguration.Signal
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| aggregationDelay  | Number   | &check;      |
| aggregationMethod | String   | &check;      |
| aggregationTimer  | Number   | &check;      |
| aggregationWindow | Number   | &check;      |
| fillOption        | String   | &check;      |
| fillValue         | Double   | &check;      |

#### ConditionConfiguration.Term
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| operator             | String   | &cross;      |
| priority             | String   | &cross;      |
| threshold            | Double   | &cross;      |
| thresholdDuration    | Int      | &cross;      |
| thresholdOccurrences | String   | &cross;      |
