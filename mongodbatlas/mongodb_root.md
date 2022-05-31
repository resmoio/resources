---
description: MongoDB Atlas Root
---
mongodb_root
------------

| **Name**   | **Type**   | **Nullable** |
| ---------- | ---------- | ------------ |
| apiKey     | ApiKey     | &cross;      |
| appName    | String     | &check;      |
| build      | String     | &check;      |
| links      | List<Link> | &cross;      |
| throttling | Boolean    | &check;      |

#### ApiKey
| **Name**   | **Type**     | **Nullable** |
| ---------- | ------------ | ------------ |
| accessList | List<String> | &cross;      |
| id         | String       | &cross;      |
| publicKey  | String       | &cross;      |
| roles      | List<Role>   | &cross;      |

#### Link
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| rel      | String   | &check;      |

#### Role
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| orgId    | String   | &cross;      |
| roleName | String   | &check;      |
