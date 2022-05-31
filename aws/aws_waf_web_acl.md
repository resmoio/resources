---
description: Amazon Web Services WAF Web ACL
---
aws_waf_web_acl
---------------

| **Name**      | **Type**   | **Nullable** |
| ------------- | ---------- | ------------ |
| accountId     | String     | &cross;      |
| arn           | String     | &cross;      |
| defaultAction | String     | &check;      |
| id            | String     | &cross;      |
| metricName    | String     | &check;      |
| name          | String     | &cross;      |
| region        | String     | &check;      |
| rules         | List<Rule> | &check;      |

#### Rule
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| action         | String       | &check;      |
| excludedRules  | List<String> | &check;      |
| overrideAction | String       | &check;      |
| priority       | Int          | &check;      |
| ruleId         | String       | &check;      |
| type           | String       | &check;      |
