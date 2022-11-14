---
description: Amazon Web Services WAF Rule
---
aws_waf_rule
------------

| **Name**    | **Type**        | **Nullable** |
| ----------- | --------------- | ------------ |
| accountId   | String          | &cross;      |
| accountName | String          | &check;      |
| metricName  | String          | &check;      |
| name        | String          | &check;      |
| predicates  | List<Predicate> | &check;      |
| region      | String          | &check;      |
| ruleId      | String          | &cross;      |
| scope       | String          | &check;      |

#### Predicate
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| dataId   | String   | &check;      |
| negated  | Boolean  | &check;      |
| type     | String   | &check;      |
