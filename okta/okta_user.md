---
description: Okta User
---
okta_user
---------

| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| activated       | String       | &check;      |
| created         | String       | &check;      |
| credentials     | Credentials  | &check;      |
| id              | String       | &cross;      |
| lastLogin       | String       | &check;      |
| lastUpdated     | String       | &check;      |
| mfaEnabled      | Boolean      | &check;      |
| passwordChanged | String       | &check;      |
| profile         | Profile      | &check;      |
| roleIds         | List<String> | &check;      |
| status          | String       | &check;      |
| statusChanged   | String       | &check;      |
| type            | Type         | &check;      |

#### Credentials
| **Name** | **Type**             | **Nullable** |
| -------- | -------------------- | ------------ |
| provider | Credentials.Provider | &check;      |

#### Credentials.Provider
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### Profile
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| email     | String   | &check;      |
| firstName | String   | &check;      |
| lastName  | String   | &check;      |
| login     | String   | &check;      |

#### Type
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
