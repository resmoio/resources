---
description: Amazon Web Services VPC Security Group
---
aws_vpc_security_group
----------------------

| **Name**    | **Type**           | **Nullable** |
| ----------- | ------------------ | ------------ |
| accountId   | String             | &cross;      |
| accountName | String             | &check;      |
| description | String             | &cross;      |
| egress      | List<IPPermission> | &cross;      |
| id          | String             | &cross;      |
| ingress     | List<IPPermission> | &cross;      |
| name        | String             | &cross;      |
| region      | String             | &cross;      |
| tags        | Map<String,String> | &cross;      |
| vpcId       | String             | &cross;      |

#### IPPermission
| **Name**         | **Type**              | **Nullable** |
| ---------------- | --------------------- | ------------ |
| fromPort         | Int                   | &check;      |
| ipProtocol       | String                | &check;      |
| ipRanges         | List<IPRange>         | &check;      |
| ipv6Ranges       | List<IPV6Range>       | &check;      |
| prefixListIds    | List<PrefixListId>    | &check;      |
| toPort           | Int                   | &check;      |
| userIdGroupPairs | List<UserIdGroupPair> | &check;      |

#### IPRange
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| cidrIp      | String   | &cross;      |
| description | String   | &check;      |

#### IPV6Range
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| cidrIpv6    | String   | &cross;      |
| description | String   | &check;      |

#### PrefixListId
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| description  | String   | &check;      |
| prefixListId | String   | &cross;      |

#### UserIdGroupPair
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| description            | String   | &check;      |
| groupId                | String   | &cross;      |
| groupName              | String   | &check;      |
| peeringStatus          | String   | &check;      |
| userId                 | String   | &cross;      |
| vpcId                  | String   | &check;      |
| vpcPeeringConnectionId | String   | &check;      |
