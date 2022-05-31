---
description: MongoDB Atlas API Key
---
mongodb_programmatic_api_key
----------------------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| desc         | String       | &check;      |
| id           | String       | &cross;      |
| links        | List<Link>   | &cross;      |
| organization | Organization | &cross;      |
| privateKey   | String       | &check;      |
| publicKey    | String       | &check;      |
| roles        | List<Role>   | &cross;      |

#### Link
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| rel      | String   | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |

#### Role
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupId  | String   | &check;      |
| orgId    | String   | &check;      |
| roleName | String   | &check;      |
