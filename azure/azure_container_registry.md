---
description: Azure Container Registry
---
azure_container_registry
------------------------

| **Name**                   | **Type**                        | **Nullable** |
| -------------------------- | ------------------------------- | ------------ |
| adminUserEnabled           | Boolean                         | &check;      |
| creationDate               | String                          | &check;      |
| dataEndpointEnabled        | Boolean                         | &check;      |
| dataEndpointHostNames      | List<String>                    | &check;      |
| encryption                 | EncryptionProperty              | &check;      |
| id                         | String                          | &cross;      |
| identity                   | Identity                        | &check;      |
| location                   | String                          | &cross;      |
| loginServer                | String                          | &check;      |
| name                       | String                          | &cross;      |
| networkRuleBypassOptions   | String                          | &check;      |
| networkRuleSet             | NetworkRuleSet                  | &check;      |
| policies                   | Policies                        | &check;      |
| privateEndpointConnections | List<PrivateEndpointConnection> | &check;      |
| provisioningState          | String                          | &check;      |
| publicNetworkAccess        | String                          | &check;      |
| resourceGroupName          | String                          | &cross;      |
| sku                        | Sku                             | &check;      |
| status                     | Status                          | &check;      |
| subscriptionId             | String                          | &cross;      |
| systemData                 | SystemData                      | &check;      |
| tags                       | Map<String,String>              | &check;      |
| type                       | String                          | &cross;      |
| zoneRedundancy             | String                          | &check;      |

#### EncryptionProperty
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| keyVaultProperties | KeyVaultProperties | &check;      |
| status             | String             | &check;      |

#### Identity
| **Name**               | **Type**                         | **Nullable** |
| ---------------------- | -------------------------------- | ------------ |
| principalId            | String                           | &check;      |
| tenantId               | String                           | &check;      |
| type                   | String                           | &check;      |
| userAssignedIdentities | Map<String,UserAssignedIdentity> | &check;      |

#### IpRule
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| action           | String   | &check;      |
| ipAddressOrRange | String   | &check;      |

#### KeyVaultProperties
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| identity                 | String   | &check;      |
| keyIdentifier            | String   | &check;      |
| keyRotationEnabled       | Boolean  | &check;      |
| lastKeyRotationTimestamp | String   | &check;      |
| versionedKeyIdentifier   | String   | &check;      |

#### NetworkRuleSet
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| defaultAction | String       | &check;      |
| ipRules       | List<IpRule> | &check;      |

#### Policies
| **Name**                       | **Type** | **Nullable** |
| ------------------------------ | -------- | ------------ |
| exportPolicyStatus             | String   | &check;      |
| quarantinePolicyStatus         | String   | &check;      |
| retentionPolicyDays            | Int      | &check;      |
| retentionPolicyLastUpdatedTime | String   | &check;      |
| retentionPolicyStatus          | String   | &check;      |
| trustPolicyStatus              | String   | &check;      |
| trustPolicyType                | String   | &check;      |

#### PrivateEndpointConnection
| **Name**                          | **Type**                          | **Nullable** |
| --------------------------------- | --------------------------------- | ------------ |
| privateEndpointId                 | String                            | &check;      |
| privateLinkServiceConnectionState | PrivateLinkServiceConnectionState | &check;      |
| provisioningState                 | String                            | &check;      |
| systemData                        | SystemData                        | &check;      |

#### PrivateLinkServiceConnectionState
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| actionsRequired | String   | &check;      |
| description     | String   | &check;      |
| status          | String   | &check;      |

#### Sku
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| tier     | String   | &check;      |

#### Status
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| displayStatus | String   | &check;      |
| message       | String   | &check;      |
| timestamp     | String   | &check;      |

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
