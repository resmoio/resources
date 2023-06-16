---
description: Azure Active Directory User
---
azure_ad_user
-------------

| **Name**                        | **Type**                          | **Nullable** |
| ------------------------------- | --------------------------------- | ------------ |
| accountEnabled                  | Boolean                           | &check;      |
| ageGroup                        | String                            | &check;      |
| agreementAcceptances            | List<AgreementAcceptance>         | &check;      |
| appRoleAssignments              | List<AppRoleAssignment>           | &check;      |
| assignedLicenses                | List<AssignedLicense>             | &check;      |
| assignedPlans                   | List<AssignedPlan>                | &check;      |
| authorizationInfo               | AuthorizationInfo                 | &check;      |
| businessPhones                  | List<String>                      | &check;      |
| city                            | String                            | &check;      |
| companyName                     | String                            | &check;      |
| consentProvidedForMinor         | String                            | &check;      |
| contacts                        | List<DirectoryObject>             | &check;      |
| country                         | String                            | &check;      |
| createdDateTime                 | String                            | &check;      |
| createdObjects                  | List<DirectoryObject>             | &check;      |
| creationType                    | String                            | &check;      |
| deletedDateTime                 | String                            | &check;      |
| department                      | String                            | &check;      |
| directReports                   | List<DirectoryObject>             | &check;      |
| displayName                     | String                            | &check;      |
| employeeHireDate                | String                            | &check;      |
| employeeId                      | String                            | &check;      |
| employeeOrgData                 | EmployeeOrgData                   | &check;      |
| employeeType                    | String                            | &check;      |
| externalUserState               | String                            | &check;      |
| externalUserStateChangeDateTime | String                            | &check;      |
| faxNumber                       | String                            | &check;      |
| followedSites                   | List<DirectoryObject>             | &check;      |
| givenName                       | String                            | &check;      |
| id                              | String                            | &cross;      |
| identities                      | List<ObjectIdentity>              | &check;      |
| imAddresses                     | List<String>                      | &check;      |
| isResourceAccount               | Boolean                           | &check;      |
| jobTitle                        | String                            | &check;      |
| lastPasswordChangeDateTime      | String                            | &check;      |
| legalAgeGroupClassification     | String                            | &check;      |
| licenseDetails                  | List<LicenseDetails>              | &check;      |
| licenseProcessingStates         | List<LicenseAssignmentState>      | &check;      |
| mail                            | String                            | &check;      |
| mailNickname                    | String                            | &check;      |
| manager                         | List<DirectoryObject>             | &check;      |
| memberOf                        | List<DirectoryObject>             | &check;      |
| mobilePhone                     | String                            | &check;      |
| oDataType                       | String                            | &check;      |
| officeLocation                  | String                            | &check;      |
| onPremisesDistinguishedName     | String                            | &check;      |
| onPremisesDomainName            | String                            | &check;      |
| onPremisesExtensionAttributes   | OnPremisesExtensionAttributes     | &check;      |
| onPremisesImmutableId           | String                            | &check;      |
| onPremisesLastSyncDateTime      | String                            | &check;      |
| onPremisesProvisioningErrors    | List<OnPremisesProvisioningError> | &check;      |
| onPremisesSamAccountName        | String                            | &check;      |
| onPremisesSecurityIdentifier    | String                            | &check;      |
| onPremisesSyncEnabled           | Boolean                           | &check;      |
| onPremisesUserPrincipalName     | String                            | &check;      |
| otherMails                      | List<String>                      | &check;      |
| ownedObjects                    | List<DirectoryObject>             | &check;      |
| passwordPolicies                | String                            | &check;      |
| passwordProfile                 | PasswordProfile                   | &check;      |
| postalCode                      | String                            | &check;      |
| preferredDataLocation           | String                            | &check;      |
| preferredLanguage               | String                            | &check;      |
| provisionedPlans                | List<ProvisionedPlan>             | &check;      |
| proxyAddresses                  | List<String>                      | &check;      |
| scopedRoleMemberOf              | List<ScopedRoleMembership>        | &check;      |
| securityIdentifier              | String                            | &check;      |
| showInAddressList               | Boolean                           | &check;      |
| signInActivity                  | SignInActivity                    | &check;      |
| signInSessionsValidFromDateTime | String                            | &check;      |
| state                           | String                            | &check;      |
| streetAddress                   | String                            | &check;      |
| surname                         | String                            | &check;      |
| transitiveMemberOf              | List<DirectoryObject>             | &check;      |
| usageLocation                   | String                            | &check;      |
| userPrincipalName               | String                            | &check;      |
| userType                        | String                            | &check;      |

