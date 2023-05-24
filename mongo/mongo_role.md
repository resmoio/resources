---
description: MongoDB Role
---
mongo_role
----------

| **Name**       | **Type**  | **Nullable** |
| -------------- | --------- | ------------ |
| db             | String    | &check;      |
| dbIdentifier   | String    | &cross;      |
| inheritedRoles | List<Map> | &check;      |
| name           | String    | &check;      |
| roles          | List<Map> | &check;      |

#### MongoResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
