---
description: Amazon Web Services WAF Web ACL
---
aws_waf_web_acl
---------------

| **Name**             | **Type**             | **Nullable** |
| -------------------- | -------------------- | ------------ |
| accountId            | String               | &cross;      |
| accountName          | String               | &check;      |
| arn                  | String               | &cross;      |
| defaultAction        | String               | &check;      |
| id                   | String               | &cross;      |
| loggingConfiguration | LoggingConfiguration | &check;      |
| metricName           | String               | &check;      |
| name                 | String               | &cross;      |
| region               | String               | &check;      |
| rules                | List<Rule>           | &check;      |
| scope                | String               | &check;      |

#### LoggingConfiguration
| **Name**              | **Type**     | **Nullable** |
| --------------------- | ------------ | ------------ |
| logDestinationConfigs | List<String> | &check;      |
| redactedFields        | List<JSON>   | &check;      |
| resourceArn           | String       | &check;      |

#### Rule
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| action         | String       | &check;      |
| excludedRules  | List<String> | &check;      |
| overrideAction | String       | &check;      |
| priority       | Int          | &check;      |
| ruleId         | String       | &check;      |
| type           | String       | &check;      |
