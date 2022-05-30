---
description: JIRA Filter
---
jira_filter
-----------

| **Name**         | **Type**         | **Nullable** |
| ---------------- | ---------------- | ------------ |
| description      | String           | &check;      |
| editPermissions  | List<Permission> | &check;      |
| favouritedCount  | Int              | &check;      |
| id               | String           | &cross;      |
| jql              | String           | &check;      |
| name             | String           | &check;      |
| owner            | String           | &check;      |
| sharePermissions | List<Permission> | &check;      |
| sharedUsers      | List<String>     | &check;      |
| site             | String           | &cross;      |
| subscriptions    | List<String>     | &check;      |

#### Permission
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| group    | String   | &check;      |
| id       | Int      | &cross;      |
| project  | Int      | &check;      |
| type     | String   | &check;      |
| user     | String   | &check;      |
