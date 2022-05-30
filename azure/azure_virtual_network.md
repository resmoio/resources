---
description: Azure Virtual Network
---
azure_virtual_network
---------------------

| **Name**                | **Type**                     | **Nullable** |
| ----------------------- | ---------------------------- | ------------ |
| addressSpaces           | List<String>                 | &check;      |
| bgpCommunities          | VirtualNetworkBgpCommunities | &check;      |
| ddosProtectionPlanId    | String                       | &check;      |
| dnsServerIPs            | List<String>                 | &check;      |
| encryptionEnabled       | Boolean                      | &check;      |
| encryptionEnforcement   | String                       | &check;      |
| etag                    | String                       | &check;      |
| extendedLocation        | ExtendedLocation             | &check;      |
| flowTimeoutInMinutes    | Int                          | &check;      |
| id                      | String                       | &cross;      |
| ipAllocations           | List<String>                 | &check;      |
| isDdosProtectionEnabled | Boolean                      | &check;      |
| isVmProtectionEnabled   | Boolean                      | &check;      |
| location                | String                       | &cross;      |
| name                    | String                       | &cross;      |
| provisioningState       | String                       | &check;      |
| resourceGroupName       | String                       | &cross;      |
| resourceGuid            | String                       | &check;      |
| subnets                 | List<Subnet>                 | &check;      |
| subscriptionId          | String                       | &cross;      |
| tags                    | Map<String,String>           | &check;      |
| type                    | String                       | &cross;      |
| virtualNetworkPeerings  | List<VirtualNetworkPeering>  | &check;      |

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

#### CustomConfigPropertiesFormat
| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| fqdn        | String       | &check;      |
| ipAddresses | List<String> | &check;      |

#### ExtendedLocation
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |

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

#### IpConfiguration
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| etag              | String   | &check;      |
| id                | String   | &check;      |
| name              | String   | &check;      |
| privateIpAddress  | String   | &check;      |
| provisioningState | String   | &check;      |

#### Link
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| allowDelete        | Boolean      | &check;      |
| etag               | String       | &check;      |
| id                 | String       | &cross;      |
| link               | String       | &check;      |
| linkedResourceType | String       | &check;      |
| locations          | List<String> | &check;      |
| name               | String       | &cross;      |
| provisioningState  | String       | &check;      |
| type               | String       | &cross;      |

#### NetworkSecurityGroup
| **Name**             | **Type**           | **Nullable** |
| -------------------- | ------------------ | ------------ |
| defaultSecurityRules | List<SecurityRule> | &check;      |
| etag                 | String             | &check;      |
| flowLogs             | List<FlowLog>      | &check;      |
| id                   | String             | &cross;      |
| location             | String             | &check;      |
| name                 | String             | &check;      |
| networkInterfaces    | List<String>       | &check;      |
| provisioningState    | String             | &check;      |
| resourceGuid         | String             | &check;      |
| securityRules        | List<SecurityRule> | &check;      |
| tags                 | Map<String,String> | &check;      |
| type                 | String             | &check;      |

#### PrivateEndpoint
| **Name**                            | **Type**                             | **Nullable** |
| ----------------------------------- | ------------------------------------ | ------------ |
| applicationSecurityGroups           | List<ApplicationSecurityGroup>       | &check;      |
| customDnsConfigs                    | List<CustomConfigPropertiesFormat>   | &check;      |
| customNetworkInterfaceName          | String                               | &check;      |
| etag                                | String                               | &check;      |
| extendedLocation                    | ExtendedLocation                     | &check;      |
| id                                  | String                               | &cross;      |
| ipConfigurations                    | List<PrivateEndpointIpConfiguration> | &check;      |
| location                            | String                               | &check;      |
| manualPrivateLinkServiceConnections | List<PrivateLinkServiceConnection>   | &check;      |
| name                                | String                               | &check;      |
| privateLinkServiceConnections       | List<PrivateLinkServiceConnection>   | &check;      |
| provisioningState                   | String                               | &check;      |
| tags                                | Map<String,String>                   | &check;      |
| type                                | String                               | &check;      |

#### PrivateEndpointIpConfiguration
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| etag             | String   | &check;      |
| groupId          | String   | &check;      |
| memberName       | String   | &check;      |
| name             | String   | &check;      |
| privateIpAddress | String   | &check;      |
| type             | String   | &check;      |

#### PrivateLinkServiceConnection
| **Name**                          | **Type**                          | **Nullable** |
| --------------------------------- | --------------------------------- | ------------ |
| etag                              | String                            | &check;      |
| groupIds                          | List<String>                      | &check;      |
| id                                | String                            | &cross;      |
| name                              | String                            | &cross;      |
| privateLinkServiceConnectionState | PrivateLinkServiceConnectionState | &check;      |
| privateLinkServiceId              | String                            | &check;      |
| provisioningState                 | String                            | &check;      |
| requestMessage                    | String                            | &check;      |
| type                              | String                            | &cross;      |

#### PrivateLinkServiceConnectionState
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| actionsRequired | String   | &check;      |
| description     | String   | &check;      |
| status          | String   | &check;      |

#### Route
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| addressPrefix     | String   | &check;      |
| etag              | String   | &check;      |
| hasBgpOverride    | Boolean  | &check;      |
| id                | String   | &cross;      |
| name              | String   | &check;      |
| nextHopIpAddress  | String   | &check;      |
| nextHopType       | String   | &check;      |
| provisioningState | String   | &check;      |
| type              | String   | &check;      |

