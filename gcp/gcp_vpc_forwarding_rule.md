---
description: Google Cloud Platform VPC Forwarding Rule
---
gcp_vpc_forwarding_rule
-----------------------

| **Name**                      | **Type**                                         | **Nullable** |
| ----------------------------- | ------------------------------------------------ | ------------ |
| IPAddress                     | String                                           | &check;      |
| IPProtocol                    | String                                           | &check;      |
| allPorts                      | Boolean                                          | &check;      |
| allowGlobalAccess             | Boolean                                          | &check;      |
| backendService                | String                                           | &check;      |
| creationTimestamp             | String                                           | &check;      |
| description                   | String                                           | &check;      |
| id                            | String                                           | &cross;      |
| ipVersion                     | String                                           | &check;      |
| isMirroringCollector          | String                                           | &check;      |
| kind                          | String                                           | &check;      |
| labels                        | Map<String,String>                               | &check;      |
| loadBalancingScheme           | String                                           | &check;      |
| metadataFilters               | List<MetadataFilter>                             | &check;      |
| name                          | String                                           | &check;      |
| network                       | String                                           | &check;      |
| networkTier                   | String                                           | &check;      |
| portRange                     | String                                           | &check;      |
| ports                         | List<String>                                     | &check;      |
| project                       | String                                           | &cross;      |
| pscConnectionId               | String                                           | &check;      |
| pscConnectionStatus           | String                                           | &check;      |
| region                        | String                                           | &check;      |
| serviceDirectoryRegistrations | List<ForwardingRuleServiceDirectoryRegistration> | &check;      |
| serviceLabel                  | String                                           | &check;      |
| serviceName                   | String                                           | &check;      |
| subnetwork                    | String                                           | &check;      |
| target                        | String                                           | &check;      |

#### ForwardingRuleServiceDirectoryRegistration
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| namespace              | String   | &check;      |
| service                | String   | &check;      |
| serviceDirectoryRegion | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### MetadataFilter
| **Name**            | **Type**                       | **Nullable** |
| ------------------- | ------------------------------ | ------------ |
| filterLabels        | List<MetadataFilterLabelMatch> | &check;      |
| filterMatchCriteria | String                         | &check;      |

#### MetadataFilterLabelMatch
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| value    | String   | &check;      |
