---
description: MonoSign User
---
monosign_user
-------------

| **Name**               | **Type**           | **Nullable** |
| ---------------------- | ------------------ | ------------ |
| additionalProperties   | Map<String,String> | &check;      |
| applicationId          | String             | &check;      |
| applicationIds         | List<String>       | &check;      |
| applicationName        | String             | &check;      |
| applicationTitle       | String             | &check;      |
| applicationUserId      | String             | &check;      |
| attributes             | Map<String,String> | &check;      |
| createdDate            | String             | &check;      |
| culture                | String             | &check;      |
| demoString             | String             | &check;      |
| email                  | String             | &check;      |
| emailAlias             | String             | &check;      |
| expirationDate         | String             | &check;      |
| formattedUserName      | String             | &check;      |
| groups                 | List<Group>        | &check;      |
| isActive               | Boolean            | &check;      |
| isExpired              | Boolean            | &check;      |
| isFavorite             | Boolean            | &check;      |
| mfa                    | Mfa                | &check;      |
| mfaRequired            | Boolean            | &check;      |
| passwordChangeRequired | Boolean            | &check;      |
| passwordChangeType     | Int                | &check;      |
| permissions            | List<Permission>   | &check;      |
| profile                | Profile            | &check;      |
| session                | Session            | &check;      |
| sourceName             | String             | &check;      |
| sourceTitle            | String             | &check;      |
| sourceUserName         | String             | &check;      |
| state                  | Int                | &check;      |
| timeZone               | String             | &check;      |
| userId                 | String             | &cross;      |
| userName               | String             | &check;      |
| userNameAlias          | String             | &check;      |

#### Group
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| source   | String   | &check;      |
| title    | String   | &check;      |

#### Mfa
| **Name**                 | **Type**                          | **Nullable** |
| ------------------------ | --------------------------------- | ------------ |
| additionalAuthenticators | List<Mfa.AdditionalAuthenticator> | &check;      |
| authenticator            | Mfa.Authenticator                 | &check;      |
| isDefined                | Boolean                           | &check;      |
| message                  | String                            | &check;      |
| requestId                | String                            | &check;      |
| title                    | String                            | &check;      |

#### Mfa.AdditionalAuthenticator
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| isDefault | Boolean  | &check;      |
| message   | String   | &check;      |
| title     | String   | &check;      |

#### Mfa.Authenticator
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| isDefault | Boolean  | &check;      |
| message   | String   | &check;      |
| title     | String   | &check;      |

#### Permission
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| isAuthorized    | Boolean  | &check;      |
| name            | String   | &check;      |
| permissionDefId | String   | &check;      |
| userId          | String   | &check;      |

#### Profile
| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| isRequireUpdate | Boolean            | &check;      |
| profileId       | String             | &check;      |
| values          | Map<String,String> | &check;      |

#### Session
| **Name**            | **Type**            | **Nullable** |
| ------------------- | ------------------- | ------------ |
| application         | Session.Application | &check;      |
| applicationId       | String              | &check;      |
| applicationUserId   | String              | &check;      |
| browserName         | String              | &check;      |
| browserVersion      | String              | &check;      |
| deviceBrand         | String              | &check;      |
| deviceModel         | String              | &check;      |
| deviceName          | String              | &check;      |
| deviceType          | Int                 | &check;      |
| expirationDate      | String              | &check;      |
| isExpired           | Boolean             | &check;      |
| isLocked            | Boolean             | &check;      |
| isMfaVerified       | Boolean             | &check;      |
| isTwoFactorRequired | Boolean             | &check;      |
| isTwoFactorVerified | Boolean             | &check;      |
| locationInfo        | String              | &check;      |
| lockMessage         | String              | &check;      |
| logoutUrl           | String              | &check;      |
| operatingSystem     | String              | &check;      |
| sessionId           | String              | &check;      |
| startDate           | String              | &check;      |
| updatedDate         | String              | &check;      |
| user                | Session.User        | &check;      |
| userId              | String              | &check;      |
| userIp              | String              | &check;      |

#### Session.Application
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| applicationId   | String   | &check;      |
| isExternalLogin | Boolean  | &check;      |
| loginFormType   | Int      | &check;      |
| loginUrl        | String   | &check;      |
| name            | String   | &check;      |
| title           | String   | &check;      |
| url             | String   | &check;      |

