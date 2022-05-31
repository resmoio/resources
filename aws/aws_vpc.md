---
description: Amazon Web Services VPC
---
aws_vpc
-------

| **Name**                | **Type**                      | **Nullable** |
| ----------------------- | ----------------------------- | ------------ |
| accountId               | String                        | &cross;      |
| cidr                    | String                        | &check;      |
| cidrBlockAssociationSet | List<CIDRBlockAssociationSet> | &cross;      |
| id                      | String                        | &cross;      |
| isDefault               | Boolean                       | &cross;      |
| region                  | String                        | &cross;      |
| tags                    | Map<String,String>            | &cross;      |

#### CIDRBlockAssociationSet
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| associationId  | String   | &cross;      |
| cidrBlock      | String   | &check;      |
| cidrBlockState | String   | &cross;      |
