---
description: Azure Network Interface
---
azure_network_interface
-----------------------

| **Name**                    | **Type**                              | **Nullable** |
| --------------------------- | ------------------------------------- | ------------ |
| dnsSettings                 | NetworkInterfaceDnsSettings           | &check;      |
| dscpConfigurationId         | String                                | &check;      |
| enableAcceleratedNetworking | Boolean                               | &check;      |
| enableIPForwarding          | Boolean                               | &check;      |
| etag                        | String                                | &check;      |
| extendedLocation            | ExtendedLocation                      | &check;      |
| hostedWorkLoads             | List<String>                          | &check;      |
| id                          | String                                | &cross;      |
| ipConfigurations            | List<NetworkInterfaceIpConfiguration> | &check;      |
| location                    | String                                | &cross;      |
| macAddress                  | String                                | &check;      |
| migrationPhase              | String                                | &check;      |
| name                        | String                                | &cross;      |
| nicType                     | String                                | &check;      |
| primary                     | Boolean                               | &check;      |
| primaryIPConfiguration      | NetworkInterfaceIpConfiguration       | &check;      |
| privateEndpoint             | PrivateEndpoint                       | &check;      |
| privateLinkService          | PrivateLinkService                    | &check;      |
| provisioningState           | String                                | &check;      |
| resourceGroupName           | String                                | &cross;      |
| resourceGuid                | String                                | &check;      |
| subscriptionId              | String                                | &cross;      |
| tags                        | Map<String,String>                    | &check;      |
| tapConfigurations           | List<VirtualNetworkTap>               | &check;      |
| type                        | String                                | &cross;      |
| virtualMachineId            | String                                | &check;      |
| vnetEncryptionSupported     | Boolean                               | &check;      |
| workloadType                | String                                | &check;      |

#### ApplicationGatewayBackendAddress
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| fqdn      | String   | &check;      |
| ipAddress | String   | &check;      |

#### ApplicationGatewayBackendAddressPool
| **Name**                | **Type**                               | **Nullable** |
| ----------------------- | -------------------------------------- | ------------ |
| backendAddress          | List<ApplicationGatewayBackendAddress> | &check;      |
| backendIpConfigurations | List<String>                           | &check;      |
| etag                    | String                                 | &check;      |
| id                      | String                                 | &cross;      |
| name                    | String                                 | &check;      |
| provisioningState       | String                                 | &check;      |
| type                    | String                                 | &check;      |

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

#### BackendAddressPool
| **Name**                     | **Type**                         | **Nullable** |
| ---------------------------- | -------------------------------- | ------------ |
| etag                         | String                           | &check;      |
| id                           | String                           | &cross;      |
| inboundNatRules              | List<String>                     | &check;      |
| loadBalancerBackendAddresses | List<LoadBalancerBackendAddress> | &check;      |
| loadBalancingRules           | List<String>                     | &check;      |
| location                     | String                           | &check;      |
| name                         | String                           | &check;      |
| outboundRule                 | String                           | &check;      |
| outboundRules                | List<String>                     | &check;      |
| provisioningState            | String                           | &check;      |
| tunnelInterfaces             | List<GatewayLoadBalancerTunnel>  | &check;      |
| type                         | String                           | &check;      |

#### CustomConfigPropertiesFormat
| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| fqdn        | String       | &check;      |
| ipAddresses | List<String> | &check;      |

#### DdosSettings
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| ddosProtectionPlan | String   | &check;      |
| protectionMode     | String   | &check;      |

#### ExtendedLocation
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### FrontendIpConfiguration
| **Name**                  | **Type**        | **Nullable** |
| ------------------------- | --------------- | ------------ |
| etag                      | String          | &check;      |
| gatewayLoadBalancerId     | String          | &check;      |
| id                        | String          | &cross;      |
| inboundNatPools           | List<String>    | &check;      |
| inboundNatRules           | List<String>    | &check;      |
| loadBalancingRules        | List<String>    | &check;      |
| name                      | String          | &cross;      |
| outboundRules             | List<String>    | &check;      |
| privateIpAddress          | String          | &check;      |
| privateIpAddressVersion   | String          | &check;      |
| privateIpAllocationMethod | String          | &check;      |
| provisioningState         | String          | &check;      |
| publicIpAddress           | PublicIpAddress | &check;      |
| publicIpPrefix            | String          | &check;      |
| type                      | String          | &cross;      |

