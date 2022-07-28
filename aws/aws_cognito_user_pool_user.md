---
description: Amazon Web Services Cognito User Pool User
---
aws_cognito_user_pool_user
--------------------------

| **Name**             | **Type**        | **Nullable** |
| -------------------- | --------------- | ------------ |
| accountId            | String          | &cross;      |
| attributes           | List<Attribute> | &check;      |
| enabled              | Boolean         | &check;      |
| mfaOptions           | List<MFAOption> | &check;      |
| region               | String          | &cross;      |
| userCreateDate       | String          | &check;      |
| userLastModifiedDate | String          | &check;      |
| userPoolId           | String          | &cross;      |
| userStatus           | String          | &check;      |
| username             | String          | &cross;      |

#### Attribute
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| value    | String   | &check;      |

#### MFAOption
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| attributeName  | String   | &check;      |
| deliveryMedium | String   | &check;      |
