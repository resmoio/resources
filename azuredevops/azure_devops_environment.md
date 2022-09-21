---
description: Azure DevOps Environment
---
azure_devops_environment
------------------------

| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| accountId      | String         | &cross;      |
| accountName    | String         | &cross;      |
| createdBy      | Identity       | &check;      |
| createdOn      | String         | &check;      |
| description    | String         | &check;      |
| id             | String         | &cross;      |
| lastModifiedBy | Identity       | &check;      |
| lastModifiedOn | String         | &check;      |
| name           | String         | &check;      |
| project        | Project        | &check;      |
| resources      | List<Resource> | &check;      |

#### Identity
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| displayName   | String   | &check;      |
| id            | String   | &check;      |
| imageUrl      | String   | &check;      |
| isAadIdentity | Boolean  | &check;      |
| isContainer   | Boolean  | &check;      |
| profileUrl    | String   | &check;      |
| uniqueName    | String   | &check;      |
| url           | String   | &check;      |

#### Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Resource
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| id       | String       | &check;      |
| name     | String       | &check;      |
| tags     | List<String> | &check;      |
| type     | String       | &check;      |
