---
description: Azure Public IP Address
---
azure_public_ip_address
-----------------------

| **Name**                                | **Type**                | **Nullable** |
| --------------------------------------- | ----------------------- | ------------ |
| assignedLoadBalancerFrontend            | FrontendIpConfiguration | &check;      |
| assignedNetworkInterfaceIPConfiguration | NicIpConfiguration      | &check;      |
| availabilityZones                       | List<String>            | &check;      |
| ddosSettings                            | DdosSettings            | &check;      |
| deleteOption                            | String                  | &check;      |
| dnsSettings                             | DnsSettings             | &check;      |
| etag                                    | String                  | &check;      |
| extendedLocation                        | ExtendedLocation        | &check;      |
| fqdn                                    | String                  | &check;      |
| hasAssignedLoadBalancer                 | Boolean                 | &check;      |
| hasAssignedNetworkInterface             | Boolean                 | &check;      |
| id                                      | String                  | &cross;      |
| idleTimeoutInMinutes                    | Int                     | &check;      |
| ipAddress                               | String                  | &check;      |
| ipAllocationMethod                      | String                  | &check;      |
| ipConfiguration                         | IpConfiguration         | &check;      |
| ipTags                                  | List<IpTag>             | &check;      |
| leafDomainLabel                         | String                  | &check;      |
| linkedPublicIpAddress                   | String                  | &check;      |
| location                                | String                  | &cross;      |
| migrationPhase                          | String                  | &check;      |
| name                                    | String                  | &cross;      |
| natGateway                              | NatGateway              | &check;      |
| provisioningState                       | String                  | &check;      |
| publicIpPrefixId                        | String                  | &check;      |
| resourceGroupName                       | String                  | &cross;      |
| resourceGuid                            | String                  | &check;      |
| reverseFqdn                             | String                  | &check;      |
| servicePublicIpAddress                  | String                  | &check;      |
| sku                                     | Sku                     | &check;      |
| subscriptionId                          | String                  | &cross;      |
| tags                                    | Map<String,String>      | &check;      |
| type                                    | String                  | &cross;      |
| version                                 | String                  | &check;      |
| zones                                   | List<String>            | &check;      |

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

#### DdosSettings
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| ddosProtectionPlan | String   | &check;      |
| protectionMode     | String   | &check;      |

#### DnsSettings
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| domainNameLabel | String   | &check;      |
| fqdn            | String   | &check;      |
| reverseFqdn     | String   | &check;      |

#### ExtendedLocation
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### FrontendIpConfiguration
| **Name**                  | **Type**     | **Nullable** |
| ------------------------- | ------------ | ------------ |
| etag                      | String       | &check;      |
| gatewayLoadBalancerId     | String       | &check;      |
| id                        | String       | &cross;      |
| inboundNatPools           | List<String> | &check;      |
| inboundNatRules           | List<String> | &check;      |
| isPublic                  | Boolean      | &check;      |
| loadBalancingRules        | List<String> | &check;      |
| name                      | String       | &cross;      |
| outboundRules             | List<String> | &check;      |
| privateIpAddress          | String       | &check;      |
| privateIpAddressVersion   | String       | &check;      |
| privateIpAllocationMethod | String       | &check;      |
| provisioningState         | String       | &check;      |
| publicIpAddress           | String       | &check;      |
| publicIpPrefix            | String       | &check;      |
| subnetName                | String       | &check;      |
| type                      | String       | &cross;      |

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
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| etag                      | String   | &check;      |
| id                        | String   | &check;      |
| name                      | String   | &check;      |
| privateIpAddress          | String   | &check;      |
| privateIpAllocationMethod | String   | &check;      |
| provisioningState         | String   | &check;      |

#### IpTag
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| tag      | String   | &check;      |
| type     | String   | &check;      |

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

#### LoadBalancingRule
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| backendPort          | Int      | &check;      |
| etag                 | String   | &check;      |
| floatingIpEnabled    | Boolean  | &check;      |
| frontendPort         | Int      | &check;      |
| id                   | String   | &cross;      |
| idleTimeoutInMinutes | Int      | &check;      |
| loadDistribution     | String   | &check;      |
| name                 | String   | &cross;      |
| probe                | Probe    | &check;      |
| protocol             | String   | &check;      |
| type                 | String   | &cross;      |

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

#### NicIpConfiguration
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
| publicIpAddress                       | String                                     | &check;      |
| type                                  | String                                     | &check;      |
| virtualNetworkTaps                    | List<VirtualNetworkTap>                    | &check;      |

#### PrivateLinkConnectionProperties
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| fqdns              | List<String> | &check;      |
| groupId            | String       | &check;      |
| requiredMemberName | String       | &check;      |

#### PrivateLinkServiceConnectionState
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| actionsRequired | String   | &check;      |
| description     | String   | &check;      |
| status          | String   | &check;      |

#### Probe
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| etag              | String   | &check;      |
| id                | String   | &cross;      |
| intervalInSeconds | Int      | &check;      |
| name              | String   | &cross;      |
| numberOfProbes    | Int      | &check;      |
| type              | String   | &cross;      |

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