#### GatewayLoadBalancerTunnel
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| identifier | Int      | &check;      |
| port       | Int      | &check;      |
| protocol   | String   | &check;      |
| type       | String   | &check;      |

#### InboundNatRule
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| backendAddressPoolId      | String   | &check;      |
| backendPort               | Int      | &check;      |
| enableFloatingIP          | Boolean  | &check;      |
| enableTcpReset            | Boolean  | &check;      |
| etag                      | String   | &check;      |
| frontendIpConfigurationId | String   | &check;      |
| frontendPort              | Int      | &check;      |
| frontendPortRangeEnd      | Int      | &check;      |
| frontendPortRangeStart    | Int      | &check;      |
| id                        | String   | &cross;      |
| idleTimeoutInMinutes      | Int      | &check;      |
| name                      | String   | &check;      |
| protocol                  | String   | &check;      |
| provisioningState         | String   | &check;      |
| type                      | String   | &check;      |

#### IpConfiguration
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| etag              | String   | &check;      |
| id                | String   | &check;      |
| name              | String   | &check;      |
| privateIpAddress  | String   | &check;      |
| provisioningState | String   | &check;      |

#### LoadBalancerBackendAddress
| **Name**                              | **Type**                 | **Nullable** |
| ------------------------------------- | ------------------------ | ------------ |
| inboundNatRulesPortMapping            | List<NatRulePortMapping> | &check;      |
| ipAddress                             | String                   | &check;      |
| loadBalancerFrontendIpConfigurationId | String                   | &check;      |
| name                                  | String                   | &check;      |
| networkInterfaceIpConfigurationId     | String                   | &check;      |
| subnetId                              | String                   | &check;      |
| virtualNetworkId                      | String                   | &check;      |

#### NatGateway
| **Name**             | **Type**           | **Nullable** |
| -------------------- | ------------------ | ------------ |
| etag                 | String             | &check;      |
| id                   | String             | &cross;      |
| idleTimeoutInMinutes | Int                | &check;      |
| name                 | String             | &check;      |
| provisioningState    | String             | &check;      |
| publicIpAddresses    | List<String>       | &check;      |
| publicIpPrefixes     | List<String>       | &check;      |
| resourceGuid         | String             | &check;      |
| skuName              | String             | &check;      |
| tags                 | Map<String,String> | &check;      |
| type                 | String             | &check;      |
| zones                | List<String>       | &check;      |

#### NatRulePortMapping
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| backendPort        | Int      | &check;      |
| frontendPort       | Int      | &check;      |
| inboundNatRuleName | String   | &check;      |

#### NetworkInterfaceDnsSettings
| **Name**                 | **Type**     | **Nullable** |
| ------------------------ | ------------ | ------------ |
| appliedDnsServers        | List<String> | &check;      |
| dnsServers               | List<String> | &check;      |
| internalDnsNameLabel     | String       | &check;      |
| internalDomainNameSuffix | String       | &check;      |
| internalFqdn             | String       | &check;      |

#### NetworkInterfaceIpConfiguration
| **Name**                              | **Type**                                   | **Nullable** |
| ------------------------------------- | ------------------------------------------ | ------------ |
| applicationGatewayBackendAddressPools | List<ApplicationGatewayBackendAddressPool> | &check;      |
| applicationSecurityGroups             | List<ApplicationSecurityGroup>             | &check;      |
| etag                                  | String                                     | &check;      |
| gatewayLoadBalancerId                 | String                                     | &check;      |
| id                                    | String                                     | &cross;      |
| loadBalancerBackendAddressPools       | List<BackendAddressPool>                   | &check;      |
| loadBalancerInboundNatRules           | List<InboundNatRule>                       | &check;      |
| name                                  | String                                     | &check;      |
| primary                               | Boolean                                    | &check;      |
| privateIpAddress                      | String                                     | &check;      |
| privateIpAddressVersion               | String                                     | &check;      |
| privateIpAllocationMethod             | String                                     | &check;      |
| privateLinkConnectionProperties       | PrivateLinkConnectionProperties            | &check;      |
| provisioningState                     | String                                     | &check;      |
| publicIpAddress                       | PublicIpAddress                            | &check;      |
| subnetId                              | String                                     | &check;      |
| type                                  | String                                     | &check;      |
| virtualNetworkTaps                    | List<VirtualNetworkTap>                    | &check;      |

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

