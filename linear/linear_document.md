---
description: Linear Document
---
linear_document
---------------

| **Name**   | **Type**  | **Nullable** |
| ---------- | --------- | ------------ |
| archivedAt | String    | &check;      |
| content    | String    | &check;      |
| createdAt  | String    | &check;      |
| creator    | Creator   | &check;      |
| id         | String    | &cross;      |
| project    | Project   | &check;      |
| slugId     | String    | &check;      |
| title      | String    | &check;      |
| updatedAt  | String    | &check;      |
| updatedBy  | UpdatedBy | &check;      |

#### Creator
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### UpdatedBy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
