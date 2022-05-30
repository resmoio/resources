---
description: Azure Network Security Group
---
azure_network_security_group
----------------------------

| **Name**             | **Type**           | **Nullable** |
| -------------------- | ------------------ | ------------ |
| defaultSecurityRules | List<SecurityRule> | &check;      |
| etag                 | String             | &cross;      |
| flowLogs             | List<FlowLog>      | &check;      |
| id                   | String             | &cross;      |
| location             | String             | &check;      |
| name                 | String             | &cross;      |
| networkInterfaces    | List<String>       | &check;      |
| provisioningState    | String             | &check;      |
| resourceGroupName    | String             | &cross;      |
| resourceGuid         | String             | &check;      |
| securityRules        | List<SecurityRule> | &check;      |
| subnets              | List<String>       | &check;      |
| subscriptionId       | String             | &cross;      |
| tags                 | Map<String,String> | &check;      |
| type                 | String             | &check;      |

#### ApplicationSecurityGroup
| **Name**          | **Type**           | **Nullable** |
| ----------------- | ------------------ | ------------ |
| etag              | String             | &check;      |
| id                | String             | &cross;      |
| location          | String             | &cross;      |
| name              | String             | &cross;      |
| provisioningState | String             | &check;      |
| resourceGuid      | String             | &check;      |
| tags              | Map<String,String> | &check;      |
| type              | String             | &cross;      |

#### FlowAnalyticsConfiguration
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| enabled                  | Boolean  | &check;      |
| trafficAnalyticsInterval | Int      | &check;      |
| workspaceId              | String   | &check;      |
| workspaceRegion          | String   | &check;      |
| workspaceResourceId      | String   | &check;      |

#### FlowLog
| **Name**                                 | **Type**                   | **Nullable** |
| ---------------------------------------- | -------------------------- | ------------ |
| enabled                                  | Boolean                    | &check;      |
| etag                                     | String                     | &check;      |
| formatType                               | String                     | &check;      |
| id                                       | String                     | &cross;      |
| location                                 | String                     | &check;      |
| name                                     | String                     | &check;      |
| networkWatcherFlowAnalyticsConfiguration | FlowAnalyticsConfiguration | &check;      |
| provisioningState                        | String                     | &check;      |
| retentionPolicyDays                      | Int                        | &check;      |
| retentionPolicyEnabled                   | Boolean                    | &check;      |
| storageId                                | String                     | &check;      |
| tag                                      | Map<String,String>         | &check;      |
| targetResourceGuid                       | String                     | &check;      |
| targetResourceId                         | String                     | &check;      |
| type                                     | String                     | &check;      |
| version                                  | Int                        | &check;      |

#### PortRange
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| fromPort | String   | &check;      |
| toPort   | String   | &check;      |

#### SecurityRule
| **Name**                             | **Type**                       | **Nullable** |
| ------------------------------------ | ------------------------------ | ------------ |
| access                               | String                         | &check;      |
| description                          | String                         | &check;      |
| destinationAddressPrefixes           | List<String>                   | &cross;      |
| destinationApplicationSecurityGroups | List<ApplicationSecurityGroup> | &check;      |
| destinationPortRanges                | List<PortRange>                | &cross;      |
| direction                            | String                         | &check;      |
| etag                                 | String                         | &check;      |
| id                                   | String                         | &cross;      |
| name                                 | String                         | &check;      |
| priority                             | Int                            | &check;      |
| protocol                             | String                         | &check;      |
| provisioningState                    | String                         | &check;      |
| sourceAddressPrefixes                | List<String>                   | &cross;      |
| sourceApplicationSecurityGroups      | List<ApplicationSecurityGroup> | &check;      |
| sourcePortRanges                     | List<PortRange>                | &cross;      |
| type                                 | String                         | &check;      |
