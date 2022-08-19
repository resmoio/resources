---
description: Heroku Enterprise Account
---
heroku_enterprise_account
-------------------------

| **Name**         | **Type**         | **Nullable** |
| ---------------- | ---------------- | ------------ |
| createdAt        | String           | &check;      |
| id               | String           | &cross;      |
| identityProvider | IdentityProvider | &check;      |
| name             | String           | &check;      |
| permissions      | List<String>     | &check;      |
| trial            | Boolean          | &check;      |
| updatedAt        | String           | &check;      |

#### IdentityProvider
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| owner    | Owner    | &check;      |

#### Owner
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |
