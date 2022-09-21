---
description: Azure DevOps Team
---
azure_devops_team
-----------------

| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| accountId   | String   | &cross;      |
| accountName | String   | &cross;      |
| description | String   | &check;      |
| id          | String   | &cross;      |
| identity    | Identity | &check;      |
| identityUrl | String   | &check;      |
| name        | String   | &check;      |
| projectId   | String   | &check;      |
| projectName | String   | &check;      |
| url         | String   | &check;      |

#### Identity
| **Name**            | **Type**                          | **Nullable** |
| ------------------- | --------------------------------- | ------------ |
| id                  | String                            | &check;      |
| isActive            | Boolean                           | &check;      |
| isContainer         | Boolean                           | &check;      |
| masterId            | String                            | &check;      |
| memberIds           | List<String>                      | &check;      |
| memberOf            | List<Identity.IdentityDescriptor> | &check;      |
| members             | List<Identity.IdentityDescriptor> | &check;      |
| metaTypeId          | String                            | &check;      |
| properties          | JSON                              | &check;      |
| providerDisplayName | String                            | &check;      |
| resourceVersion     | String                            | &check;      |

#### Identity.IdentityDescriptor
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| identifier   | String   | &check;      |
| identityType | String   | &check;      |
