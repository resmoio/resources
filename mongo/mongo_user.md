---
description: MongoDB User
---
mongo_user
----------

| **Name**     | **Type**  | **Nullable** |
| ------------ | --------- | ------------ |
| db           | String    | &check;      |
| dbIdentifier | String    | &cross;      |
| name         | String    | &check;      |
| roles        | List<Map> | &check;      |

#### MongoResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
