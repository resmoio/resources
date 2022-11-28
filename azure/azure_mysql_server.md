---
description: Azure MySql Server
---
azure_mysql_server
------------------

| **Name**                   | **Type**                        | **Nullable** |
| -------------------------- | ------------------------------- | ------------ |
| administratorLogin         | String                          | &check;      |
| byokEnforcement            | String                          | &check;      |
| configurations             | List<Configuration>             | &check;      |
| fullyQualifiedDomainName   | String                          | &check;      |
| id                         | String                          | &cross;      |
| identity                   | Identity                        | &check;      |
| infrastructureEncryption   | String                          | &check;      |
| location                   | String                          | &cross;      |
| masterServerId             | String                          | &check;      |
| minimalTlsVersion          | String                          | &check;      |
| name                       | String                          | &cross;      |
| privateEndpointConnections | List<PrivateEndpointConnection> | &check;      |
| publicNetworkAccess        | String                          | &check;      |
| region                     | String                          | &check;      |
| replicaCapacity            | Int                             | &check;      |
| replicationRole            | String                          | &check;      |
| resourceGroupName          | String                          | &cross;      |
| sku                        | String                          | &check;      |
| sslEnforcement             | String                          | &check;      |
| storageProfile             | StorageProfile                  | &check;      |
| subscriptionId             | String                          | &cross;      |
| tags                       | Map<String,String>              | &check;      |
| type                       | String                          | &cross;      |
| userVisibleState           | String                          | &check;      |
| version                    | String                          | &check;      |

#### Configuration
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| allowedValues | String   | &check;      |
| dataType      | String   | &check;      |
| defaultValue  | String   | &check;      |
| description   | String   | &check;      |
| id            | String   | &cross;      |
| name          | String   | &check;      |
| source        | String   | &check;      |
| type          | String   | &check;      |
| value         | String   | &check;      |

#### Identity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| principalId | String   | &check;      |
| tenantId    | String   | &check;      |
| type        | String   | &check;      |

#### PrivateEndpointConnection
| **Name**                          | **Type**                          | **Nullable** |
| --------------------------------- | --------------------------------- | ------------ |
| id                                | String                            | &cross;      |
| privateEndpointId                 | String                            | &check;      |
| privateLinkServiceConnectionState | PrivateLinkServiceConnectionState | &check;      |
| provisioningState                 | String                            | &check;      |

#### PrivateLinkServiceConnectionState
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| actionsRequired | String   | &check;      |
| description     | String   | &check;      |
| status          | String   | &check;      |

#### StorageProfile
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| backupRetentionDays | Int      | &check;      |
| geoRedundantBackup  | String   | &check;      |
| storageAutogrow     | String   | &check;      |
| storageMB           | Int      | &check;      |
