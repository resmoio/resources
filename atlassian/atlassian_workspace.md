---
description: Atlassian Workspace
---
atlassian_workspace
-------------------

| **Name**       | **Type**           | **Nullable** |
| -------------- | ------------------ | ------------ |
| attributes     | WorkspaceAttribute | &check;      |
| id             | String             | &cross;      |
| organizationId | String             | &cross;      |

#### WorkspaceAttribute
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| capacity      | Int          | &check;      |
| createAt      | String       | &check;      |
| createdBy     | String       | &check;      |
| hostUrl       | String       | &check;      |
| labels        | List<String> | &check;      |
| name          | String       | &check;      |
| owner         | String       | &check;      |
| realm         | String       | &check;      |
| regions       | List<String> | &check;      |
| sandbox       | JSON         | &check;      |
| status        | String       | &check;      |
| statusDetails | List<String> | &check;      |
| type          | String       | &check;      |
| typeKey       | String       | &check;      |
| updatedAt     | String       | &check;      |
| usage         | Int          | &check;      |
