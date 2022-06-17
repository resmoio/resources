---
description: Bitbucket Deploy Key
---
bitbucket_deploy_key
--------------------

| **Name**     | **Type**   | **Nullable** |
| ------------ | ---------- | ------------ |
| added_on     | String     | &check;      |
| comment      | String     | &check;      |
| key          | String     | &cross;      |
| label        | String     | &check;      |
| last_used    | String     | &check;      |
| owner        | Owner      | &check;      |
| repository   | Repository | &cross;      |
| workspace_id | String     | &cross;      |

#### Owner
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| account_id   | String   | &check;      |
| display_name | String   | &check;      |
| type         | String   | &check;      |
| uuid         | String   | &check;      |

#### Repository
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| full_name | String   | &check;      |
| name      | String   | &check;      |
| type      | String   | &check;      |
| uuid      | String   | &cross;      |
