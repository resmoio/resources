---
description: Amazon Web Services Secrets Manager Secret
---
aws_secretsmanager_secret
-------------------------

| **Name**          | **Type**           | **Nullable** |
| ----------------- | ------------------ | ------------ |
| accountId         | String             | &cross;      |
| accountName       | String             | &check;      |
| arn               | String             | &cross;      |
| createdDate       | String             | &check;      |
| deletedDate       | String             | &check;      |
| description       | String             | &check;      |
| kmsKeyId          | String             | &check;      |
| lastAccessedDate  | String             | &check;      |
| lastChangedDate   | String             | &check;      |
| lastRotatedDate   | String             | &check;      |
| name              | String             | &cross;      |
| owningService     | String             | &check;      |
| primaryRegion     | String             | &check;      |
| region            | String             | &cross;      |
| resourcePolicy    | JSON               | &check;      |
| rotationEnabled   | Boolean            | &check;      |
| rotationLambdaARN | String             | &check;      |
| rotationRules     | RotationRulesType  | &cross;      |
| tags              | Map<String,String> | &cross;      |
| versionsToStages  | Map<String,List>   | &cross;      |

#### RotationRulesType
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| automaticallyAfterDays | Long     | &check;      |
