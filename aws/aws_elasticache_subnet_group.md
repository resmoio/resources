---
description: Amazon Web Services ElastiCache Subnet Group
---
aws_elasticache_subnet_group
----------------------------

| **Name**                    | **Type**     | **Nullable** |
| --------------------------- | ------------ | ------------ |
| accountId                   | String       | &cross;      |
| accountName                 | String       | &check;      |
| arn                         | String       | &check;      |
| cacheSubnetGroupDescription | String       | &check;      |
| cacheSubnetGroupName        | String       | &cross;      |
| region                      | String       | &cross;      |
| subnets                     | List<Subnet> | &check;      |
| vpcId                       | String       | &check;      |

#### Subnet
| **Name**               | **Type**                | **Nullable** |
| ---------------------- | ----------------------- | ------------ |
| subnetAvailabilityZone | Subnet.AvailabilityZone | &check;      |
| subnetIdentifier       | String                  | &check;      |
| subnetOutpost          | Subnet.SubnetOutpost    | &check;      |

#### Subnet.AvailabilityZone
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |

#### Subnet.SubnetOutpost
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| subnetOutpostArn | String   | &check;      |
