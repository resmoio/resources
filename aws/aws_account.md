---
description: Amazon Web Services Account
---
aws_account
-----------

| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| accountId       | String             | &check;      |
| accountName     | String             | &check;      |
| arn             | String             | &cross;      |
| canAssumeRole   | Boolean            | &check;      |
| email           | String             | &check;      |
| id              | String             | &cross;      |
| joinedMethod    | String             | &check;      |
| joinedTimestamp | String             | &check;      |
| name            | String             | &check;      |
| parent          | String             | &check;      |
| status          | String             | &check;      |
| tags            | Map<String,String> | &cross;      |

#### AccountProvision
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| available          | Boolean      | &cross;      |
| missingPermissions | List<String> | &cross;      |
