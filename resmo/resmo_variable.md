---
description: Resmo Variable
---
resmo_variable
--------------

| **Name**     | **Type**             | **Nullable** |
| ------------ | -------------------- | ------------ |
| defaultValue | JSON                 | &check;      |
| description  | String               | &check;      |
| isManaged    | Boolean              | &cross;      |
| modifiedAt   | Timestamp            | &check;      |
| modifiedBy   | String               | &check;      |
| name         | String               | &cross;      |
| type         | String               | &check;      |
| values       | List<ValuePerDomain> | &cross;      |

#### ValuePerDomain
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| domain   | String   | &cross;      |
| value    | JSON     | &cross;      |
