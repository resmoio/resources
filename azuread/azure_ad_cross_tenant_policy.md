---
description: Azure Active Directory Cross Tenant Policy
---
azure_ad_cross_tenant_policy
----------------------------

| **Name**              | **Type**                                          | **Nullable** |
| --------------------- | ------------------------------------------------- | ------------ |
| allowedCloudEndpoints | List<String>                                      | &check;      |
| description           | String                                            | &check;      |
| displayName           | String                                            | &check;      |
| id                    | String                                            | &cross;      |
| msgraphDefault        | CrossTenantAccessPolicyConfigurationDefault       | &check;      |
| oDataType             | String                                            | &check;      |
| partners              | List<CrossTenantAccessPolicyConfigurationPartner> | &check;      |

#### CrossTenantAccessPolicyB2BSetting
| **Name**       | **Type**                                   | **Nullable** |
| -------------- | ------------------------------------------ | ------------ |
| applications   | CrossTenantAccessPolicyTargetConfiguration | &check;      |
| oDataType      | String                                     | &check;      |
| usersAndGroups | CrossTenantAccessPolicyTargetConfiguration | &check;      |

#### CrossTenantAccessPolicyConfigurationDefault
| **Name**                     | **Type**                            | **Nullable** |
| ---------------------------- | ----------------------------------- | ------------ |
| automaticUserConsentSettings | InboundOutboundPolicyConfiguration  | &check;      |
| b2bCollaborationInbound      | CrossTenantAccessPolicyB2BSetting   | &check;      |
| b2bCollaborationOutbound     | CrossTenantAccessPolicyB2BSetting   | &check;      |
| b2bDirectConnectInbound      | CrossTenantAccessPolicyB2BSetting   | &check;      |
| b2bDirectConnectOutbound     | CrossTenantAccessPolicyB2BSetting   | &check;      |
| inboundTrust                 | CrossTenantAccessPolicyInboundTrust | &check;      |
| isServiceDefault             | Boolean                             | &check;      |

#### CrossTenantAccessPolicyConfigurationPartner
| **Name**                     | **Type**                             | **Nullable** |
| ---------------------------- | ------------------------------------ | ------------ |
| automaticUserConsentSettings | InboundOutboundPolicyConfiguration   | &check;      |
| b2bCollaborationInbound      | CrossTenantAccessPolicyB2BSetting    | &check;      |
| b2bCollaborationOutbound     | CrossTenantAccessPolicyB2BSetting    | &check;      |
| b2bDirectConnectInbound      | CrossTenantAccessPolicyB2BSetting    | &check;      |
| b2bDirectConnectOutbound     | CrossTenantAccessPolicyB2BSetting    | &check;      |
| identitySynchronization      | CrossTenantIdentitySyncPolicyPartner | &check;      |
| inboundTrust                 | CrossTenantAccessPolicyInboundTrust  | &check;      |
| isServiceProvider            | Boolean                              | &check;      |
| oDataType                    | String                               | &check;      |
| tenantId                     | String                               | &check;      |

#### CrossTenantAccessPolicyInboundTrust
| **Name**                            | **Type** | **Nullable** |
| ----------------------------------- | -------- | ------------ |
| isCompliantDeviceAccepted           | Boolean  | &check;      |
| isHybridAzureADJoinedDeviceAccepted | Boolean  | &check;      |
| isMfaAccepted                       | Boolean  | &check;      |
| oDataType                           | String   | &check;      |

#### CrossTenantAccessPolicyTarget
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| oDataType  | String   | &check;      |
| target     | String   | &check;      |
| targetType | String   | &check;      |

#### CrossTenantAccessPolicyTargetConfiguration
| **Name**   | **Type**                            | **Nullable** |
| ---------- | ----------------------------------- | ------------ |
| accessType | String                              | &check;      |
| oDataType  | String                              | &check;      |
| targets    | List<CrossTenantAccessPolicyTarget> | &check;      |

#### CrossTenantIdentitySyncPolicyPartner
| **Name**        | **Type**                   | **Nullable** |
| --------------- | -------------------------- | ------------ |
| displayName     | String                     | &check;      |
| oDataType       | String                     | &check;      |
| tenantId        | String                     | &check;      |
| userSyncInbound | CrossTenantUserSyncInbound | &check;      |

#### CrossTenantUserSyncInbound
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| isSyncAllowed | Boolean  | &check;      |
| oDataType     | String   | &check;      |

#### InboundOutboundPolicyConfiguration
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| inboundAllowed  | Boolean  | &check;      |
| oDataType       | String   | &check;      |
| outboundAllowed | Boolean  | &check;      |
