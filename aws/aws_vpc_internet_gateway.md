---
description: Amazon Web Services VPC Internet Gateway
---
aws_vpc_internet_gateway
------------------------

| **Name**    | **Type**           | **Nullable** |
| ----------- | ------------------ | ------------ |
| accountId   | String             | &cross;      |
| attachments | List<Attachment>   | &cross;      |
| id          | String             | &cross;      |
| ownerId     | String             | &cross;      |
| region      | String             | &cross;      |
| tags        | Map<String,String> | &cross;      |

#### Attachment
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| state    | String   | &check;      |
| vpcId    | String   | &cross;      |
