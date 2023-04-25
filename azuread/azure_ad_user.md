---
description: Azure Active Directory User
---
azure_ad_user
-------------

| **Name**                        | **Type**                          | **Nullable** |
| ------------------------------- | --------------------------------- | ------------ |
| accountEnabled                  | Boolean                           | &check;      |
| ageGroup                        | String                            | &check;      |
| appRoleAssignments              | List<AppRoleAssignment>           | &check;      |
| assignedLicenses                | List<AssignedLicense>             | &check;      |
| assignedPlans                   | List<AssignedPlan>                | &check;      |
| city                            | String                            | &check;      |
| companyName                     | String                            | &check;      |
| consentProvidedForMinor         | String                            | &check;      |
| contacts                        | List<DirectoryObject>             | &check;      |
| country                         | String                            | &check;      |
| createdDateTime                 | String                            | &check;      |
| creationType                    | String                            | &check;      |
| deletedDateTime                 | String                            | &check;      |
| department                      | String                            | &check;      |
| displayName                     | String                            | &check;      |
| employeeHireDate                | String                            | &check;      |
| employeeId                      | String                            | &check;      |
| employeeOrgData                 | EmployeeOrgData                   | &check;      |
| employeeType                    | String                            | &check;      |
| externalUserState               | String                            | &check;      |
| externalUserStateChangeDateTime | String                            | &check;      |
| faxNumber                       | String                            | &check;      |
| givenName                       | String                            | &check;      |
| id                              | String                            | &cross;      |
| identities                      | List<ObjectIdentity>              | &check;      |
| imAddresses                     | List<String>                      | &check;      |
| isResourceAccount               | Boolean                           | &check;      |
| jobTitle                        | String                            | &check;      |
| lastPasswordChangeDateTime      | String                            | &check;      |
| legalAgeGroupClassification     | String                            | &check;      |
| licenseProcessingStates         | List<LicenseAssignmentState>      | &check;      |
| mail                            | String                            | &check;      |
| mailNickname                    | String                            | &check;      |
| manager                         | DirectoryObject                   | &check;      |
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
| passwordPolicies                | String                            | &check;      |
| passwordProfile                 | PasswordProfile                   | &check;      |
| postalCode                      | String                            | &check;      |
| preferredDataLocation           | String                            | &check;      |
| preferredLanguage               | String                            | &check;      |
| provisionedPlans                | List<ProvisionedPlan>             | &check;      |
| proxyAddresses                  | List<String>                      | &check;      |
| registeredDevices               | List<DirectoryObject>             | &check;      |
| scopedRoleMemberships           | List<ScopedRoleMembership>        | &check;      |
| showInAddressList               | Boolean                           | &check;      |
| signInSessionsValidFromDateTime | String                            | &check;      |
| state                           | String                            | &check;      |
| streetAddress                   | String                            | &check;      |
| surname                         | String                            | &check;      |
| usageLocation                   | String                            | &check;      |
| userPrincipalName               | String                            | &check;      |
| userType                        | String                            | &check;      |

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

#### DeviceActionResult
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| actionName          | String   | &check;      |
| actionState         | String   | &check;      |
| lastUpdatedDateTime | String   | &check;      |
| oDataType           | String   | &check;      |
| startDateTime       | String   | &check;      |

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
| oDataType   | String   | &check;      |

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
| oDataType     | String                | &check;      |
| servicePlans  | List<ServicePlanInfo> | &check;      |
| skuId         | String                | &check;      |
| skuPartNumber | String                | &check;      |

#### ManagedAppRegistration
| **Name**             | **Type**     | **Nullable** |
| -------------------- | ------------ | ------------ |
| androidPackageId     | String       | &check;      |
| applicationVersion   | String       | &check;      |
| deviceName           | String       | &check;      |
| deviceTag            | String       | &check;      |
| deviceType           | String       | &check;      |
| flaggedReasons       | List<String> | &check;      |
| iosBundleId          | String       | &check;      |
| managementSdkVersion | String       | &check;      |
| platformVersion      | String       | &check;      |
| userId               | String       | &check;      |
| version              | String       | &check;      |

#### ManagedDevice
| **Name**                                | **Type**                 | **Nullable** |
| --------------------------------------- | ------------------------ | ------------ |
| activationLockBypassCode                | String                   | &check;      |
| androidSecurityPatchLevel               | String                   | &check;      |
| azureADDeviceId                         | String                   | &check;      |
| complianceGracePeriodExpirationDateTime | String                   | &check;      |
| complianceState                         | String                   | &check;      |
| deviceActionResults                     | List<DeviceActionResult> | &check;      |
| deviceCategory                          | String                   | &check;      |
| deviceCategoryDisplayName               | String                   | &check;      |
| deviceEnrollmentType                    | String                   | &check;      |
| deviceName                              | String                   | &check;      |
| deviceRegistrationState                 | String                   | &check;      |
| easActivated                            | Boolean                  | &check;      |
| easActivationDateTime                   | String                   | &check;      |
| easDeviceId                             | String                   | &check;      |
| emailAddress                            | String                   | &check;      |
| exchangeAccessState                     | String                   | &check;      |
| exchangeAccessStateReason               | String                   | &check;      |
| iccid                                   | String                   | &check;      |
| id                                      | String                   | &check;      |
| imei                                    | String                   | &check;      |
| isEncrypted                             | Boolean                  | &check;      |
| isSupervised                            | Boolean                  | &check;      |
| jailBroken                              | String                   | &check;      |
| lastSyncDateTime                        | String                   | &check;      |
| managedDeviceName                       | String                   | &check;      |
| managedDeviceOwnerType                  | String                   | &check;      |
| managementAgent                         | String                   | &check;      |
| manufacturer                            | String                   | &check;      |
| meid                                    | String                   | &check;      |
| model                                   | String                   | &check;      |
| notes                                   | String                   | &check;      |
| oDataType                               | String                   | &check;      |
| operatingSystem                         | String                   | &check;      |
| osVersion                               | String                   | &check;      |
| partnerReportedThreatState              | String                   | &check;      |
| phoneNumber                             | String                   | &check;      |
| serialNumber                            | String                   | &check;      |
| subscriberCarrier                       | String                   | &check;      |
| udid                                    | String                   | &check;      |
| userDisplayName                         | String                   | &check;      |
| userId                                  | String                   | &check;      |
| userPrincipalName                       | String                   | &check;      |
| wiFiMacAddress                          | String                   | &check;      |

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
