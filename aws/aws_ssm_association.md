---
description: Amazon Web Services SSM Association
---
aws_ssm_association
-------------------

| **Name**           | **Type**            | **Nullable** |
| ------------------ | ------------------- | ------------ |
| accountId          | String              | &cross;      |
| associationId      | String              | &cross;      |
| associationName    | String              | &check;      |
| associationVersion | String              | &check;      |
| documentVersion    | String              | &check;      |
| instanceId         | String              | &check;      |
| lastExecutionDate  | String              | &check;      |
| name               | String              | &check;      |
| overview           | AssociationOverview | &check;      |
| region             | String              | &cross;      |
| scheduleExpression | String              | &check;      |
| scheduleOffset     | Int                 | &check;      |
| targetMaps         | List<Map>           | &check;      |
| targets            | List<Target>        | &check;      |

#### AssociationOverview
| **Name**                         | **Type**        | **Nullable** |
| -------------------------------- | --------------- | ------------ |
| associationStatusAggregatedCount | Map<String,Int> | &check;      |
| detailedStatus                   | String          | &check;      |
| status                           | String          | &check;      |

#### Target
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| key      | String       | &check;      |
| values   | List<String> | &check;      |