#### RouteTable
| **Name**                   | **Type**           | **Nullable** |
| -------------------------- | ------------------ | ------------ |
| disableBgpRoutePropagation | Boolean            | &check;      |
| id                         | String             | &cross;      |
| location                   | String             | &check;      |
| name                       | String             | &check;      |
| provisioningState          | String             | &check;      |
| resourceGuid               | String             | &check;      |
| routes                     | List<Route>        | &check;      |
| tags                       | Map<String,String> | &check;      |
| type                       | String             | &check;      |

#### SecurityRule
| **Name**                             | **Type**                       | **Nullable** |
| ------------------------------------ | ------------------------------ | ------------ |
| access                               | String                         | &check;      |
| description                          | String                         | &check;      |
| destinationAddressPrefix             | String                         | &check;      |
| destinationAddressPrefixes           | List<String>                   | &check;      |
| destinationApplicationSecurityGroups | List<ApplicationSecurityGroup> | &check;      |
| destinationPortRange                 | String                         | &check;      |
| destinationPortRanges                | List<String>                   | &check;      |
| direction                            | String                         | &check;      |
| etag                                 | String                         | &check;      |
| id                                   | String                         | &cross;      |
| name                                 | String                         | &check;      |
| priority                             | Int                            | &check;      |
| protocol                             | String                         | &check;      |
| provisioningState                    | String                         | &check;      |
| sourceAddressPrefix                  | String                         | &check;      |
| sourceAddressPrefixes                | List<String>                   | &check;      |
| sourceApplicationSecurityGroups      | List<ApplicationSecurityGroup> | &check;      |
| sourcePortRange                      | String                         | &check;      |
| sourcePortRanges                     | List<String>                   | &check;      |
| type                                 | String                         | &check;      |

#### ServiceEndpoint
| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| locations         | List<String> | &check;      |
| provisioningState | String       | &check;      |
| service           | String       | &cross;      |

#### ServiceEndpointPolicy
| **Name**                          | **Type**                              | **Nullable** |
| --------------------------------- | ------------------------------------- | ------------ |
| contextualServiceEndpointPolicies | List<String>                          | &check;      |
| etag                              | String                                | &check;      |
| id                                | String                                | &cross;      |
| kind                              | String                                | &check;      |
| location                          | String                                | &check;      |
| name                              | String                                | &check;      |
| provisioningState                 | String                                | &check;      |
| resourceGuid                      | String                                | &check;      |
| serviceAlias                      | String                                | &check;      |
| serviceEndpointPolicyDefinitions  | List<ServiceEndpointPolicyDefinition> | &check;      |
| tags                              | Map<String,String>                    | &check;      |
| type                              | String                                | &check;      |

#### ServiceEndpointPolicyDefinition
| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| description       | String       | &check;      |
| etag              | String       | &check;      |
| id                | String       | &cross;      |
| name              | String       | &check;      |
| provisioningState | String       | &check;      |
| service           | String       | &check;      |
| serviceResources  | List<String> | &check;      |
| type              | String       | &check;      |

#### Subnet
| **Name**                           | **Type**                    | **Nullable** |
| ---------------------------------- | --------------------------- | ------------ |
| addressPrefix                      | String                      | &check;      |
| addressPrefixes                    | List<String>                | &check;      |
| applicationGatewayIpConfigurations | List<String>                | &check;      |
| etag                               | String                      | &check;      |
| id                                 | String                      | &cross;      |
| ipAllocations                      | List<String>                | &check;      |
| ipConfigurationProfiles            | List<String>                | &check;      |
| ipConfigurations                   | List<IpConfiguration>       | &check;      |
| name                               | String                      | &check;      |
| natGatewayId                       | String                      | &check;      |
| networkSecurityGroup               | NetworkSecurityGroup        | &check;      |
| privateEndpointNetworkPolicies     | String                      | &check;      |
| privateEndpoints                   | List<PrivateEndpoint>       | &check;      |
| privateLinkServiceNetworkPolicies  | String                      | &check;      |
| provisioningState                  | String                      | &check;      |
| purpose                            | String                      | &check;      |
| resourceNavigationLinks            | List<Link>                  | &check;      |
| routeTable                         | RouteTable                  | &check;      |
| serviceAssociationLinks            | List<Link>                  | &check;      |
| serviceEndpointPolicies            | List<ServiceEndpointPolicy> | &check;      |
| serviceEndpoints                   | List<ServiceEndpoint>       | &check;      |
| type                               | String                      | &check;      |

#### VirtualNetworkBgpCommunities
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| regionalCommunity       | String   | &check;      |
| virtualNetworkCommunity | String   | &check;      |

#### VirtualNetworkPeering
| **Name**                                  | **Type**                     | **Nullable** |
| ----------------------------------------- | ---------------------------- | ------------ |
| allowForwardedTraffic                     | Boolean                      | &check;      |
| allowGatewayTransit                       | Boolean                      | &check;      |
| allowVirtualNetworkAccess                 | Boolean                      | &check;      |
| doNotVerifyRemoteGateways                 | Boolean                      | &check;      |
| etag                                      | String                       | &check;      |
| id                                        | String                       | &cross;      |
| name                                      | String                       | &check;      |
| peeringState                              | String                       | &check;      |
| peeringSyncLevel                          | String                       | &check;      |
| provisioningState                         | String                       | &check;      |
| remoteAddressSpacePrefixes                | List<String>                 | &check;      |
| remoteBgpCommunities                      | VirtualNetworkBgpCommunities | &check;      |
| remoteVirtualNetworkAddressSpacePrefixes  | List<String>                 | &check;      |
| remoteVirtualNetworkEncryptionEnabled     | Boolean                      | &check;      |
| remoteVirtualNetworkEncryptionEnforcement | String                       | &check;      |
| remoteVirtualNetworkId                    | String                       | &check;      |
| resourceGuid                              | String                       | &check;      |
| type                                      | String                       | &check;      |
| useRemoteGateways                         | Boolean                      | &check;      |
