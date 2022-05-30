---
description: Azure Network Watcher
---
azure_network_watcher
---------------------

| **Name**           | **Type**                | **Nullable** |
| ------------------ | ----------------------- | ------------ |
| connectionMonitors | List<ConnectionMonitor> | &check;      |
| etag               | String                  | &check;      |
| id                 | String                  | &cross;      |
| location           | String                  | &cross;      |
| name               | String                  | &cross;      |
| packetCaptures     | List<PacketCapture>     | &check;      |
| provisioningState  | String                  | &check;      |
| resourceGroupName  | String                  | &cross;      |
| subscriptionId     | String                  | &cross;      |
| tags               | Map<String,String>      | &check;      |
| type               | String                  | &cross;      |

#### ConnectionMonitor
| **Name**                    | **Type**                                 | **Nullable** |
| --------------------------- | ---------------------------------------- | ------------ |
| autoStart                   | Boolean                                  | &check;      |
| connectionMonitorType       | String                                   | &check;      |
| destination                 | ConnectionMonitorDestination             | &check;      |
| destinationAddress          | String                                   | &check;      |
| destinationPort             | Int                                      | &check;      |
| destinationResourceId       | String                                   | &check;      |
| endpoints                   | List<ConnectionMonitorEndpoint>          | &check;      |
| etag                        | String                                   | &check;      |
| id                          | String                                   | &cross;      |
| location                    | String                                   | &check;      |
| monitoringIntervalInSeconds | Int                                      | &check;      |
| monitoringStatus            | String                                   | &check;      |
| name                        | String                                   | &cross;      |
| notes                       | String                                   | &check;      |
| outputs                     | List<ConnectionMonitorOutput>            | &check;      |
| provisioningState           | String                                   | &check;      |
| source                      | ConnectionMonitorSource                  | &check;      |
| sourcePort                  | Int                                      | &check;      |
| sourceResourceId            | String                                   | &check;      |
| startTime                   | String                                   | &check;      |
| tags                        | Map<String,String>                       | &check;      |
| testConfigurations          | List<ConnectionMonitorTestConfiguration> | &check;      |
| testGroups                  | List<ConnectionMonitorTestGroup>         | &check;      |

#### ConnectionMonitorDestination
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| address    | String   | &check;      |
| port       | Int      | &check;      |
| resourceId | String   | &check;      |

#### ConnectionMonitorEndpoint
| **Name**            | **Type**                      | **Nullable** |
| ------------------- | ----------------------------- | ------------ |
| address             | String                        | &check;      |
| coverageLevel       | String                        | &check;      |
| filterType          | String                        | &check;      |
| filters             | List<ConnectionMonitorFilter> | &check;      |
| name                | String                        | &check;      |
| resourceId          | String                        | &check;      |
| scopeExcludeAddress | List<String>                  | &check;      |
| scopeIncludeAddress | List<String>                  | &check;      |
| type                | String                        | &check;      |

#### ConnectionMonitorFilter
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| address  | String   | &check;      |
| type     | String   | &check;      |

#### ConnectionMonitorOutput
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| type                | String   | &check;      |
| workspaceResourceId | String   | &check;      |

#### ConnectionMonitorSource
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| port       | Int      | &check;      |
| resourceId | String   | &check;      |

#### ConnectionMonitorSuccessThreshold
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| checksFailedPercent | Int      | &check;      |
| roundTripTimeMs     | Double   | &check;      |

#### ConnectionMonitorTestConfiguration
| **Name**           | **Type**                          | **Nullable** |
| ------------------ | --------------------------------- | ------------ |
| httpConfiguration  | JSON                              | &check;      |
| icmpConfiguration  | JSON                              | &check;      |
| name               | String                            | &check;      |
| preferredIpVersion | String                            | &check;      |
| protocol           | String                            | &check;      |
| successThreshold   | ConnectionMonitorSuccessThreshold | &check;      |
| tcpConfiguration   | JSON                              | &check;      |
| testFrequencySec   | Int                               | &check;      |

#### ConnectionMonitorTestGroup
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| destinations       | List<String> | &check;      |
| disable            | Boolean      | &check;      |
| name               | String       | &check;      |
| sources            | List<String> | &check;      |
| testConfigurations | List<String> | &check;      |

#### PacketCapture
| **Name**                | **Type**                     | **Nullable** |
| ----------------------- | ---------------------------- | ------------ |
| bytesToCapturePerPacket | Long                         | &check;      |
| etag                    | String                       | &check;      |
| filters                 | List<PacketCaptureFilter>    | &check;      |
| id                      | String                       | &cross;      |
| name                    | String                       | &cross;      |
| provisioningState       | String                       | &check;      |
| storageLocation         | PacketCaptureStorageLocation | &check;      |
| targetId                | String                       | &check;      |
| timeLimitInSeconds      | Int                          | &check;      |
| totalBytesPerSession    | Long                         | &check;      |

#### PacketCaptureFilter
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| localIPAddress  | String   | &check;      |
| localPort       | String   | &cross;      |
| protocol        | String   | &check;      |
| remoteIPAddress | String   | &check;      |
| remotePort      | String   | &cross;      |

#### PacketCaptureStorageLocation
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| filePath    | String   | &check;      |
| storageId   | String   | &check;      |
| storagePath | String   | &check;      |
