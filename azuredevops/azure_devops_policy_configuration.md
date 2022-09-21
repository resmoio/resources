---
description: Azure DevOps Policy Configuration
---
azure_devops_policy_configuration
---------------------------------

| **Name**            | **Type**   | **Nullable** |
| ------------------- | ---------- | ------------ |
| accountId           | String     | &cross;      |
| accountName         | String     | &cross;      |
| createdBy           | Identity   | &check;      |
| createdDate         | String     | &check;      |
| id                  | String     | &cross;      |
| isBlocking          | Boolean    | &check;      |
| isDeleted           | Boolean    | &check;      |
| isEnabled           | Boolean    | &check;      |
| isEnterpriseManaged | Boolean    | &check;      |
| projectId           | String     | &cross;      |
| revision            | Int        | &check;      |
| settings            | JSON       | &check;      |
| type                | PolicyType | &check;      |
| url                 | String     | &check;      |

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

#### PolicyType
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| id          | String   | &check;      |
| url         | String   | &check;      |
