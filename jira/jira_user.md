---
description: JIRA User
---
jira_user
---------

| **Name**         | **Type**              | **Nullable** |
| ---------------- | --------------------- | ------------ |
| accountId        | String                | &cross;      |
| accountType      | String                | &check;      |
| active           | Boolean               | &check;      |
| applicationRoles | List<ApplicationRole> | &check;      |
| displayName      | String                | &check;      |
| emailAddress     | String                | &check;      |
| groups           | List<String>          | &check;      |
| key              | String                | &check;      |
| name             | String                | &check;      |
| site             | String                | &check;      |
| timeZone         | String                | &check;      |

#### ApplicationRole
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| groups   | List<String> | &check;      |
| key      | String       | &cross;      |
| name     | String       | &check;      |
