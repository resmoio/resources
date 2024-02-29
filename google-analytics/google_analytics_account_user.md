---
description: Google Analytics Account User
---
google_analytics_account_user
-----------------------------

| **Name**    | **Type**    | **Nullable** |
| ----------- | ----------- | ------------ |
| accountId   | String      | &check;      |
| id          | String      | &cross;      |
| kind        | String      | &cross;      |
| permissions | Permissions | &check;      |
| selfLink    | String      | &check;      |
| userRef     | UserRef     | &cross;      |

#### Permissions
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| effective | List<String> | &cross;      |
| local     | List<String> | &cross;      |

#### UserRef
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &cross;      |
| id       | String   | &cross;      |
| kind     | String   | &check;      |
