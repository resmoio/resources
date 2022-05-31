---
description: Resmo Resource Group
---
resmo_resource_group
--------------------

| **Name**   | **Type**                      | **Nullable** |
| ---------- | ----------------------------- | ------------ |
| expression | ResmoResourceFilterExpression | &check;      |
| id         | String                        | &cross;      |
| name       | String                        | &check;      |

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
