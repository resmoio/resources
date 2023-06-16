---
description: Azure Active Directory User Group
---
azure_ad_user_group
-------------------

| **Name**                      | **Type**                              | **Nullable** |
| ----------------------------- | ------------------------------------- | ------------ |
| acceptedSenders               | List<DirectoryObject>                 | &check;      |
| appRoleAssignments            | List<AppRoleAssignment>               | &check;      |
| assignedLabels                | List<AssignedLabel>                   | &check;      |
| assignedLicenses              | List<AssignedLicense>                 | &check;      |
| classification                | String                                | &check;      |
| createdOnBehalfOf             | DirectoryObject                       | &check;      |
| deletedDateTime               | String                                | &check;      |
| description                   | String                                | &check;      |
| displayName                   | String                                | &check;      |
| expirationDateTime            | String                                | &check;      |
| groupTypes                    | List<String>                          | &check;      |
| hasMembersWithLicenseErrors   | Boolean                               | &check;      |
| id                            | String                                | &cross;      |
| isAssignableToRole            | Boolean                               | &check;      |
| licenseProcessingState        | LicenseProcessingState                | &check;      |
| mail                          | String                                | &check;      |
| mailEnabled                   | Boolean                               | &check;      |
| mailNickname                  | String                                | &check;      |
| memberOf                      | List<DirectoryObject>                 | &check;      |
| members                       | List<DirectoryObject>                 | &check;      |
| membersWithLicenseErrors      | List<DirectoryObject>                 | &check;      |
| membershipRule                | String                                | &check;      |
| membershipRuleProcessingState | String                                | &check;      |
| oDataType                     | String                                | &check;      |
| onPremisesDomainName          | String                                | &check;      |
| onPremisesLastSyncDateTime    | String                                | &check;      |
| onPremisesNetBiosName         | String                                | &check;      |
| onPremisesProvisioningErrors  | List<OnPremisesProvisioningError>     | &check;      |
| onPremisesSamAccountName      | String                                | &check;      |
| onPremisesSecurityIdentifier  | String                                | &check;      |
| onPremisesSyncEnabled         | Boolean                               | &check;      |
| owners                        | List<DirectoryObject>                 | &check;      |
| permissionGrants              | List<ResourceSpecificPermissionGrant> | &check;      |
| preferredDataLocation         | String                                | &check;      |
| preferredLanguage             | String                                | &check;      |
| proxyAddresses                | List<String>                          | &check;      |
| renewedDateTime               | String                                | &check;      |
| securityEnabled               | Boolean                               | &check;      |
| securityIdentifier            | String                                | &check;      |
| settings                      | List<GroupSetting>                    | &check;      |
| theme                         | String                                | &check;      |
| transitiveMemberOf            | List<DirectoryObject>                 | &check;      |
| transitiveMembers             | List<DirectoryObject>                 | &check;      |
| visibility                    | String                                | &check;      |

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

#### AssignedLabel
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| labelId     | String   | &check;      |
| oDataType   | String   | &check;      |

#### AssignedLicense
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| disabledPlans | List<String> | &check;      |
| oDataType     | String       | &check;      |
| skuId         | String       | &check;      |

#### DirectoryObject
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| oDataType | String   | &check;      |

#### GroupSetting
| **Name**    | **Type**           | **Nullable** |
| ----------- | ------------------ | ------------ |
| displayName | String             | &check;      |
| id          | String             | &check;      |
| oDataType   | String             | &check;      |
| templateId  | String             | &check;      |
| values      | Map<String,String> | &check;      |

#### LicenseProcessingState
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| oDataType | String   | &check;      |
| state     | String   | &check;      |

#### OnPremisesProvisioningError
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| category             | String   | &check;      |
| oDataType            | String   | &check;      |
| occurredDateTime     | String   | &check;      |
| propertyCausingError | String   | &check;      |
| value                | String   | &check;      |

#### ResourceSpecificPermissionGrant
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| clientAppId     | String   | &check;      |
| clientId        | String   | &check;      |
| deletedDateTime | String   | &check;      |
| id              | String   | &check;      |
| oDataType       | String   | &check;      |
| permission      | String   | &check;      |
| resourceAppId   | String   | &check;      |
