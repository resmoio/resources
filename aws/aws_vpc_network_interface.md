---
description: Amazon Web Services VPC Network Interface
---
aws_vpc_network_interface
-------------------------

| **Name**           | **Type**             | **Nullable** |
| ------------------ | -------------------- | ------------ |
| accountId          | String               | &cross;      |
| association        | Association          | &check;      |
| attachment         | Attachment           | &check;      |
| availabilityZone   | String               | &check;      |
| description        | String               | &check;      |
| groups             | List<Group>          | &check;      |
| id                 | String               | &cross;      |
| interfaceType      | String               | &check;      |
| ipv6Addresses      | List<String>         | &check;      |
| macAddress         | String               | &check;      |
| ownerId            | String               | &check;      |
| privateDnsName     | String               | &check;      |
| privateIpAddress   | String               | &check;      |
| privateIpAddresses | List<PrivateAddress> | &check;      |
| region             | String               | &cross;      |
| requesterId        | String               | &check;      |
| requesterManaged   | Boolean              | &check;      |
| sourceDestCheck    | Boolean              | &check;      |
| status             | String               | &check;      |
| subnetId           | String               | &check;      |
| tagSet             | Map<String,String>   | &check;      |
| vpcId              | String               | &check;      |

#### Association
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| allocationId    | String   | &check;      |
| carrierIp       | String   | &check;      |
| customerOwnedIp | String   | &check;      |
| id              | String   | &check;      |
| ipOwnerId       | String   | &check;      |
| publicDnsName   | String   | &check;      |
| publicIp        | String   | &check;      |

#### Attachment
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| attachTime          | String   | &check;      |
| deleteOnTermination | Boolean  | &check;      |
| deviceIndex         | Int      | &check;      |
| id                  | String   | &check;      |
| instanceId          | String   | &check;      |
| instanceOwnerId     | String   | &check;      |
| networkCardIndex    | Int      | &check;      |
| status              | String   | &check;      |

#### Group
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### PrivateAddress
| **Name**         | **Type**    | **Nullable** |
| ---------------- | ----------- | ------------ |
| association      | Association | &check;      |
| primary          | Boolean     | &check;      |
| privateDnsName   | String      | &check;      |
| privateIpAddress | String      | &check;      |
