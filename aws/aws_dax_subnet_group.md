---
description: Amazon Web Services DAX Subnet Group
---
aws_dax_subnet_group
--------------------

| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| accountId       | String       | &cross;      |
| accountName     | String       | &check;      |
| description     | String       | &check;      |
| region          | String       | &cross;      |
| subnetGroupName | String       | &cross;      |
| subnets         | List<Subnet> | &check;      |
| vpcId           | String       | &check;      |

#### Subnet
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| subnetAvailabilityZone | String   | &check;      |
| subnetIdentifier       | String   | &check;      |
