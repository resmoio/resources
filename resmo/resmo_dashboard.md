---
description: Resmo Dashboard
---
resmo_dashboard
---------------

| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| accountId   | String       | &check;      |
| description | String       | &check;      |
| id          | String       | &cross;      |
| name        | String       | &check;      |
| tags        | List<String> | &check;      |
| widgets     | List<Widget> | &check;      |

#### Widget
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| configuration | JSON     | &cross;      |
| title         | String   | &cross;      |
| type          | String   | &cross;      |
