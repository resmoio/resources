---
description: Datadog User
---
datadog_user
------------

| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| createdAt          | String       | &check;      |
| disabled           | Boolean      | &check;      |
| email              | String       | &check;      |
| handle             | String       | &check;      |
| icon               | String       | &check;      |
| id                 | String       | &cross;      |
| name               | String       | &check;      |
| organization       | String       | &check;      |
| otherOrganizations | List<String> | &check;      |
| otherUsers         | List<String> | &check;      |
| roles              | List<String> | &check;      |
| serviceAccount     | Boolean      | &check;      |
| status             | String       | &check;      |
| teams              | List<Team>   | &check;      |
| title              | String       | &check;      |
| verified           | Boolean      | &check;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| role     | String   | &check;      |
