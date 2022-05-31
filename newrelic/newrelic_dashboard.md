---
description: New Relic Dashboard
---
newrelic_dashboard
------------------

| **Name**            | **Type**   | **Nullable** |
| ------------------- | ---------- | ------------ |
| accountId           | Int        | &cross;      |
| dashboardParentGuid | String     | &check;      |
| description         | String     | &check;      |
| guid                | String     | &cross;      |
| name                | String     | &cross;      |
| owner               | Int        | &check;      |
| pages               | List<Page> | &check;      |
| permalink           | String     | &cross;      |
| permissions         | String     | &check;      |
| updatedAt           | String     | &check;      |

#### Page
| **Name**  | **Type**          | **Nullable** |
| --------- | ----------------- | ------------ |
| createdAt | Date              | &cross;      |
| guid      | String            | &cross;      |
| name      | String            | &cross;      |
| owner     | Int               | &check;      |
| updatedAt | Date              | &cross;      |
| widgets   | List<Page.Widget> | &cross;      |

#### Page.NewRelicQuery
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| accountId | Int      | &check;      |
| query     | String   | &check;      |

#### Page.Widget
| **Name**    | **Type**                 | **Nullable** |
| ----------- | ------------------------ | ------------ |
| id          | String                   | &cross;      |
| nrqlQueries | List<Page.NewRelicQuery> | &check;      |
| title       | String                   | &check;      |
