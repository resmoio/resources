---
description: Amazon Web Services VPC Network ACL
---
aws_vpc_network_acl
-------------------

| **Name**    | **Type**           | **Nullable** |
| ----------- | ------------------ | ------------ |
| accountId   | String             | &cross;      |
| accountName | String             | &check;      |
| attachments | List<Association>  | &cross;      |
| entries     | List<Entry>        | &cross;      |
| id          | String             | &cross;      |
| isDefault   | Boolean            | &cross;      |
| ownerId     | String             | &cross;      |
| region      | String             | &cross;      |
| tags        | Map<String,String> | &cross;      |

#### Association
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| subnetId | String   | &check;      |

#### Entry
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| cidrBlock     | String       | &check;      |
| egress        | Boolean      | &check;      |
| icmp          | ICMPTypeCode | &check;      |
| ipv6CidrBlock | String       | &check;      |
| portRange     | PortRange    | &check;      |
| protocol      | String       | &cross;      |
| ruleAction    | String       | &check;      |
| ruleNumber    | Int          | &cross;      |

#### ICMPTypeCode
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | Int      | &cross;      |
| type     | Int      | &cross;      |

#### PortRange
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| from     | Int      | &check;      |
| to       | Int      | &check;      |
