---
description: Azure Sql Server
---
azure_sql_server
----------------

| **Name**                   | **Type**                            | **Nullable** |
| -------------------------- | ----------------------------------- | ------------ |
| administratorLogin         | String                              | &check;      |
| blobAuditingPolicies       | List<BlobAuditingPolicy>            | &check;      |
| encryptionProtectors       | List<EncryptionProtector>           | &check;      |
| firewallRules              | List<FirewallRule>                  | &check;      |
| fullyQualifiedDomainName   | String                              | &check;      |
| id                         | String                              | &cross;      |
| identity                   | Identity                            | &check;      |
| kind                       | String                              | &check;      |
| location                   | String                              | &cross;      |
| minimalTlsVersion          | String                              | &check;      |
| name                       | String                              | &cross;      |
| privateEndpointConnections | List<PrivateEndpointConnection>     | &check;      |
| publicNetworkAccess        | String                              | &check;      |
| resourceGroupName          | String                              | &cross;      |
| securityAlertPolicy        | SecurityAlertPolicy                 | &check;      |
| state                      | String                              | &check;      |
| subscriptionId             | String                              | &cross;      |
| tags                       | Map<String,String>                  | &check;      |
| type                       | String                              | &cross;      |
| version                    | String                              | &check;      |
| vulnerabilityAssessment    | List<ServerVulnerabilityAssessment> | &check;      |

#### BlobAuditingPolicy
| **Name**                     | **Type**     | **Nullable** |
| ---------------------------- | ------------ | ------------ |
| auditActionsAndGroups        | List<String> | &check;      |
| id                           | String       | &check;      |
| isAzureMonitorTargetEnabled  | Boolean      | &check;      |
| isStorageSecondaryKeyInUse   | Boolean      | &check;      |
| name                         | String       | &check;      |
| queueDelayMs                 | Int          | &check;      |
| retentionDays                | Int          | &check;      |
| state                        | String       | &check;      |
| storageAccountAccessKey      | String       | &check;      |
| storageAccountSubscriptionId | String       | &check;      |
| storageEndpoint              | String       | &check;      |
| type                         | String       | &check;      |

#### EncryptionProtector
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| kind          | String   | &check;      |
| parentId      | String   | &check;      |
| region        | String   | &check;      |
| serverKeyName | String   | &check;      |
| serverKeyType | String   | &check;      |
| sqlServerName | String   | &check;      |
| thumbprint    | String   | &check;      |
| uri           | String   | &check;      |

#### FirewallRule
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| endIpAddress   | String   | &check;      |
| kind           | String   | &check;      |
| parentId       | String   | &check;      |
| region         | String   | &check;      |
| sqlServerName  | String   | &check;      |
| startIpAddress | String   | &check;      |

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

#### SecurityAlertPolicy
| **Name**                | **Type**     | **Nullable** |
| ----------------------- | ------------ | ------------ |
| disabledAlerts          | List<String> | &check;      |
| emailAccountAdmins      | Boolean      | &check;      |
| emailAddresses          | List<String> | &cross;      |
| parentId                | String       | &check;      |
| retentionDays           | Int          | &check;      |
| sqlServerName           | String       | &check;      |
| state                   | String       | &check;      |
| storageAccountAccessKey | String       | &check;      |
| storageEndpoint         | String       | &check;      |

#### ServerVulnerabilityAssessment
| **Name**                | **Type**     | **Nullable** |
| ----------------------- | ------------ | ------------ |
| emailSubscriptionAdmins | Boolean      | &check;      |
| emails                  | List<String> | &check;      |
| id                      | String       | &check;      |
| name                    | String       | &check;      |
| recurringScans          | Boolean      | &check;      |
| storageContainerPath    | String       | &check;      |
| type                    | String       | &check;      |
