---
description: New Relic Browser Application
---
newrelic_browser_application
----------------------------

| **Name**                 | **Type**                      | **Nullable** |
| ------------------------ | ----------------------------- | ------------ |
| accountId                | Int                           | &cross;      |
| agentInstallType         | String                        | &check;      |
| alertSeverity            | String                        | &check;      |
| applicationId            | Long                          | &check;      |
| browserSettings          | Setting                       | &check;      |
| entityType               | String                        | &check;      |
| guid                     | String                        | &cross;      |
| indexedAt                | Date                          | &check;      |
| metricNormalizationRules | List<MetricNormalizationRule> | &check;      |
| name                     | String                        | &check;      |
| reporting                | Boolean                       | &check;      |
| runningAgentVersions     | RunningAgentVersion           | &check;      |
| servingApmApplicationId  | Int                           | &check;      |
| settings                 | Setting                       | &check;      |
| tags                     | List<Tag>                     | &check;      |
| type                     | String                        | &check;      |

#### MetricNormalizationRule
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| action          | String   | &check;      |
| applicationGuid | String   | &cross;      |
| applicationName | String   | &cross;      |
| createdAt       | Date     | &check;      |
| enabled         | Boolean  | &cross;      |
| evalOrder       | Long     | &cross;      |
| id              | Long     | &cross;      |
| matchExpression | String   | &cross;      |
| notes           | String   | &check;      |
| replacement     | String   | &check;      |
| terminateChain  | Boolean  | &check;      |

#### RunningAgentVersion
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| maxVersion | Int      | &check;      |
| minVersion | Int      | &check;      |

#### Setting
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| apdexTarget | Double   | &check;      |

#### Tag
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| key      | String       | &cross;      |
| values   | List<String> | &cross;      |
