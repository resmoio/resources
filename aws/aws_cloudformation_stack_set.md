---
description: Amazon Web Services CloudFormation StackSet
---
aws_cloudformation_stack_set
----------------------------

| **Name**              | **Type**           | **Nullable** |
| --------------------- | ------------------ | ------------ |
| accountId             | String             | &cross;      |
| accountName           | String             | &check;      |
| administrationRoleArn | String             | &check;      |
| arn                   | String             | &cross;      |
| autoDeployment        | AutoDeployment     | &check;      |
| capabilities          | List<String>       | &check;      |
| description           | String             | &check;      |
| id                    | String             | &cross;      |
| managedExecution      | ManagedExecution   | &check;      |
| name                  | String             | &check;      |
| organizationalUnitIds | List<String>       | &check;      |
| permissionModel       | String             | &check;      |
| region                | String             | &cross;      |
| status                | String             | &check;      |
| tags                  | Map<String,String> | &check;      |
| templateBody          | JSON               | &cross;      |

#### AutoDeployment
| **Name**                     | **Type** | **Nullable** |
| ---------------------------- | -------- | ------------ |
| enabled                      | Boolean  | &cross;      |
| retainStacksOnAccountRemoval | Boolean  | &cross;      |

#### ManagedExecution
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| active   | Boolean  | &cross;      |
