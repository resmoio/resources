---
description: New Relic Mobile Application
---
newrelic_mobile_application
---------------------------

| **Name**                 | **Type**                      | **Nullable** |
| ------------------------ | ----------------------------- | ------------ |
| accountId                | Int                           | &cross;      |
| alertSeverity            | String                        | &cross;      |
| applicationId            | Long                          | &cross;      |
| entityType               | String                        | &cross;      |
| guid                     | String                        | &cross;      |
| indexedAt                | Date                          | &cross;      |
| metricNormalizationRules | List<MetricNormalizationRule> | &check;      |
| name                     | String                        | &cross;      |
| reporting                | Boolean                       | &cross;      |
| tags                     | List<Tag>                     | &cross;      |
| type                     | String                        | &cross;      |

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

#### Tag
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| key      | String       | &cross;      |
| values   | List<String> | &cross;      |
