---
description: Azure Active Directory Service Principal
---
azure_ad_service_principal
--------------------------

| **Name**                               | **Type**                                | **Nullable** |
| -------------------------------------- | --------------------------------------- | ------------ |
| accountEnabled                         | Boolean                                 | &check;      |
| addIns                                 | List<AddIn>                             | &check;      |
| alternativeNames                       | List<String>                            | &check;      |
| appDescription                         | String                                  | &check;      |
| appDisplayName                         | String                                  | &check;      |
| appId                                  | String                                  | &check;      |
| appOwnerOrganizationId                 | String                                  | &check;      |
| appRoleAssignedTo                      | List<AppRoleAssignment>                 | &check;      |
| appRoleAssignmentRequired              | Boolean                                 | &check;      |
| appRoleAssignments                     | List<AppRoleAssignment>                 | &check;      |
| appRoles                               | List<AppRole>                           | &check;      |
| applicationTemplateId                  | String                                  | &check;      |
| claimsMappingPolicies                  | List<Policy>                            | &check;      |
| createdObjects                         | List<DirectoryObject>                   | &check;      |
| delegatedPermissionClassifications     | List<DelegatedPermissionClassification> | &check;      |
| deletedDateTime                        | String                                  | &check;      |
| description                            | String                                  | &check;      |
| disabledByMicrosoftStatus              | String                                  | &check;      |
| displayName                            | String                                  | &check;      |
| endpoints                              | List<Endpoint>                          | &check;      |
| federatedIdentityCredentials           | List<FederatedIdentityCredential>       | &check;      |
| homeRealmDiscoveryPolicies             | List<Policy>                            | &check;      |
| homepage                               | String                                  | &check;      |
| id                                     | String                                  | &cross;      |
| info                                   | JSON                                    | &check;      |
| keyCredentials                         | List<KeyCredential>                     | &check;      |
| loginUrl                               | String                                  | &check;      |
| logoutUrl                              | String                                  | &check;      |
| memberOf                               | List<DirectoryObject>                   | &check;      |
| notes                                  | String                                  | &check;      |
| oDataType                              | String                                  | &check;      |
| oauth2Permissions                      | List<PermissionScope>                   | &check;      |
| ownedObjects                           | List<DirectoryObject>                   | &check;      |
| owners                                 | List<DirectoryObject>                   | &check;      |
| passwordCredentials                    | List<PasswordCredential>                | &check;      |
| preferredSingleSignOnMode              | String                                  | &check;      |
| preferredTokenSigningKeyThumbprint     | String                                  | &check;      |
| replyUrls                              | List<String>                            | &check;      |
| resourceSpecificApplicationPermissions | List<ResourceSpecificPermission>        | &check;      |
| samlSingleSignOnSettings               | SamlSingleSignOnSettings                | &check;      |
| servicePrincipalNames                  | List<String>                            | &check;      |
| servicePrincipalType                   | String                                  | &check;      |
| signInAudience                         | String                                  | &check;      |
| tags                                   | List<String>                            | &check;      |
| tokenEncryptionKeyId                   | String                                  | &check;      |
| tokenIssuancePolicies                  | List<Policy>                            | &check;      |
| tokenLifetimePolicies                  | List<Policy>                            | &check;      |
| transitiveMemberOf                     | List<DirectoryObject>                   | &check;      |

#### AddIn
| **Name**   | **Type**           | **Nullable** |
| ---------- | ------------------ | ------------ |
| id         | String             | &check;      |
| oDataType  | String             | &check;      |
| properties | Map<String,String> | &check;      |

#### AppRole
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| allowedMemberTypes | List<String> | &check;      |
| description        | String       | &check;      |
| displayName        | String       | &check;      |
| id                 | String       | &check;      |
| isEnabled          | Boolean      | &check;      |
| oDataType          | String       | &check;      |
| origin             | String       | &check;      |
| value              | String       | &check;      |

#### AppRoleAssignment
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| appRoleId            | String   | &check;      |
| createdDateTime      | String   | &check;      |
| principalDisplayName | String   | &check;      |
| principalId          | String   | &check;      |
| principalType        | String   | &check;      |
| resourceDisplayName  | String   | &check;      |
| resourceId           | String   | &check;      |

#### DelegatedPermissionClassification
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| classification | String   | &check;      |
| id             | String   | &check;      |
| oDataType      | String   | &check;      |
| permissionId   | String   | &check;      |
| permissionName | String   | &check;      |

#### DirectoryObject
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| oDataType | String   | &check;      |

#### Endpoint
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| capability         | String   | &check;      |
| deletedDateTime    | String   | &check;      |
| id                 | String   | &check;      |
| oDataType          | String   | &check;      |
| providerId         | String   | &check;      |
| providerName       | String   | &check;      |
| providerResourceId | String   | &check;      |
| uri                | String   | &check;      |

#### FederatedIdentityCredential
| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| audiences   | List<String> | &check;      |
| description | String       | &check;      |
| id          | String       | &cross;      |
| issuer      | String       | &check;      |
| name        | String       | &check;      |
| oDataType   | String       | &check;      |
| subject     | String       | &check;      |

#### KeyCredential
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| displayName   | String   | &check;      |
| endDateTime   | String   | &check;      |
| keyId         | String   | &check;      |
| oDataType     | String   | &check;      |
| startDateTime | String   | &check;      |
| type          | String   | &check;      |

#### PasswordCredential
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| displayName   | String   | &check;      |
| endDateTime   | String   | &check;      |
| hint          | String   | &check;      |
| keyId         | String   | &check;      |
| oDataType     | String   | &check;      |
| secretText    | String   | &check;      |
| startDateTime | String   | &check;      |

#### PermissionScope
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| adminConsentDescription | String   | &check;      |
| adminConsentDisplayName | String   | &check;      |
| id                      | String   | &check;      |
| isEnabled               | Boolean  | &check;      |
| oDataType               | String   | &check;      |
| origin                  | String   | &check;      |
| type                    | String   | &check;      |
| userConsentDescription  | String   | &check;      |
| userConsentDisplayName  | String   | &check;      |
| value                   | String   | &check;      |

#### Policy
| **Name**              | **Type**     | **Nullable** |
| --------------------- | ------------ | ------------ |
| definition            | List<String> | &check;      |
| deletedDateTime       | String       | &check;      |
| description           | String       | &check;      |
| displayName           | String       | &check;      |
| id                    | String       | &check;      |
| isEnabled             | Boolean      | &check;      |
| isOrganizationDefault | Boolean      | &check;      |
| oDataType             | String       | &check;      |

#### ResourceSpecificPermission
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| displayName | String   | &check;      |
| id          | String   | &check;      |
| isEnabled   | Boolean  | &check;      |
| oDataType   | String   | &check;      |
| value       | String   | &check;      |

#### SamlSingleSignOnSettings
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| oDataType  | String   | &check;      |
| relayState | String   | &check;      |
