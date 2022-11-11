---
description: Terraform Cloud Team Access
---
terraformcloud_team_access
--------------------------

| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| access           | String       | &check;      |
| id               | String       | &cross;      |
| relationships    | Relationship | &check;      |
| runTasks         | Boolean      | &check;      |
| runs             | String       | &check;      |
| sentinelMocks    | String       | &check;      |
| stateVersions    | String       | &check;      |
| type             | String       | &check;      |
| variables        | String       | &check;      |
| workspaceId      | String       | &check;      |
| workspaceLocking | Boolean      | &check;      |

#### Relationship
| **Name** | **Type**          | **Nullable** |
| -------- | ----------------- | ------------ |
| team     | Relationship.Team | &check;      |

#### Relationship.Team
| **Name** | **Type**               | **Nullable** |
| -------- | ---------------------- | ------------ |
| data     | Relationship.Team.Data | &check;      |

#### Relationship.Team.Data
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
