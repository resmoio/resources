---
description: Amazon Web Services GuardDuty Filter
---
aws_guardduty_filter
--------------------

| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| accountId       | String             | &cross;      |
| accountName     | String             | &check;      |
| action          | String             | &check;      |
| description     | String             | &check;      |
| detectorId      | String             | &check;      |
| findingCriteria | FindingCriteria    | &check;      |
| name            | String             | &cross;      |
| rank            | Int                | &check;      |
| tags            | Map<String,String> | &check;      |

#### Condition
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| equals             | List<String> | &check;      |
| greaterThan        | Long         | &check;      |
| greaterThanOrEqual | Long         | &check;      |
| lessThan           | Long         | &check;      |
| lessThanOrEqual    | Long         | &check;      |
| notEquals          | List<String> | &check;      |

#### FindingCriteria
| **Name**  | **Type**              | **Nullable** |
| --------- | --------------------- | ------------ |
| criterion | Map<String,Condition> | &check;      |
