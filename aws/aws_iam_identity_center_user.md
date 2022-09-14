---
description: Amazon Web Services IAM Identity Center User
---
aws_iam_identity_center_user
----------------------------

| **Name**          | **Type**          | **Nullable** |
| ----------------- | ----------------- | ------------ |
| addresses         | List<Address>     | &cross;      |
| displayName       | String            | &cross;      |
| email             | String            | &check;      |
| emails            | List<Email>       | &cross;      |
| externalIds       | List<ExternalId>  | &cross;      |
| identityStoreId   | String            | &cross;      |
| locale            | String            | &check;      |
| name              | Name              | &check;      |
| nickName          | String            | &check;      |
| phoneNumbers      | List<PhoneNumber> | &cross;      |
| preferredLanguage | String            | &check;      |
| profileUrl        | String            | &check;      |
| title             | String            | &check;      |
| userId            | String            | &cross;      |
| userName          | String            | &cross;      |
| userType          | String            | &check;      |

#### Address
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| country       | String   | &check;      |
| formatted     | String   | &check;      |
| locality      | String   | &check;      |
| postalCode    | String   | &check;      |
| primary       | Boolean  | &check;      |
| region        | String   | &check;      |
| streetAddress | String   | &check;      |
| type          | String   | &check;      |

#### Email
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| primary  | Boolean  | &check;      |
| type     | String   | &check;      |
| value    | String   | &cross;      |

#### ExternalId
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| issuer   | String   | &check;      |

#### Name
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| familyName      | String   | &check;      |
| formatted       | String   | &check;      |
| givenName       | String   | &check;      |
| honorificPrefix | String   | &check;      |
| honorificSuffix | String   | &check;      |

#### PhoneNumber
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| primary  | Boolean  | &check;      |
| type     | String   | &check;      |
| value    | String   | &check;      |
