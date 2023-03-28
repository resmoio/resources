---
description: Resmo Pack
---
resmo_pack
----------

| **Name**    | **Type**         | **Nullable** |
| ----------- | ---------------- | ------------ |
| accountId   | String           | &check;      |
| controls    | List<Control>    | &check;      |
| createdAt   | Timestamp        | &check;      |
| createdBy   | String           | &check;      |
| description | String           | &check;      |
| id          | String           | &cross;      |
| isManaged   | Boolean          | &check;      |
| labels      | List<String>     | &check;      |
| name        | String           | &check;      |
| sources     | List<Datasource> | &check;      |
| updatedAt   | Timestamp        | &check;      |
| updatedBy   | String           | &check;      |

#### Control
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| id          | String   | &cross;      |
| name        | String   | &check;      |
| packId      | String   | &check;      |
| parentId    | String   | &check;      |
| pos         | Int      | &check;      |

#### Datasource
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| controlId | String   | &check;      |
| id        | String   | &cross;      |
| packId    | String   | &check;      |
| pos       | Int      | &check;      |
| ruleId    | String   | &check;      |
| type      | String   | &check;      |
