---
description: Amazon Web Services DocumentDB Subnet Group
---
aws_documentdb_subnet_group
---------------------------

| **Name**                 | **Type**     | **Nullable** |
| ------------------------ | ------------ | ------------ |
| accountId                | String       | &cross;      |
| accountName              | String       | &check;      |
| dbSubnetGroupArn         | String       | &check;      |
| dbSubnetGroupDescription | String       | &check;      |
| dbSubnetGroupName        | String       | &cross;      |
| region                   | String       | &cross;      |
| subnetGroupStatus        | String       | &check;      |
| subnets                  | List<Subnet> | &check;      |
| vpcId                    | String       | &check;      |

#### AvailabilityZone
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |

#### Subnet
| **Name**               | **Type**         | **Nullable** |
| ---------------------- | ---------------- | ------------ |
| subnetAvailabilityZone | AvailabilityZone | &check;      |
| subnetIdentifier       | String           | &check;      |
| subnetStatus           | String           | &check;      |
