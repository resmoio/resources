---
description: Amazon Web Services IAM Instance Profile
---
aws_iam_instance_profile
------------------------

| **Name**            | **Type**           | **Nullable** |
| ------------------- | ------------------ | ------------ |
| accountId           | String             | &cross;      |
| accountName         | String             | &check;      |
| arn                 | String             | &cross;      |
| createDate          | String             | &check;      |
| instanceProfileId   | String             | &check;      |
| instanceProfileName | String             | &cross;      |
| path                | String             | &cross;      |
| roles               | List<Role>         | &check;      |
| tags                | Map<String,String> | &check;      |

#### AttachedPermissionsBoundary
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| permissionsBoundaryArn  | String   | &check;      |
| permissionsBoundaryType | String   | &check;      |

#### ResourceCustomComparable
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |


#### Role
| **Name**                 | **Type**                    | **Nullable** |
| ------------------------ | --------------------------- | ------------ |
| arn                      | String                      | &check;      |
| assumeRolePolicyDocument | JSON                        | &check;      |
| createDate               | String                      | &check;      |
| description              | String                      | &check;      |
| maxSessionDuration       | Int                         | &check;      |
| path                     | String                      | &check;      |
| permissionsBoundary      | AttachedPermissionsBoundary | &check;      |
| roleId                   | String                      | &check;      |
| roleLastUsed             | RoleLastUsed                | &check;      |
| roleName                 | String                      | &check;      |
| tags                     | Map<String,String>          | &check;      |

#### RoleLastUsed
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| lastUsedDate | String   | &check;      |
| region       | String   | &check;      |
