---
description: Google Cloud Platform VPC Subnet
---
gcp_vpc_subnet
--------------

| **Name**                | **Type**                       | **Nullable** |
| ----------------------- | ------------------------------ | ------------ |
| creationTimestamp       | String                         | &check;      |
| description             | String                         | &check;      |
| enableFlowLogs          | Boolean                        | &check;      |
| externalIpv6Prefix      | String                         | &check;      |
| gatewayAddress          | String                         | &check;      |
| id                      | String                         | &cross;      |
| ipCidrRange             | String                         | &check;      |
| ipv6AccessType          | String                         | &check;      |
| ipv6CidrRange           | String                         | &check;      |
| kind                    | String                         | &check;      |
| logConfig               | SubnetworkLogConfig            | &check;      |
| name                    | String                         | &check;      |
| network                 | String                         | &check;      |
| privateIpGoogleAccess   | Boolean                        | &check;      |
| privateIpv6GoogleAccess | String                         | &check;      |
| project                 | String                         | &cross;      |
| purpose                 | String                         | &check;      |
| region                  | String                         | &check;      |
| role                    | String                         | &check;      |
| secondaryIpRanges       | List<SubnetworkSecondaryRange> | &check;      |
| stackType               | String                         | &check;      |
| state                   | String                         | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### SubnetworkLogConfig
| **Name**            | **Type**     | **Nullable** |
| ------------------- | ------------ | ------------ |
| aggregationInterval | String       | &check;      |
| enable              | Boolean      | &check;      |
| filterExpr          | String       | &check;      |
| flowSampling        | Number       | &check;      |
| metadata            | String       | &check;      |
| metadataFields      | List<String> | &check;      |

#### SubnetworkSecondaryRange
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| ipCidrRange | String   | &check;      |
| rangeName   | String   | &check;      |
