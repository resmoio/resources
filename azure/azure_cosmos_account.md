---
description: Azure Cosmos Account
---
azure_cosmos_account
--------------------

| **Name**                            | **Type**                        | **Nullable** |
| ----------------------------------- | ------------------------------- | ------------ |
| analyticalStorageSchemaType         | String                          | &check;      |
| apiServerVersion                    | String                          | &check;      |
| backupPolicy                        | JSON                            | &check;      |
| capabilities                        | List<String>                    | &check;      |
| cassandraConnectorEnabled           | Boolean                         | &check;      |
| cassandraConnectorOffer             | String                          | &check;      |
| consistencyPolicy                   | ConsistencyPolicy               | &check;      |
| cors                                | List<CorsPolicy>                | &check;      |
| createMode                          | String                          | &check;      |
| databaseAccountOfferType            | String                          | &check;      |
| defaultIdentity                     | String                          | &check;      |
| disableLocalAuth                    | Boolean                         | &check;      |
| documentEndpoint                    | String                          | &cross;      |
| enableAnalyticalStorage             | Boolean                         | &check;      |
| enableAutomaticFailover             | Boolean                         | &check;      |
| enableFreeTier                      | Boolean                         | &check;      |
| failoverPolicies                    | List<FailoverPolicy>            | &check;      |
| id                                  | String                          | &cross;      |
| identity                            | Identity                        | &check;      |
| instanceId                          | String                          | &check;      |
| ipRules                             | List<String>                    | &check;      |
| isVirtualNetworkFilterEnabled       | Boolean                         | &check;      |
| keyBasedMetadataWriteAccessDisabled | Boolean                         | &check;      |
| keyVaultKeyUri                      | String                          | &check;      |
| kind                                | String                          | &check;      |
| location                            | String                          | &cross;      |
| locations                           | List<Location>                  | &check;      |
| multipleWriteLocationsEnabled       | Boolean                         | &check;      |
| name                                | String                          | &cross;      |
| networkAclBypass                    | String                          | &check;      |
| networkAclBypassResourceIds         | List<String>                    | &check;      |
| privateEndpointConnections          | List<PrivateEndpointConnection> | &check;      |
| privateLinkResources                | List<PrivateLinkResource>       | &check;      |
| provisioningState                   | String                          | &check;      |
| publicAccessNetwork                 | String                          | &check;      |
| readableReplications                | List<Location>                  | &check;      |
| resourceGroupName                   | String                          | &cross;      |
| restoreParameters                   | RestoreParameters               | &check;      |
| sqlDatabases                        | List<SqlDatabase>               | &check;      |
| subscriptionId                      | String                          | &cross;      |
| systemData                          | SystemData                      | &check;      |
| tags                                | Map<String,String>              | &check;      |
| totalThroughputLimit                | Int                             | &check;      |
| type                                | String                          | &cross;      |
| virtualNetworkRules                 | List<VirtualNetworkRule>        | &check;      |
| writableReplications                | List<Location>                  | &check;      |

#### ConsistencyPolicy
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| defaultConsistencyLevel | String   | &check;      |
| maxIntervalInSeconds    | Int      | &check;      |
| maxStalenessPrefix      | Long     | &check;      |

#### CorsPolicy
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| allowedHeaders  | String   | &check;      |
| allowedMethods  | String   | &check;      |
| allowedOrigins  | String   | &check;      |
| exposedHeaders  | String   | &check;      |
| maxAgeInSeconds | Long     | &check;      |

#### FailoverPolicy
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| failoverPriority | Int      | &check;      |
| id               | String   | &check;      |
| locationName     | String   | &check;      |

#### Identity
| **Name**               | **Type**                         | **Nullable** |
| ---------------------- | -------------------------------- | ------------ |
| principalId            | String                           | &check;      |
| tenantId               | String                           | &check;      |
| type                   | String                           | &check;      |
| userAssignedIdentities | Map<String,UserAssignedIdentity> | &check;      |

#### Keys
| **Name**                   | **Type** | **Nullable** |
| -------------------------- | -------- | ------------ |
| primaryMasterKey           | String   | &cross;      |
| primaryReadonlyMasterKey   | String   | &cross;      |
| secondaryMasterKey         | String   | &cross;      |
| secondaryReadonlyMasterKey | String   | &cross;      |

#### Location
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| documentEndpoint  | String   | &check;      |
| failoverPriority  | Int      | &check;      |
| id                | String   | &check;      |
| isZoneRedundant   | Boolean  | &check;      |
| locationName      | String   | &check;      |
| provisioningState | String   | &check;      |

#### PrivateEndpointConnection
| **Name**                          | **Type**                          | **Nullable** |
| --------------------------------- | --------------------------------- | ------------ |
| groupId                           | String                            | &cross;      |
| id                                | String                            | &cross;      |
| name                              | String                            | &cross;      |
| privateEndpointId                 | String                            | &check;      |
| privateLinkServiceConnectionState | PrivateLinkServiceConnectionState | &check;      |
| provisioningState                 | String                            | &check;      |

#### PrivateLinkResource
| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| groupId           | String       | &check;      |
| id                | String       | &check;      |
| name              | String       | &check;      |
| requiredMembers   | List<String> | &check;      |
| requiredZoneNames | List<String> | &check;      |
| type              | String       | &check;      |

#### PrivateLinkServiceConnectionState
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| actionsRequired | String   | &check;      |
| description     | String   | &check;      |
| status          | String   | &check;      |

#### RestoreParameters
| **Name**              | **Type**              | **Nullable** |
| --------------------- | --------------------- | ------------ |
| databasesToRestore    | List<RestoreResource> | &check;      |
| restoreMode           | String                | &check;      |
| restoreSource         | String                | &check;      |
| restoreTimestampInUtc | String                | &check;      |

#### RestoreResource
| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| collectionNames | List<String> | &check;      |
| databaseName    | String       | &check;      |

#### SqlDatabase
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| colls         | String   | &check;      |
| etag          | String   | &check;      |
| rid           | String   | &check;      |
| sqlDatabaseId | String   | &check;      |
| ts            | String   | &check;      |
| users         | String   | &check;      |

#### SystemData
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| createdAt          | String   | &check;      |
| createdBy          | String   | &check;      |
| createdByType      | String   | &check;      |
| lastModifiedAt     | String   | &check;      |
| lastModifiedBy     | String   | &check;      |
| lastModifiedByType | String   | &check;      |

#### UserAssignedIdentity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| clientId    | String   | &check;      |
| principalId | String   | &check;      |

#### VirtualNetworkRule
| **Name**                         | **Type** | **Nullable** |
| -------------------------------- | -------- | ------------ |
| id                               | String   | &check;      |
| ignoreMissingVNetServiceEndpoint | Boolean  | &check;      |
