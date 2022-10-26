---
description: JumpCloud User
---
jumpcloud_user
--------------

| **Name**                       | **Type**           | **Nullable** |
| ------------------------------ | ------------------ | ------------ |
| accountLocked                  | Boolean            | &check;      |
| accountLockedDate              | String             | &check;      |
| activated                      | Boolean            | &check;      |
| addresses                      | List<Address>      | &check;      |
| allowPublicKey                 | Boolean            | &check;      |
| alternateEmail                 | String             | &check;      |
| applications                   | List<String>       | &cross;      |
| attributes                     | List<Attribute>    | &check;      |
| badLoginAttempts               | Int                | &check;      |
| company                        | String             | &check;      |
| costCenter                     | String             | &check;      |
| created                        | String             | &check;      |
| creationSource                 | String             | &check;      |
| department                     | String             | &check;      |
| description                    | String             | &check;      |
| devices                        | List<String>       | &cross;      |
| directories                    | List<String>       | &cross;      |
| disableDeviceMaxLoginAttempts  | Boolean            | &check;      |
| displayname                    | String             | &check;      |
| email                          | String             | &check;      |
| employeeIdentifier             | String             | &check;      |
| employeeType                   | String             | &check;      |
| enableManagedUid               | Boolean            | &check;      |
| enableUserPortalMultifactor    | Boolean            | &check;      |
| externalDn                     | String             | &check;      |
| externalPasswordExpirationDate | String             | &check;      |
| externalSourceType             | String             | &check;      |
| externallyManaged              | Boolean            | &check;      |
| firstname                      | String             | &check;      |
| id                             | String             | &cross;      |
| jobTitle                       | String             | &check;      |
| lastname                       | String             | &check;      |
| ldapBindingUser                | Boolean            | &check;      |
| location                       | String             | &check;      |
| managedAppleId                 | String             | &check;      |
| manager                        | String             | &check;      |
| mfa                            | Mfa                | &check;      |
| mfaEnrollment                  | MfaEnrollment      | &check;      |
| middlename                     | String             | &check;      |
| organization                   | String             | &check;      |
| organizationId                 | String             | &cross;      |
| organizationName               | String             | &cross;      |
| passwordExpirationDate         | String             | &check;      |
| passwordExpired                | Boolean            | &check;      |
| passwordNeverExpires           | Boolean            | &check;      |
| passwordlessSudo               | Boolean            | &check;      |
| phoneNumbers                   | List<PhoneNumber>  | &check;      |
| publicKey                      | String             | &check;      |
| recoveryEmail                  | RecoveryEmail      | &check;      |
| relationships                  | List<Relationship> | &check;      |
| sambaServiceUser               | Boolean            | &check;      |
| sshKeys                        | List<SshKey>       | &check;      |
| state                          | String             | &check;      |
| sudo                           | Boolean            | &check;      |
| suspended                      | Boolean            | &check;      |
| tags                           | List<String>       | &check;      |
| totpEnabled                    | Boolean            | &check;      |
| unixGuid                       | Int                | &check;      |
| unixUid                        | Int                | &check;      |
| userGroups                     | List<String>       | &cross;      |
| username                       | String             | &check;      |

#### Address
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| country         | String   | &check;      |
| extendedAddress | String   | &check;      |
| id              | String   | &check;      |
| locality        | String   | &check;      |
| poBox           | String   | &check;      |
| postalCode      | String   | &check;      |
| region          | String   | &check;      |
| streetAddress   | String   | &check;      |
| type            | String   | &check;      |

#### Attribute
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| value    | String   | &check;      |

#### Mfa
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| configured     | Boolean  | &check;      |
| exclusion      | Boolean  | &check;      |
| exclusionDays  | Int      | &check;      |
| exclusionUntil | String   | &check;      |

#### MfaEnrollment
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| overallStatus  | String   | &check;      |
| pushStatus     | String   | &check;      |
| totpStatus     | String   | &check;      |
| webAuthnStatus | String   | &check;      |

#### PhoneNumber
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| number   | String   | &check;      |
| type     | String   | &check;      |

#### RecoveryEmail
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| address    | String   | &check;      |
| verified   | Boolean  | &check;      |
| verifiedAt | String   | &check;      |

#### Relationship
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |
| value    | String   | &check;      |

#### SshKey
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| createDate | String   | &check;      |
| id         | String   | &check;      |
| name       | String   | &check;      |
| publicKey  | String   | &check;      |
