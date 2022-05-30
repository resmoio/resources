---
description: Amazon Web Services Backup Selection
---
aws_backup_selection
--------------------

| **Name**         | **Type**        | **Nullable** |
| ---------------- | --------------- | ------------ |
| accountId        | String          | &cross;      |
| backupPlanId     | String          | &cross;      |
| conditions       | Conditions      | &check;      |
| creationDate     | String          | &check;      |
| creatorRequestId | String          | &check;      |
| iamRoleArn       | String          | &cross;      |
| id               | String          | &cross;      |
| listOfTags       | List<Condition> | &check;      |
| name             | String          | &cross;      |
| notResources     | List<String>    | &check;      |
| region           | String          | &cross;      |
| resources        | List<String>    | &check;      |

#### Condition
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| key      | String   | &cross;      |
| type     | String   | &cross;      |
| value    | String   | &cross;      |

#### Conditions
| **Name**        | **Type**                            | **Nullable** |
| --------------- | ----------------------------------- | ------------ |
| stringEquals    | List<Conditions.ConditionParameter> | &check;      |
| stringLike      | List<Conditions.ConditionParameter> | &check;      |
| stringNotEquals | List<Conditions.ConditionParameter> | &check;      |
| stringNotLike   | List<Conditions.ConditionParameter> | &check;      |

#### Conditions.ConditionParameter
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| key      | String   | &cross;      |
| value    | String   | &cross;      |
