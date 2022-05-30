---
description: Azure Policy Assignment
---
azure_policy_assignment
-----------------------

| **Name**              | **Type**                   | **Nullable** |
| --------------------- | -------------------------- | ------------ |
| description           | String                     | &check;      |
| displayName           | String                     | &cross;      |
| enforcementMode       | String                     | &check;      |
| excludedScopes        | List<String>               | &check;      |
| id                    | String                     | &cross;      |
| identity              | Identity                   | &check;      |
| location              | String                     | &check;      |
| metadata              | String                     | &check;      |
| name                  | String                     | &cross;      |
| nonComplianceMessages | List<NonComplianceMessage> | &check;      |
| parameters            | Map<String,JSON>           | &check;      |
| policyDefinitionId    | String                     | &check;      |
| resourceGroupName     | String                     | &cross;      |
| scope                 | String                     | &check;      |
| subscriptionId        | String                     | &cross;      |
| systemData            | SystemData                 | &check;      |
| type                  | String                     | &cross;      |

#### Identity
| **Name**               | **Type**                                        | **Nullable** |
| ---------------------- | ----------------------------------------------- | ------------ |
| principalId            | String                                          | &check;      |
| tenantId               | String                                          | &check;      |
| type                   | String                                          | &check;      |
| userAssignedIdentities | Map<String,IdentityUserAssignedIdentitiesValue> | &check;      |

#### IdentityUserAssignedIdentitiesValue
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| clientId    | String   | &check;      |
| principalId | String   | &check;      |

#### NonComplianceMessage
| **Name**                    | **Type** | **Nullable** |
| --------------------------- | -------- | ------------ |
| message                     | String   | &check;      |
| policyDefinitionReferenceId | String   | &check;      |

#### SystemData
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| createdAt          | String   | &check;      |
| createdBy          | String   | &check;      |
| createdByType      | String   | &check;      |
| lastModifiedAt     | String   | &check;      |
| lastModifiedBy     | String   | &check;      |
| lastModifiedByType | String   | &check;      |
