---
description: Azure DevOps Plan
---
azure_devops_plan
-----------------

| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| accountId          | String   | &cross;      |
| accountName        | String   | &cross;      |
| createdByIdentity  | Identity | &check;      |
| createdDate        | String   | &check;      |
| description        | String   | &check;      |
| id                 | String   | &cross;      |
| modifiedByIdentity | Identity | &check;      |
| modifiedDate       | String   | &check;      |
| name               | String   | &check;      |
| projectId          | String   | &cross;      |
| properties         | JSON     | &check;      |
| revision           | Int      | &check;      |
| type               | String   | &check;      |
| url                | String   | &check;      |
| userPermissions    | Long     | &check;      |

#### Identity
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| descriptor    | String   | &check;      |
| displayName   | String   | &check;      |
| id            | String   | &check;      |
| imageUrl      | String   | &check;      |
| inactive      | Boolean  | &check;      |
| isAadIdentity | Boolean  | &check;      |
| profileUrl    | String   | &check;      |
| uniqueName    | String   | &check;      |
| url           | String   | &check;      |