#### Session.User
| **Name**                     | **Type**                          | **Nullable** |
| ---------------------------- | --------------------------------- | ------------ |
| additionalProperties         | Map<String,String>                | &check;      |
| applicationIds               | List<String>                      | &check;      |
| authenticators               | List<Session.User.Authenticator>  | &check;      |
| createdDate                  | String                            | &check;      |
| culture                      | String                            | &check;      |
| defaultLoginType             | Int                               | &check;      |
| email                        | String                            | &check;      |
| emailAlias                   | String                            | &check;      |
| groups                       | List<Session.User.Group>          | &check;      |
| isActive                     | Boolean                           | &check;      |
| isTwoFactorEnabled           | Boolean                           | &check;      |
| mfa                          | Session.User.Mfa                  | &check;      |
| mfaRequired                  | Boolean                           | &check;      |
| passwordChangeType           | Int                               | &check;      |
| profile                      | Session.User.Profile              | &check;      |
| profiles                     | List<Session.User.ProfileDetails> | &check;      |
| session                      | String                            | &check;      |
| sourceName                   | String                            | &check;      |
| sourceTitle                  | String                            | &check;      |
| sourceUserName               | String                            | &check;      |
| state                        | Int                               | &check;      |
| timeZone                     | String                            | &check;      |
| updatedDate                  | String                            | &check;      |
| userAuthRequestId            | String                            | &check;      |
| userId                       | String                            | &check;      |
| userName                     | String                            | &check;      |
| userNameAlias                | String                            | &check;      |
| userRegistrationId           | String                            | &check;      |
| userSource                   | Session.User.UserSource           | &check;      |
| userSourceAccountExpiresDate | String                            | &check;      |
| userSourceId                 | String                            | &check;      |
| userSourceKey                | String                            | &check;      |
| userSourceLastLoginDate      | String                            | &check;      |
| userSourceValues             | String                            | &check;      |

#### Session.User.Authenticator
| **Name**              | **Type**                                 | **Nullable** |
| --------------------- | ---------------------------------------- | ------------ |
| authenticator         | Session.User.Authenticator.Authenticator | &check;      |
| authenticatorId       | String                                   | &check;      |
| authenticatorSecret   | String                                   | &check;      |
| createdById           | String                                   | &check;      |
| createdDate           | String                                   | &check;      |
| generatedValue        | String                                   | &check;      |
| generatedValueDate    | String                                   | &check;      |
| isDefault             | Boolean                                  | &check;      |
| isRemoved             | Boolean                                  | &check;      |
| isVerified            | Boolean                                  | &check;      |
| lastActionDate        | String                                   | &check;      |
| priority              | Int                                      | &check;      |
| requiredPropertyValue | String                                   | &check;      |
| secondPropertyValue   | String                                   | &check;      |
| state                 | Int                                      | &check;      |
| updatedDate           | String                                   | &check;      |
| userAuthenticatorId   | String                                   | &check;      |
| userDevice            | Session.User.Authenticator.UserDevice    | &check;      |
| userDeviceId          | String                                   | &check;      |
| userId                | String                                   | &check;      |
| verifiedDate          | String                                   | &check;      |
| verifiedValue         | String                                   | &check;      |

#### Session.User.Authenticator.Authenticator
| **Name**                  | **Type**                                                         | **Nullable** |
| ------------------------- | ---------------------------------------------------------------- | ------------ |
| authenticatorId           | String                                                           | &check;      |
| createdById               | String                                                           | &check;      |
| createdDate               | String                                                           | &check;      |
| data                      | String                                                           | &check;      |
| description               | String                                                           | &check;      |
| interactiveLogin          | Boolean                                                          | &check;      |
| isClientSupport           | Boolean                                                          | &check;      |
| name                      | String                                                           | &check;      |
| priority                  | Int                                                              | &check;      |
| requiredAuthenticatorId   | String                                                           | &check;      |
| requiredProfileProperty   | Session.User.Authenticator.Authenticator.RequiredProfileProperty | &check;      |
| requiredProfilePropertyId | String                                                           | &check;      |
| secondProfilePropertyId   | String                                                           | &check;      |
| settings                  | Session.User.Authenticator.Authenticator.Settings                | &check;      |
| settingsContent           | String                                                           | &check;      |
| state                     | Int                                                              | &check;      |
| title                     | String                                                           | &check;      |
| typeName                  | String                                                           | &check;      |
| userDescription           | String                                                           | &check;      |
| userTitle                 | String                                                           | &check;      |

