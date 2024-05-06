---
description: Okta Authorization Server
---
okta_authorization_server
-------------------------

| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| audiences   | List<String> | &check;      |
| created     | String       | &check;      |
| credentials | Credentials  | &check;      |
| description | String       | &check;      |
| id          | String       | &cross;      |
| issuer      | String       | &check;      |
| issuerMode  | String       | &check;      |
| lastUpdated | String       | &check;      |
| name        | String       | &check;      |
| status      | String       | &check;      |

#### Credentials
| **Name** | **Type**            | **Nullable** |
| -------- | ------------------- | ------------ |
| signing  | Credentials.Signing | &check;      |

#### Credentials.Signing
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| lastRotated  | String   | &check;      |
| nextRotation | String   | &check;      |
| rotationMode | String   | &check;      |
