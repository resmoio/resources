---
description: Resmo Resource Auto Tagging Config
---
resmo_auto_tagging
------------------

| **Name**   | **Type**                      | **Nullable** |
| ---------- | ----------------------------- | ------------ |
| accountId  | String                        | &check;      |
| createdBy  | String                        | &check;      |
| expression | ResmoResourceFilterExpression | &check;      |
| id         | String                        | &cross;      |
| name       | String                        | &check;      |
| state      | String                        | &check;      |
| tags       | Set                           | &check;      |
| updatedBy  | String                        | &check;      |

#### ResmoResourceFilterExpression
| **Name** | **Type**                                   | **Nullable** |
| -------- | ------------------------------------------ | ------------ |
| filters  | List<ResmoResourceFilterExpression.Filter> | &cross;      |

#### ResmoResourceFilterExpression.Filter
| **Name**         | **Type**         | **Nullable** |
| ---------------- | ---------------- | ------------ |
| fields           | Map<String,List> | &cross;      |
| integrationTypes | List<String>     | &cross;      |
| resources        | List<String>     | &cross;      |
| tags             | Set              | &cross;      |