#### Session.User.Authenticator.Authenticator.RequiredProfileProperty
| **Name**               | **Type**                                                               | **Nullable** |
| ---------------------- | ---------------------------------------------------------------------- | ------------ |
| bindingType            | Int                                                                    | &check;      |
| dataViewType           | Int                                                                    | &check;      |
| description            | String                                                                 | &check;      |
| format                 | String                                                                 | &check;      |
| getFormat              | String                                                                 | &check;      |
| getFormatType          | Int                                                                    | &check;      |
| group                  | Session.User.Authenticator.Authenticator.RequiredProfileProperty.Group | &check;      |
| isAccessibleByPublic   | Boolean                                                                | &check;      |
| isComputed             | Boolean                                                                | &check;      |
| isDisplayable          | Boolean                                                                | &check;      |
| isEditable             | Boolean                                                                | &check;      |
| isIdentity             | Boolean                                                                | &check;      |
| isRequired             | Boolean                                                                | &check;      |
| name                   | String                                                                 | &check;      |
| profilePropertyGroupId | String                                                                 | &check;      |
| profilePropertyId      | String                                                                 | &check;      |
| setFormat              | String                                                                 | &check;      |
| setFormatType          | Int                                                                    | &check;      |
| sort                   | Int                                                                    | &check;      |
| title                  | String                                                                 | &check;      |
| type                   | Int                                                                    | &check;      |
| urlSupport             | Boolean                                                                | &check;      |
| validation             | String                                                                 | &check;      |

#### Session.User.Authenticator.Authenticator.RequiredProfileProperty.Group
| **Name**                     | **Type**     | **Nullable** |
| ---------------------------- | ------------ | ------------ |
| description                  | String       | &check;      |
| name                         | String       | &check;      |
| parent                       | String       | &check;      |
| parentProfilePropertyGroupId | String       | &check;      |
| profilePropertyGroupId       | String       | &check;      |
| properties                   | List<String> | &check;      |
| sort                         | Int          | &check;      |
| title                        | String       | &check;      |

#### Session.User.Authenticator.Authenticator.Settings
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| codeIncludeChar   | Boolean  | &check;      |
| codeIncludeNumber | Boolean  | &check;      |
| codeLength        | Int      | &check;      |
| ui                | String   | &check;      |

#### Session.User.Authenticator.UserDevice
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| appName         | String   | &check;      |
| appPackageName  | String   | &check;      |
| appVersion      | String   | &check;      |
| brand           | String   | &check;      |
| carrier         | String   | &check;      |
| createdDate     | String   | &check;      |
| data            | String   | &check;      |
| deviceId        | String   | &check;      |
| deviceKey       | String   | &check;      |
| isActive        | Boolean  | &check;      |
| isRemoved       | Boolean  | &check;      |
| lastLoginDate   | String   | &check;      |
| model           | String   | &check;      |
| name            | String   | &check;      |
| operatingSystem | String   | &check;      |
| pushId          | String   | &check;      |
| sessionId       | String   | &check;      |
| settings        | String   | &check;      |
| title           | String   | &check;      |
| type            | Int      | &check;      |
| updateDate      | String   | &check;      |
| userDeviceId    | String   | &check;      |
| userId          | String   | &check;      |

#### Session.User.Group
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| source   | String   | &check;      |
| title    | String   | &check;      |

#### Session.User.Mfa
| **Name**                 | **Type**                                       | **Nullable** |
| ------------------------ | ---------------------------------------------- | ------------ |
| additionalAuthenticators | List<Session.User.Mfa.AdditionalAuthenticator> | &check;      |
| authenticator            | Session.User.Mfa.Authenticator                 | &check;      |
| isDefined                | Boolean                                        | &check;      |
| message                  | String                                         | &check;      |
| requestId                | String                                         | &check;      |
| title                    | String                                         | &check;      |

