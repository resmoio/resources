---
description: Azure Active Directory Contact
---
azure_ad_contact
----------------

| **Name**                     | **Type**                          | **Nullable** |
| ---------------------------- | --------------------------------- | ------------ |
| addresses                    | List<PhysicalOfficeAddress>       | &check;      |
| companyName                  | String                            | &check;      |
| department                   | String                            | &check;      |
| directReports                | List<DirectoryObject>             | &check;      |
| displayName                  | String                            | &check;      |
| givenName                    | String                            | &check;      |
| id                           | String                            | &cross;      |
| jobTitle                     | String                            | &check;      |
| mail                         | String                            | &check;      |
| mailNickname                 | String                            | &check;      |
| manager                      | DirectoryObject                   | &check;      |
| memberOf                     | List<DirectoryObject>             | &check;      |
| oDataType                    | String                            | &check;      |
| onPremisesLastSyncDateTime   | String                            | &check;      |
| onPremisesProvisioningErrors | List<OnPremisesProvisioningError> | &check;      |
| onPremisesSyncEnabled        | Boolean                           | &check;      |
| phones                       | List<Phone>                       | &check;      |
| proxyAddresses               | List<String>                      | &check;      |
| surname                      | String                            | &check;      |
| transitiveMemberOf           | List<DirectoryObject>             | &check;      |

#### DirectoryObject
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| oDataType | String   | &check;      |

#### OnPremisesProvisioningError
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| category             | String   | &check;      |
| oDataType            | String   | &check;      |
| occurredDateTime     | String   | &check;      |
| propertyCausingError | String   | &check;      |
| value                | String   | &check;      |

#### Phone
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| language  | String   | &check;      |
| number    | String   | &check;      |
| oDataType | String   | &check;      |
| region    | String   | &check;      |
| type      | String   | &check;      |

#### PhysicalOfficeAddress
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| city            | String   | &check;      |
| countryOrRegion | String   | &check;      |
| oDataType       | String   | &check;      |
| officeLocation  | String   | &check;      |
| postalCode      | String   | &check;      |
| state           | String   | &check;      |
| street          | String   | &check;      |
