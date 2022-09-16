---
description: Azure Storage Account
---
azure_storage_account
---------------------

| **Name**                                        | **Type**                              | **Nullable** |
| ----------------------------------------------- | ------------------------------------- | ------------ |
| accessTier                                      | String                                | &check;      |
| allowCrossTenantReplication                     | Boolean                               | &check;      |
| allowedCopyScope                                | String                                | &check;      |
| azureFilesIdentityBasedAuthentication           | AzureFilesIdentityBasedAuthentication | &check;      |
| blobRestoreStatus                               | BlobRestoreStatus                     | &check;      |
| canAccessFromAzureServices                      | Boolean                               | &check;      |
| canReadLogEntriesFromAnyNetwork                 | Boolean                               | &check;      |
| canReadMetricsFromAnyNetwork                    | Boolean                               | &check;      |
| creationTime                                    | String                                | &check;      |
| customDomain                                    | CustomDomain                          | &check;      |
| defaultToOAuthAuthentication                    | Boolean                               | &check;      |
| dnsEndpointType                                 | String                                | &check;      |
| encryption                                      | Encryption                            | &check;      |
| failoverInProgress                              | Boolean                               | &check;      |
| geoReplicationStats                             | GeoReplicationStats                   | &check;      |
| id                                              | String                                | &cross;      |
| immutableStorageWithVersioning                  | ImmutableStorageAccount               | &check;      |
| infrastructureEncryptionEnabled                 | Boolean                               | &check;      |
| ipAddressRangesWithAccess                       | List<String>                          | &check;      |
| ipAddressesWithAccess                           | List<String>                          | &check;      |
| isAccessAllowedFromAllNetworks                  | Boolean                               | &check;      |
| isAzureFilesAadIntegrationEnabled               | Boolean                               | &check;      |
| isBlobPublicAccessAllowed                       | Boolean                               | &check;      |
| isHnsEnabled                                    | Boolean                               | &check;      |
| isHttpsTrafficOnly                              | Boolean                               | &check;      |
| isLargeFileSharesEnabled                        | Boolean                               | &check;      |
| isLocalUserEnabled                              | Boolean                               | &check;      |
| isNfsV3Enabled                                  | Boolean                               | &check;      |
| isSftpEnabled                                   | Boolean                               | &check;      |
| isSharedKeyAccessAllowed                        | Boolean                               | &check;      |
| key1CreationTime                                | String                                | &check;      |
| key2CreationTime                                | String                                | &check;      |
| keyExpirationPeriodInDays                       | Int                                   | &check;      |
| kind                                            | String                                | &check;      |
| largeFileSharesState                            | String                                | &check;      |
| minimumTlsVersion                               | String                                | &check;      |
| name                                            | String                                | &cross;      |
| networkRuleSet                                  | NetworkRuleSet                        | &check;      |
| networkSubnetsWithAccess                        | List<String>                          | &check;      |
| primaryAccountStatus                            | String                                | &check;      |
| primaryEndpoints                                | Endpoints                             | &check;      |
| primaryLocation                                 | String                                | &check;      |
| privateEndpointConnections                      | List<PrivateEndpointConnection>       | &check;      |
| privateLinkResources                            | List<PrivateLinkResource>             | &check;      |
| provisioningState                               | String                                | &check;      |
| publicNetworkAccess                             | String                                | &check;      |
| resourceGroupName                               | String                                | &cross;      |
| routingReference                                | RoutingReference                      | &check;      |
| sasPolicy                                       | SasPolicy                             | &check;      |
| secondaryAccountStatus                          | String                                | &check;      |
| secondaryEndpoints                              | Endpoints                             | &check;      |
| secondaryLocation                               | String                                | &check;      |
| sku                                             | String                                | &check;      |
| subscriptionId                                  | String                                | &cross;      |
| systemAssignedManagedServiceIdentityPrincipalId | String                                | &check;      |
| systemAssignedManagedServiceIdentityTenantId    | String                                | &check;      |
| tags                                            | Map<String,String>                    | &check;      |
| type                                            | String                                | &cross;      |

#### ActiveDirectoryProperties
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| accountType       | String   | &check;      |
| azureStorageSid   | String   | &check;      |
| domainGuid        | String   | &check;      |
| domainName        | String   | &check;      |
| domainSid         | String   | &check;      |
| forestName        | String   | &check;      |
| netBiosDomainName | String   | &check;      |
| samAccountName    | String   | &check;      |

#### AzureFilesIdentityBasedAuthentication
| **Name**                  | **Type**                  | **Nullable** |
| ------------------------- | ------------------------- | ------------ |
| activeDirectoryProperties | ActiveDirectoryProperties | &check;      |
| defaultSharePermission    | String                    | &check;      |
| directoryServiceOptions   | String                    | &check;      |

#### BlobRestoreRange
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| endRange   | String   | &check;      |
| startRange | String   | &check;      |

#### BlobRestoreStatus
| **Name**      | **Type**               | **Nullable** |
| ------------- | ---------------------- | ------------ |
| blobRanges    | List<BlobRestoreRange> | &check;      |
| failureReason | String                 | &check;      |
| restoreId     | String                 | &check;      |
| status        | String                 | &check;      |
| timeToRestore | String                 | &check;      |

