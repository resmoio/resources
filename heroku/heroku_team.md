---
description: Heroku Team
---
heroku_team
-----------

| **Name**              | **Type**          | **Nullable** |
| --------------------- | ----------------- | ------------ |
| createdAt             | String            | &check;      |
| creditCardCollections | Boolean           | &check;      |
| default               | Boolean           | &check;      |
| enterpriseAccount     | EnterpriseAccount | &check;      |
| id                    | String            | &cross;      |
| identityProvider      | IdentityProvider  | &check;      |
| membershipLimit       | Int               | &check;      |
| name                  | String            | &check;      |
| provisionedLicenses   | Boolean           | &check;      |
| role                  | String            | &check;      |
| type                  | String            | &check;      |
| updatedAt             | String            | &check;      |

#### EnterpriseAccount
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

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