#### Session.User.Mfa.AdditionalAuthenticator
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| isDefault | Boolean  | &check;      |
| message   | String   | &check;      |
| title     | String   | &check;      |

#### Session.User.Mfa.Authenticator
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| isDefault | Boolean  | &check;      |
| message   | String   | &check;      |
| title     | String   | &check;      |

#### Session.User.Profile
| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| isRequireUpdate | Boolean            | &check;      |
| profileId       | String             | &check;      |
| values          | Map<String,String> | &check;      |

#### Session.User.ProfileDetails
| **Name**     | **Type**                                | **Nullable** |
| ------------ | --------------------------------------- | ------------ |
| createdDate  | String                                  | &check;      |
| isDefault    | Boolean                                 | &check;      |
| isEnabled    | Boolean                                 | &check;      |
| lastSyncDate | String                                  | &check;      |
| profileId    | String                                  | &check;      |
| updatedDate  | String                                  | &check;      |
| user         | String                                  | &check;      |
| userId       | String                                  | &check;      |
| values       | List<Session.User.ProfileDetails.Value> | &check;      |

#### Session.User.ProfileDetails.Value
| **Name**          | **Type**                                   | **Nullable** |
| ----------------- | ------------------------------------------ | ------------ |
| createdDate       | String                                     | &check;      |
| deserializedValue | String                                     | &check;      |
| isChangedByUser   | Boolean                                    | &check;      |
| profile           | String                                     | &check;      |
| profileId         | String                                     | &check;      |
| profilePropertyId | String                                     | &check;      |
| profileSourceId   | String                                     | &check;      |
| profileValueId    | String                                     | &check;      |
| property          | Session.User.ProfileDetails.Value.Property | &check;      |
| updatedDate       | String                                     | &check;      |
| user              | String                                     | &check;      |
| userId            | String                                     | &check;      |
| value             | String                                     | &check;      |
| values            | String                                     | &check;      |

#### Session.User.ProfileDetails.Value.Property
| **Name**               | **Type**                                         | **Nullable** |
| ---------------------- | ------------------------------------------------ | ------------ |
| bindingType            | Int                                              | &check;      |
| dataViewType           | Int                                              | &check;      |
| description            | String                                           | &check;      |
| format                 | String                                           | &check;      |
| getFormat              | String                                           | &check;      |
| getFormatType          | Int                                              | &check;      |
| group                  | Session.User.ProfileDetails.Value.Property.Group | &check;      |
| isAccessibleByPublic   | Boolean                                          | &check;      |
| isComputed             | Boolean                                          | &check;      |
| isDisplayable          | Boolean                                          | &check;      |
| isEditable             | Boolean                                          | &check;      |
| isIdentity             | Boolean                                          | &check;      |
| isRequired             | Boolean                                          | &check;      |
| name                   | String                                           | &check;      |
| profilePropertyGroupId | String                                           | &check;      |
| profilePropertyId      | String                                           | &check;      |
| setFormat              | String                                           | &check;      |
| setFormatType          | Int                                              | &check;      |
| sort                   | Int                                              | &check;      |
| title                  | String                                           | &check;      |
| type                   | Int                                              | &check;      |
| urlSupport             | Boolean                                          | &check;      |
| validation             | String                                           | &check;      |

#### Session.User.ProfileDetails.Value.Property.Group
| **Name**                     | **Type**     | **Nullable** |
| ---------------------------- | ------------ | ------------ |
| description                  | String       | &check;      |
| name                         | String       | &check;      |
| parent                       | String       | &check;      |
| parentProfilePropertyGroupId | String       | &check;      |
| profilePropertyGroupId       | String       | &check;      |
| properties                   | List<String> | &check;      |
| sort                         | Int          | &check;      |
| title                        | String       | &check;      |

#### Session.User.UserSource
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| allowPasswordChange | Boolean  | &check;      |
| autoSync            | Boolean  | &check;      |
| fullSyncEndDate     | String   | &check;      |
| fullSyncStartDate   | String   | &check;      |
| id                  | String   | &check;      |
| isExternalLogin     | Boolean  | &check;      |
| name                | String   | &check;      |
| passwordManagement  | Int      | &check;      |
| properties          | String   | &check;      |
| syncEndDate         | String   | &check;      |
| syncStartDate       | String   | &check;      |
| title               | String   | &check;      |