#### CustomDomain
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| name         | String   | &check;      |
| useSubDomain | Boolean  | &check;      |

#### Encryption
| **Name**                            | **Type**           | **Nullable** |
| ----------------------------------- | ------------------ | ------------ |
| encryptionFederatedIdentityClientId | String             | &check;      |
| encryptionUserAssignedIdentity      | String             | &check;      |
| keySource                           | String             | &check;      |
| keyVaultProperties                  | KeyVaultProperties | &check;      |
| requireInfrastructureEncryption     | Boolean            | &check;      |
| services                            | EncryptionServices | &check;      |

#### EncryptionService
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| enabled         | Boolean  | &check;      |
| keyType         | String   | &check;      |
| lastEnabledTime | String   | &check;      |

#### EncryptionServices
| **Name** | **Type**          | **Nullable** |
| -------- | ----------------- | ------------ |
| blob     | EncryptionService | &check;      |
| file     | EncryptionService | &check;      |
| queue    | EncryptionService | &check;      |
| table    | EncryptionService | &check;      |

#### Endpoints
| **Name**           | **Type**          | **Nullable** |
| ------------------ | ----------------- | ------------ |
| blob               | String            | &check;      |
| dfs                | String            | &check;      |
| file               | String            | &check;      |
| internetEndpoints  | InternetEndpoints | &check;      |
| microsoftEndpoints | InternetEndpoints | &check;      |
| queue              | String            | &check;      |
| table              | String            | &check;      |
| web                | String            | &check;      |

#### GeoReplicationStats
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| canFailover  | Boolean  | &check;      |
| lastSyncTime | String   | &check;      |
| status       | String   | &check;      |

#### Identity
| **Name**               | **Type**                         | **Nullable** |
| ---------------------- | -------------------------------- | ------------ |
| principalId            | String                           | &check;      |
| tenantId               | String                           | &check;      |
| type                   | String                           | &check;      |
| userAssignedIdentities | Map<String,UserAssignedIdentity> | &check;      |

#### ImmutableStorageAccount
| **Name**                              | **Type** | **Nullable** |
| ------------------------------------- | -------- | ------------ |
| allowProtectedAppendWrites            | Boolean  | &check;      |
| enabled                               | Boolean  | &check;      |
| immutabilityPeriodSinceCreationInDays | Int      | &check;      |
| state                                 | String   | &check;      |

#### InternetEndpoints
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| blob     | String   | &check;      |
| dfs      | String   | &check;      |
| file     | String   | &check;      |
| queue    | String   | &check;      |
| table    | String   | &check;      |
| web      | String   | &check;      |

#### IpRule
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| action           | String   | &check;      |
| ipAddressOrRange | String   | &check;      |

#### KeyVaultProperties
| **Name**                               | **Type** | **Nullable** |
| -------------------------------------- | -------- | ------------ |
| currentVersionKeyIdentifier            | String   | &check;      |
| currentVersionedKeyExpirationTimestamp | String   | &check;      |
| keyName                                | String   | &check;      |
| keyVaultUri                            | String   | &check;      |
| keyVersion                             | String   | &check;      |
| lastKeyRotationTimestamp               | String   | &check;      |

#### NetworkRuleSet
| **Name**            | **Type**                 | **Nullable** |
| ------------------- | ------------------------ | ------------ |
| bypass              | String                   | &check;      |
| defaultAction       | String                   | &check;      |
| ipRules             | List<IpRule>             | &check;      |
| resourceAccessRules | List<ResourceAccessRule> | &check;      |
| virtualNetworkRules | List<VirtualNetworkRule> | &check;      |

#### PrivateEndpointConnection
| **Name**                          | **Type**                          | **Nullable** |
| --------------------------------- | --------------------------------- | ------------ |
| id                                | String                            | &check;      |
| name                              | String                            | &check;      |
| privateEndpointId                 | String                            | &check;      |
| privateLinkServiceConnectionState | PrivateLinkServiceConnectionState | &check;      |
| provisioningState                 | String                            | &check;      |
| type                              | String                            | &check;      |

#### PrivateLinkResource
| **Name**             | **Type**     | **Nullable** |
| -------------------- | ------------ | ------------ |
| groupId              | String       | &check;      |
| requiredDnsZoneNames | List<String> | &check;      |
| requiredMembers      | List<String> | &check;      |

#### PrivateLinkServiceConnectionState
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| actionsRequired | String   | &check;      |
| description     | String   | &check;      |
| status          | String   | &check;      |

#### ResourceAccessRule
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| resourceId | String   | &check;      |
| tenantId   | String   | &check;      |

#### RoutingReference
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| publishInternetEndpoints  | Boolean  | &check;      |
| publishMicrosoftEndpoints | Boolean  | &check;      |
| routingChoice             | String   | &check;      |

#### SasPolicy
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| expirationAction    | String   | &check;      |
| sasExpirationPeriod | String   | &check;      |

#### UserAssignedIdentity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| clientId    | String   | &check;      |
| principalId | String   | &check;      |

#### VirtualNetworkRule
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| action     | String   | &check;      |
| resourceId | String   | &check;      |
| state      | String   | &check;      |
