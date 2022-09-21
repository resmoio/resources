---
description: Azure DevOps Team Member
---
azure_devops_team_member
------------------------

| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| accountId   | String   | &cross;      |
| accountName | String   | &cross;      |
| identity    | Identity | &cross;      |
| isTeamAdmin | Boolean  | &cross;      |
| projectId   | String   | &cross;      |
| teamId      | String   | &cross;      |

#### Identity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| descriptor  | String   | &check;      |
| displayName | String   | &cross;      |
| id          | String   | &cross;      |
| imageUrl    | String   | &cross;      |
| uniqueName  | String   | &cross;      |
| url         | String   | &cross;      |
