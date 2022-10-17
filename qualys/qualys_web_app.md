---
description: Qualys Web App
---
qualys_web_app
--------------

| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| createdDate | String   | &check;      |
| id          | String   | &cross;      |
| name        | String   | &check;      |
| owner       | Owner    | &check;      |
| tags        | Tags     | &check;      |
| updatedDate | String   | &check;      |
| url         | String   | &check;      |

#### Owner
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| firstName | String   | &check;      |
| id        | String   | &check;      |
| lastName  | String   | &check;      |
| username  | String   | &check;      |

#### Tags
| **Name** | **Type**       | **Nullable** |
| -------- | -------------- | ------------ |
| count    | Int            | &check;      |
| list     | List<Tags.Tag> | &check;      |

#### Tags.Tag
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &check;      |
| name     | String   | &check;      |
