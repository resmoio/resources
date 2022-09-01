---
description: Heroku Team Member
---
heroku_team_member
------------------

| **Name**                | **Type**         | **Nullable** |
| ----------------------- | ---------------- | ------------ |
| createdAt               | String           | &check;      |
| email                   | String           | &check;      |
| federated               | Boolean          | &check;      |
| id                      | String           | &cross;      |
| identityProvider        | IdentityProvider | &check;      |
| role                    | String           | &check;      |
| team                    | Team             | &check;      |
| twoFactorAuthentication | Boolean          | &check;      |
| updatedAt               | String           | &check;      |
| user                    | User             | &check;      |

#### IdentityProvider
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| owner    | Owner    | &check;      |
| redacted | Boolean  | &check;      |

#### Owner
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| id       | String   | &check;      |
| name     | String   | &check;      |
