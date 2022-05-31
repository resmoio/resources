---
description: Bitbucket Project
---
bitbucket_project
-----------------

| **Name**                   | **Type**  | **Nullable** |
| -------------------------- | --------- | ------------ |
| created_on                 | String    | &check;      |
| description                | String    | &check;      |
| has_publicly_visible_repos | Boolean   | &cross;      |
| is_private                 | Boolean   | &check;      |
| key                        | String    | &check;      |
| name                       | String    | &check;      |
| owner                      | Owner     | &cross;      |
| type                       | String    | &check;      |
| uuid                       | String    | &cross;      |
| workspace                  | Workspace | &cross;      |

#### Owner
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| account_id   | String   | &check;      |
| display_name | String   | &check;      |
| type         | String   | &check;      |
| uuid         | String   | &cross;      |

#### Workspace
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| slug     | String   | &check;      |
| type     | String   | &check;      |
| uuid     | String   | &check;      |
