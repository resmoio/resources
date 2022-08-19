---
description: Heroku Enterprise Account Member
---
heroku_enterprise_account_member
--------------------------------

| **Name**                | **Type**          | **Nullable** |
| ----------------------- | ----------------- | ------------ |
| enterpriseAccount       | EnterpriseAccount | &check;      |
| id                      | String            | &cross;      |
| identityProvider        | IdentityProvider  | &check;      |
| permissions             | List<Permission>  | &check;      |
| twoFactorAuthentication | Boolean           | &check;      |
| user                    | User              | &check;      |

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
| redacted | Boolean  | &check;      |

#### Owner
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### Permission
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| name        | String   | &check;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| id       | String   | &check;      |
