---
description: Google Workspace User
---
gsuite_user
-----------

| **Name**                   | **Type**           | **Nullable** |
| -------------------------- | ------------------ | ------------ |
| addresses                  | List<Address>      | &check;      |
| agreedToTerms              | Boolean            | &check;      |
| aliases                    | List<String>       | &check;      |
| archived                   | Boolean            | &check;      |
| changePasswordAtNextLogin  | Boolean            | &check;      |
| creationTime               | String             | &check;      |
| customerId                 | String             | &cross;      |
| deletionTime               | String             | &check;      |
| emails                     | List<Email>        | &check;      |
| externalIds                | List<ExternalId>   | &check;      |
| gender                     | Gender             | &check;      |
| id                         | String             | &check;      |
| ims                        | List<Im>           | &check;      |
| includeInGlobalAddressList | Boolean            | &check;      |
| ipWhitelisted              | Boolean            | &check;      |
| isAdmin                    | Boolean            | &check;      |
| isDelegatedAdmin           | Boolean            | &check;      |
| isEnforcedIn2Sv            | Boolean            | &check;      |
| isEnrolledIn2Sv            | Boolean            | &check;      |
| isMailboxSetup             | Boolean            | &check;      |
| keywords                   | List<Keyword>      | &check;      |
| languages                  | List<Language>     | &check;      |
| locations                  | List<Location>     | &check;      |
| name                       | Name               | &check;      |
| nonEditableAliases         | List<String>       | &check;      |
| orgUnitPath                | String             | &check;      |
| organizations              | List<Organization> | &check;      |
| phones                     | List<Phone>        | &check;      |
| posixAccounts              | List<PosixAccount> | &check;      |
| primaryEmail               | String             | &cross;      |
| recoveryEmail              | String             | &check;      |
| recoveryPhone              | String             | &check;      |
| relations                  | List<Relation>     | &check;      |
| sshPublicKeys              | List<SshPublicKey> | &check;      |
| suspended                  | Boolean            | &check;      |
| suspensionReason           | String             | &check;      |

#### Address
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| country            | String   | &check;      |
| countryCode        | String   | &check;      |
| customType         | String   | &check;      |
| extendedAddress    | String   | &check;      |
| formatted          | String   | &check;      |
| locality           | String   | &check;      |
| poBox              | String   | &check;      |
| postalCode         | String   | &check;      |
| primary            | Boolean  | &check;      |
| region             | String   | &check;      |
| sourceIsStructured | Boolean  | &check;      |
| streetAddress      | String   | &check;      |
| type               | String   | &check;      |

#### Email
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| address    | String   | &check;      |
| customType | String   | &check;      |
| primary    | Boolean  | &check;      |
| type       | String   | &check;      |

#### ExternalId
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| customType | String   | &check;      |
| type       | String   | &check;      |
| value      | String   | &check;      |

#### Gender
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| addressMeAs  | String   | &check;      |
| customGender | String   | &check;      |
| type         | String   | &check;      |

#### Im
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| customProtocol | String   | &check;      |
| customType     | String   | &check;      |
| im             | String   | &check;      |
| primary        | Boolean  | &check;      |
| protocol       | String   | &check;      |
| type           | String   | &check;      |

#### Keyword
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| customType | String   | &check;      |
| type       | String   | &check;      |
| value      | String   | &check;      |

#### Language
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| customLanguage | String   | &check;      |
| languageCode   | String   | &check;      |
| preference     | String   | &check;      |

#### Location
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| area         | String   | &check;      |
| buildingId   | String   | &check;      |
| customType   | String   | &check;      |
| deskCode     | String   | &check;      |
| floorName    | String   | &check;      |
| floorSection | String   | &check;      |
| type         | String   | &check;      |

#### Name
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| familyName | String   | &check;      |
| fullName   | String   | &check;      |
| givenName  | String   | &check;      |

#### Organization
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| costCenter         | String   | &check;      |
| customType         | String   | &check;      |
| department         | String   | &check;      |
| description        | String   | &check;      |
| domain             | String   | &check;      |
| fullTimeEquivalent | Int      | &check;      |
| location           | String   | &check;      |
| name               | String   | &check;      |
| primary            | Boolean  | &check;      |
| symbol             | String   | &check;      |
| title              | String   | &check;      |
| type               | String   | &check;      |

#### Phone
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| customType | String   | &check;      |
| primary    | Boolean  | &check;      |
| type       | String   | &check;      |
| value      | String   | &check;      |

#### PosixAccount
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| accountId           | String   | &check;      |
| gecos               | String   | &check;      |
| gid                 | Long     | &check;      |
| homeDirectory       | String   | &check;      |
| operatingSystemType | String   | &check;      |
| primary             | Boolean  | &check;      |
| shell               | String   | &check;      |
| systemId            | String   | &check;      |
| uid                 | Long     | &check;      |
| username            | String   | &check;      |

#### Relation
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| customType | String   | &check;      |
| type       | String   | &check;      |
| value      | String   | &check;      |

#### SshPublicKey
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| expirationTimeUsec | Long     | &check;      |
| fingerprint        | String   | &check;      |
| key                | String   | &check;      |
