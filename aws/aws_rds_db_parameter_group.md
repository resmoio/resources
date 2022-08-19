---
description: Amazon Web Services RDS DB Parameter Group
---
aws_rds_db_parameter_group
--------------------------

| **Name**    | **Type**                | **Nullable** |
| ----------- | ----------------------- | ------------ |
| accountId   | String                  | &cross;      |
| accountName | String                  | &check;      |
| arn         | String                  | &cross;      |
| description | String                  | &check;      |
| family      | String                  | &check;      |
| name        | String                  | &check;      |
| parameters  | List<AWSRDSDBParameter> | &check;      |
| region      | String                  | &cross;      |

#### AWSRDSDBParameter
| **Name**             | **Type**     | **Nullable** |
| -------------------- | ------------ | ------------ |
| allowedValues        | String       | &check;      |
| applyMethod          | String       | &check;      |
| applyType            | String       | &check;      |
| dataType             | String       | &check;      |
| description          | String       | &check;      |
| isModifiable         | Boolean      | &check;      |
| minimumEngineVersion | String       | &check;      |
| parameterName        | String       | &check;      |
| parameterValue       | String       | &check;      |
| source               | String       | &check;      |
| supportedEngineModes | List<String> | &check;      |
