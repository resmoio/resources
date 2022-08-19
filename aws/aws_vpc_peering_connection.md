---
description: Amazon Web Services VPC Peering Connection
---
aws_vpc_peering_connection
--------------------------

| **Name**         | **Type**           | **Nullable** |
| ---------------- | ------------------ | ------------ |
| accepterVpcInfo  | VpcInfo            | &cross;      |
| accountId        | String             | &cross;      |
| accountName      | String             | &check;      |
| expirationTime   | String             | &check;      |
| id               | String             | &cross;      |
| region           | String             | &cross;      |
| requesterVpcInfo | VpcInfo            | &cross;      |
| status           | Status             | &cross;      |
| tags             | Map<String,String> | &cross;      |

#### Group
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |

#### PeeringOptions
| **Name**                                   | **Type** | **Nullable** |
| ------------------------------------------ | -------- | ------------ |
| allowDnsResolutionFromRemoteVpc            | Boolean  | &cross;      |
| allowEgressFromLocalClassicLinkToRemoteVpc | Boolean  | &cross;      |
| allowEgressFromLocalVpcToRemoteClassicLink | Boolean  | &cross;      |

#### Status
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | String   | &cross;      |
| message  | String   | &cross;      |

#### VpcInfo
| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| cidrBlock      | String         | &check;      |
| cidrBlockSet   | List<String>   | &cross;      |
| ownerId        | String         | &cross;      |
| peeringOptions | PeeringOptions | &check;      |
| region         | String         | &cross;      |
| vpcId          | String         | &cross;      |
