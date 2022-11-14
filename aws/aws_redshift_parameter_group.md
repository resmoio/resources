---
description: Amazon Web Services Redshift Parameter Group
---
aws_redshift_parameter_group
----------------------------

| **Name**             | **Type**           | **Nullable** |
| -------------------- | ------------------ | ------------ |
| accountId            | String             | &cross;      |
| accountName          | String             | &check;      |
| description          | String             | &check;      |
| parameterGroupFamily | String             | &check;      |
| parameterGroupName   | String             | &cross;      |
| parameters           | List<Parameter>    | &check;      |
| region               | String             | &cross;      |
| tags                 | Map<String,String> | &check;      |

#### Parameter
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| allowedValues        | String   | &check;      |
| applyType            | String   | &check;      |
| dataType             | String   | &check;      |
| description          | String   | &check;      |
| isModifiable         | Boolean  | &check;      |
| minimumEngineVersion | String   | &check;      |
| parameterName        | String   | &check;      |
| parameterValue       | String   | &check;      |
| source               | String   | &check;      |
