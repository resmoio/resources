---
description: PipeDrive Product
---
pipedrive_product
-----------------

| **Name**    | **Type**    | **Nullable** |
| ----------- | ----------- | ------------ |
| activeFlag  | Boolean     | &check;      |
| addTime     | String      | &check;      |
| category    | String      | &check;      |
| code        | String      | &check;      |
| description | String      | &check;      |
| filesCount  | Int         | &check;      |
| firstChar   | String      | &check;      |
| id          | Long        | &cross;      |
| name        | String      | &check;      |
| owner       | Owner       | &check;      |
| prices      | List<Price> | &check;      |
| selectable  | Boolean     | &check;      |
| tax         | Int         | &check;      |
| unit        | String      | &check;      |
| updateTime  | String      | &check;      |
| visibleTo   | String      | &check;      |

#### Owner
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| activeFlag | Boolean  | &check;      |
| email      | String   | &check;      |
| hasPic     | Boolean  | &check;      |
| id         | Long     | &check;      |
| name       | String   | &check;      |
| picHash    | String   | &check;      |
| value      | Long     | &check;      |

#### Price
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| cost         | Int      | &check;      |
| currency     | String   | &check;      |
| id           | Long     | &check;      |
| overheadCost | Int      | &check;      |
| price        | Int      | &check;      |
| productId    | Long     | &check;      |
