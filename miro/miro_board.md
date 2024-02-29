---
description: Miro Board
---
miro_board
----------

| **Name**     | **Type**   | **Nullable** |
| ------------ | ---------- | ------------ |
| boardMembers | List<User> | &check;      |
| createdBy    | User       | &check;      |
| description  | String     | &check;      |
| id           | String     | &cross;      |
| name         | String     | &check;      |
| owner        | User       | &check;      |
| type         | String     | &check;      |
| viewLink     | String     | &check;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |
| type     | String   | &check;      |
