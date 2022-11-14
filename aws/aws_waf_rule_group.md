---
description: Amazon Web Services WAF Rule Group
---
aws_waf_rule_group
------------------

| **Name**       | **Type**             | **Nullable** |
| -------------- | -------------------- | ------------ |
| accountId      | String               | &cross;      |
| accountName    | String               | &check;      |
| activatedRules | List<ActivatedRules> | &check;      |
| metricName     | String               | &check;      |
| name           | String               | &check;      |
| region         | String               | &check;      |
| ruleGroupId    | String               | &cross;      |
| scope          | String               | &check;      |

#### ActivatedRules
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| priority | Int      | &check;      |
| ruleId   | String   | &check;      |
| type     | String   | &check;      |