#### AgreementAcceptance
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| agreementFileId    | String   | &check;      |
| agreementId        | String   | &check;      |
| deviceDisplayName  | String   | &check;      |
| deviceId           | String   | &check;      |
| deviceOSType       | String   | &check;      |
| deviceOSVersion    | String   | &check;      |
| expirationDateTime | String   | &check;      |
| id                 | String   | &check;      |
| oDataType          | String   | &check;      |
| recordedDateTime   | String   | &check;      |
| state              | String   | &check;      |
| userDisplayName    | String   | &check;      |
| userEmail          | String   | &check;      |
| userId             | String   | &check;      |
| userPrincipalName  | String   | &check;      |

#### AppRoleAssignment
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| appRoleId            | String   | &check;      |
| createdDateTime      | String   | &check;      |
| id                   | String   | &check;      |
| oDataType            | String   | &check;      |
| principalDisplayName | String   | &check;      |
| principalId          | String   | &check;      |
| principalType        | String   | &check;      |
| resourceDisplayName  | String   | &check;      |
| resourceId           | String   | &check;      |

#### AssignedLicense
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| disabledPlans | List<String> | &check;      |
| oDataType     | String       | &check;      |
| skuId         | String       | &check;      |

#### AssignedPlan
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| assignedDateTime | String   | &check;      |
| capabilityStatus | String   | &check;      |
| oDataType        | String   | &check;      |
| service          | String   | &check;      |
| servicePlanId    | String   | &check;      |

#### AuthorizationInfo
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| certificateUserIds | List<String> | &check;      |

#### DirectoryObject
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| oDataType | String   | &check;      |

#### EmployeeOrgData
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| costCenter | String   | &check;      |
| division   | String   | &check;      |
| oDataType  | String   | &check;      |

#### Identity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| id          | String   | &check;      |

#### LicenseAssignmentState
| **Name**            | **Type**     | **Nullable** |
| ------------------- | ------------ | ------------ |
| assignedByGroup     | String       | &check;      |
| disabledPlans       | List<String> | &check;      |
| error               | String       | &check;      |
| lastUpdatedDateTime | String       | &check;      |
| oDataType           | String       | &check;      |
| skuId               | String       | &check;      |
| state               | String       | &check;      |

#### LicenseDetails
| **Name**      | **Type**              | **Nullable** |
| ------------- | --------------------- | ------------ |
| id            | String                | &check;      |
| oDataType     | String                | &check;      |
| servicePlans  | List<ServicePlanInfo> | &check;      |
| skuId         | String                | &check;      |
| skuPartNumber | String                | &check;      |

#### ObjectIdentity
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| issuer           | String   | &check;      |
| issuerAssignedId | String   | &check;      |
| oDataType        | String   | &check;      |
| signInType       | String   | &check;      |

#### OnPremisesExtensionAttributes
| **Name**            | **Type**           | **Nullable** |
| ------------------- | ------------------ | ------------ |
| extensionAttributes | Map<String,String> | &check;      |
| oDataType           | String             | &check;      |

#### OnPremisesProvisioningError
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| category             | String   | &check;      |
| oDataType            | String   | &check;      |
| occurredDateTime     | String   | &check;      |
| propertyCausingError | String   | &check;      |
| value                | String   | &check;      |

#### PasswordProfile
| **Name**                             | **Type** | **Nullable** |
| ------------------------------------ | -------- | ------------ |
| forceChangePasswordNextSignIn        | Boolean  | &check;      |
| forceChangePasswordNextSignInWithMfa | Boolean  | &check;      |
| oDataType                            | String   | &check;      |
| password                             | String   | &check;      |

#### ProvisionedPlan
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| capabilityStatus   | String   | &check;      |
| oDataType          | String   | &check;      |
| provisioningStatus | String   | &check;      |
| service            | String   | &check;      |

#### ScopedRoleMembership
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| administrativeUnitId | String   | &check;      |
| id                   | String   | &check;      |
| oDataType            | String   | &check;      |
| roleId               | String   | &check;      |
| roleMemberInfo       | Identity | &check;      |

#### ServicePlanInfo
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| appliesTo          | String   | &check;      |
| oDataType          | String   | &check;      |
| provisioningStatus | String   | &check;      |
| servicePlanId      | String   | &check;      |
| servicePlanName    | String   | &check;      |

#### SignInActivity
| **Name**                          | **Type** | **Nullable** |
| --------------------------------- | -------- | ------------ |
| lastNonInteractiveSignInDateTime  | String   | &check;      |
| lastNonInteractiveSignInRequestId | String   | &check;      |
| lastSignInDateTime                | String   | &check;      |
| lastSignInRequestId               | String   | &check;      |
