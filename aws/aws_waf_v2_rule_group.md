---
description: Amazon Web Services WAF V2 Rule Group
---
aws_waf_v2_rule_group
---------------------

| **Name**         | **Type**         | **Nullable** |
| ---------------- | ---------------- | ------------ |
| accountId        | String           | &cross;      |
| accountName      | String           | &check;      |
| arn              | String           | &cross;      |
| capacity         | Long             | &check;      |
| description      | String           | &check;      |
| id               | String           | &check;      |
| labelNamespace   | String           | &check;      |
| name             | String           | &check;      |
| region           | String           | &check;      |
| rules            | List<Rule>       | &check;      |
| scope            | String           | &check;      |
| visibilityConfig | VisibilityConfig | &check;      |

#### Rule
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| priority | Int      | &check;      |

#### VisibilityConfig
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| cloudWatchMetricsEnabled | Boolean  | &check;      |
| metricName               | String   | &check;      |
| sampledRequestsEnabled   | Boolean  | &check;      |
