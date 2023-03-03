---
description: MonoSign User Authenticator
---
monosign_user_authenticator
---------------------------

| **Name**              | **Type**      | **Nullable** |
| --------------------- | ------------- | ------------ |
| authenticator         | Authenticator | &check;      |
| authenticatorId       | String        | &check;      |
| authenticatorSecret   | String        | &check;      |
| createdById           | String        | &check;      |
| createdDate           | String        | &check;      |
| generatedValue        | String        | &check;      |
| generatedValueDate    | String        | &check;      |
| isDefault             | Boolean       | &check;      |
| isRemoved             | Boolean       | &check;      |
| isVerified            | Boolean       | &check;      |
| lastActionDate        | String        | &check;      |
| priority              | Int           | &check;      |
| requiredPropertyValue | String        | &check;      |
| secondPropertyValue   | String        | &check;      |
| state                 | Int           | &check;      |
| updatedDate           | String        | &check;      |
| userAuthenticatorId   | String        | &cross;      |
| userDevice            | UserDevice    | &check;      |
| userDeviceId          | String        | &check;      |
| userId                | String        | &check;      |
| verifiedDate          | String        | &check;      |
| verifiedValue         | String        | &check;      |

#### Authenticator
| **Name**                  | **Type**                              | **Nullable** |
| ------------------------- | ------------------------------------- | ------------ |
| authenticatorId           | String                                | &check;      |
| createdById               | String                                | &check;      |
| createdDate               | String                                | &check;      |
| data                      | String                                | &check;      |
| description               | String                                | &check;      |
| interactiveLogin          | Boolean                               | &check;      |
| isClientSupport           | Boolean                               | &check;      |
| name                      | String                                | &check;      |
| priority                  | Int                                   | &check;      |
| requiredAuthenticatorId   | String                                | &check;      |
| requiredProfileProperty   | Authenticator.RequiredProfileProperty | &check;      |
| requiredProfilePropertyId | String                                | &check;      |
| secondProfilePropertyId   | String                                | &check;      |
| settings                  | Authenticator.Settings                | &check;      |
| settingsContent           | String                                | &check;      |
| state                     | Int                                   | &check;      |
| title                     | String                                | &check;      |
| typeName                  | String                                | &check;      |
| userDescription           | String                                | &check;      |
| userTitle                 | String                                | &check;      |

#### Authenticator.RequiredProfileProperty
| **Name**               | **Type**                                    | **Nullable** |
| ---------------------- | ------------------------------------------- | ------------ |
| bindingType            | Int                                         | &check;      |
| dataViewType           | Int                                         | &check;      |
| description            | String                                      | &check;      |
| format                 | String                                      | &check;      |
| getFormat              | String                                      | &check;      |
| getFormatType          | Int                                         | &check;      |
| group                  | Authenticator.RequiredProfileProperty.Group | &check;      |
| isAccessibleByPublic   | Boolean                                     | &check;      |
| isComputed             | Boolean                                     | &check;      |
| isDisplayable          | Boolean                                     | &check;      |
| isEditable             | Boolean                                     | &check;      |
| isIdentity             | Boolean                                     | &check;      |
| isRequired             | Boolean                                     | &check;      |
| name                   | String                                      | &check;      |
| profilePropertyGroupId | String                                      | &check;      |
| profilePropertyId      | String                                      | &check;      |
| setFormat              | String                                      | &check;      |
| setFormatType          | Int                                         | &check;      |
| sort                   | Int                                         | &check;      |
| title                  | String                                      | &check;      |
| type                   | Int                                         | &check;      |
| urlSupport             | Boolean                                     | &check;      |
| validation             | String                                      | &check;      |

#### Authenticator.RequiredProfileProperty.Group
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

#### Authenticator.Settings
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| codeIncludeChar   | Boolean  | &check;      |
| codeIncludeNumber | Boolean  | &check;      |
| codeLength        | Int      | &check;      |
| ui                | String   | &check;      |

#### UserDevice
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
