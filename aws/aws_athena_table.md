---
description: Amazon Web Services Athena Table
---
aws_athena_table
----------------

| **Name**      | **Type**           | **Nullable** |
| ------------- | ------------------ | ------------ |
| accountId     | String             | &cross;      |
| accountName   | String             | &check;      |
| columns       | List<Column>       | &check;      |
| createTime    | String             | &check;      |
| name          | String             | &cross;      |
| parameters    | Map<String,String> | &check;      |
| partitionKeys | List<Column>       | &check;      |
| region        | String             | &cross;      |
| tableType     | String             | &check;      |

#### Column
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| comment  | String   | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |
