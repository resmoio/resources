---
description: Google Analytics Account
---
google_analytics_account
------------------------

| **Name**    | **Type**    | **Nullable** |
| ----------- | ----------- | ------------ |
| childLink   | ChildLink   | &check;      |
| created     | String      | &check;      |
| id          | String      | &cross;      |
| kind        | String      | &check;      |
| name        | String      | &check;      |
| permissions | Permissions | &check;      |
| selfLink    | String      | &check;      |
| starred     | Boolean     | &check;      |
| updated     | String      | &check;      |

#### ChildLink
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &cross;      |
| type     | String   | &cross;      |

#### Permissions
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| effective | List<String> | &cross;      |