#### PrivateLinkConnectionProperties
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| fqdns              | List<String> | &check;      |
| groupId            | String       | &check;      |
| requiredMemberName | String       | &check;      |

#### PrivateLinkService
| **Name**                             | **Type**                             | **Nullable** |
| ------------------------------------ | ------------------------------------ | ------------ |
| alias                                | String                               | &check;      |
| autoApprovalSubscriptions            | List<String>                         | &check;      |
| enableProxyProtocol                  | Boolean                              | &check;      |
| etag                                 | String                               | &check;      |
| extendedLocation                     | ExtendedLocation                     | &check;      |
| fqdns                                | List<String>                         | &check;      |
| id                                   | String                               | &cross;      |
| ipConfigurations                     | List<PrivateEndpointIpConfiguration> | &check;      |
| loadBalancerFrontendIpConfigurations | List<FrontendIpConfiguration>        | &check;      |
| location                             | String                               | &cross;      |
| name                                 | String                               | &cross;      |
| provisioningState                    | String                               | &check;      |
| tags                                 | Map<String,String>                   | &check;      |
| type                                 | String                               | &cross;      |
| visibilitySubscriptions              | List<String>                         | &check;      |

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

#### PublicIpAddress
| **Name**                 | **Type**                   | **Nullable** |
| ------------------------ | -------------------------- | ------------ |
| ddosSettings             | DdosSettings               | &check;      |
| deleteOption             | String                     | &check;      |
| dnsSettings              | PublicIpAddressDnsSettings | &check;      |
| etag                     | String                     | &check;      |
| extendedLocation         | ExtendedLocation           | &check;      |
| id                       | String                     | &cross;      |
| idleTimeoutInMinutes     | Int                        | &check;      |
| ipAddress                | String                     | &check;      |
| ipConfiguration          | IpConfiguration            | &check;      |
| ipTags                   | Map<String,String>         | &check;      |
| linkedPublicIPAddressId  | String                     | &check;      |
| migrationPhase           | String                     | &check;      |
| name                     | String                     | &check;      |
| natGateway               | NatGateway                 | &check;      |
| provisioningState        | String                     | &check;      |
| publicIpAddressVersion   | String                     | &check;      |
| publicIpAllocationMethod | String                     | &check;      |
| publicIpPrefixId         | String                     | &check;      |
| servicePublicIPAddressId | String                     | &check;      |
| sku                      | Sku                        | &check;      |
| tags                     | Map<String,String>         | &check;      |
| type                     | String                     | &check;      |
| zones                    | List<String>               | &check;      |

#### PublicIpAddressDnsSettings
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| domainNameLabel | String   | &check;      |
| fqdn            | String   | &check;      |
| reverseFqdn     | String   | &check;      |

#### Sku
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| tier     | String   | &check;      |

#### VirtualNetworkTap
| **Name**                                       | **Type**                             | **Nullable** |
| ---------------------------------------------- | ------------------------------------ | ------------ |
| destinationLoadBalancerFrontEndIpConfiguration | FrontendIpConfiguration              | &check;      |
| destinationNetworkInterfaceIpConfigurationId   | String                               | &check;      |
| destinationPort                                | Int                                  | &check;      |
| etag                                           | String                               | &check;      |
| id                                             | String                               | &cross;      |
| location                                       | String                               | &check;      |
| name                                           | String                               | &cross;      |
| networkInterfaceTapConfigurations              | List<VirtualNetworkTapConfiguration> | &check;      |
| provisioningState                              | String                               | &check;      |
| resourceGuid                                   | String                               | &check;      |
| tags                                           | Map<String,String>                   | &check;      |
| type                                           | String                               | &cross;      |

#### VirtualNetworkTapConfiguration
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| etag              | String   | &check;      |
| id                | String   | &cross;      |
| name              | String   | &cross;      |
| provisioningState | String   | &check;      |
| type              | String   | &cross;      |
