---
description: Azure Key Vault
---
azure_key_vault
---------------

| **Name**                     | **Type**                        | **Nullable** |
| ---------------------------- | ------------------------------- | ------------ |
| accessPolicies               | List<AccessPolicyEntry>         | &check;      |
| createMode                   | String                          | &check;      |
| diagnosticSettings           | List<DiagnosticSetting>         | &check;      |
| enabledForDeployment         | Boolean                         | &check;      |
| enabledForDiskEncryption     | Boolean                         | &check;      |
| enabledForTemplateDeployment | Boolean                         | &check;      |
| hsmPoolResourceId            | String                          | &check;      |
| id                           | String                          | &cross;      |
| keys                         | List<Key>                       | &check;      |
| location                     | String                          | &cross;      |
| name                         | String                          | &cross;      |
| networkAcls                  | NetworkRuleSet                  | &check;      |
| privateEndpointConnections   | List<PrivateEndpointConnection> | &check;      |
| privateLinkResources         | List<PrivateLinkResource>       | &check;      |
| provisioningState            | String                          | &check;      |
| purgeProtectionEnabled       | Boolean                         | &check;      |
| rbacAuthorizationEnabled     | Boolean                         | &check;      |
| resourceGroupName            | String                          | &cross;      |
| secrets                      | List<Secret>                    | &check;      |
| sku                          | Sku                             | &check;      |
| softDeleteEnabled            | Boolean                         | &check;      |
| softDeleteRetentionInDays    | Int                             | &check;      |
| subscriptionId               | String                          | &cross;      |
| tags                         | Map<String,String>              | &cross;      |
| tenantId                     | String                          | &check;      |
| type                         | String                          | &cross;      |
| vaultUri                     | String                          | &check;      |

#### AccessPolicyEntry
| **Name**      | **Type**    | **Nullable** |
| ------------- | ----------- | ------------ |
| applicationId | String      | &check;      |
| objectId      | String      | &check;      |
| permissions   | Permissions | &check;      |
| tenantId      | String      | &check;      |

#### DiagnosticSetting
| **Name**                    | **Type**             | **Nullable** |
| --------------------------- | -------------------- | ------------ |
| eventHubAuthorizationRuleId | String               | &check;      |
| eventHubName                | String               | &check;      |
| logs                        | List<LogSettings>    | &check;      |
| metrics                     | List<MetricSettings> | &check;      |
| resourceId                  | String               | &check;      |
| storageAccountId            | String               | &check;      |
| workspaceId                 | String               | &check;      |

#### JsonWebKey
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| keyId    | String       | &cross;      |
| keyOps   | List<String> | &check;      |
| keyType  | String       | &check;      |
| valid    | Boolean      | &check;      |

#### Key
| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| createdOn       | String             | &check;      |
| enabled         | Boolean            | &check;      |
| expiresOn       | String             | &check;      |
| id              | String             | &cross;      |
| key             | JsonWebKey         | &check;      |
| managed         | Boolean            | &check;      |
| name            | String             | &cross;      |
| notBefore       | String             | &check;      |
| recoverableDays | Int                | &check;      |
| recoveryLevel   | String             | &check;      |
| tags            | Map<String,String> | &check;      |
| updatedOn       | String             | &check;      |
| version         | String             | &check;      |

#### LogSettings
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| category               | String   | &check;      |
| enabled                | Boolean  | &check;      |
| retentionDays          | Int      | &check;      |
| retentionPolicyEnabled | Boolean  | &check;      |

#### MetricSettings
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| category               | String   | &check;      |
| enabled                | Boolean  | &check;      |
| retentionDays          | Int      | &check;      |
| retentionPolicyEnabled | Boolean  | &check;      |
| timeGrain              | String   | &check;      |

#### NetworkRuleSet
| **Name**            | **Type**                 | **Nullable** |
| ------------------- | ------------------------ | ------------ |
| bypass              | String                   | &check;      |
| defaultAction       | String                   | &check;      |
| ipRules             | List<String>             | &check;      |
| virtualNetworkRules | List<VirtualNetworkRule> | &check;      |

#### Permissions
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| certificates | List<String> | &check;      |
| keys         | List<String> | &check;      |
| secrets      | List<String> | &check;      |
| storage      | List<String> | &check;      |

#### PrivateEndpointConnection
| **Name**                          | **Type**                          | **Nullable** |
| --------------------------------- | --------------------------------- | ------------ |
| etag                              | String                            | &check;      |
| id                                | String                            | &check;      |
| privateEndpointId                 | String                            | &check;      |
| privateLinkServiceConnectionState | PrivateLinkServiceConnectionState | &check;      |
| provisioningState                 | String                            | &check;      |

#### PrivateLinkResource
| **Name**             | **Type**     | **Nullable** |
| -------------------- | ------------ | ------------ |
| groupId              | String       | &check;      |
| requiredDnsZoneNames | List<String> | &check;      |
| requiredMemberNames  | List<String> | &check;      |

#### PrivateLinkServiceConnectionState
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| actionsRequired | String   | &check;      |
| description     | String   | &check;      |
| status          | String   | &check;      |

#### Secret
| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| contentType     | String             | &check;      |
| createdOn       | String             | &check;      |
| enabled         | Boolean            | &check;      |
| expiresOn       | String             | &check;      |
| id              | String             | &cross;      |
| keyId           | String             | &check;      |
| managed         | Boolean            | &check;      |
| name            | String             | &cross;      |
| notBefore       | String             | &check;      |
| recoverableDays | Int                | &check;      |
| recoveryLevel   | String             | &check;      |
| tags            | Map<String,String> | &check;      |
| updatedOn       | String             | &check;      |
| version         | String             | &check;      |

#### Sku
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| family   | String   | &check;      |
| name     | String   | &check;      |

#### VirtualNetworkRule
| **Name**                         | **Type** | **Nullable** |
| -------------------------------- | -------- | ------------ |
| id                               | String   | &check;      |
| ignoreMissingVnetServiceEndpoint | Boolean  | &check;      |
