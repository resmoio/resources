---
description: Terraform Cloud Policy Set
---
terraformcloud_policy_set
-------------------------

| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| createdAt      | String       | &check;      |
| description    | String       | &check;      |
| global         | Boolean      | &check;      |
| id             | String       | &cross;      |
| kind           | String       | &check;      |
| name           | String       | &check;      |
| policiesPath   | String       | &check;      |
| relationships  | Relationship | &check;      |
| type           | String       | &check;      |
| updatedAt      | String       | &check;      |
| versioned      | Boolean      | &check;      |
| workspaceCount | String       | &check;      |

#### Relationship
| **Name** | **Type**          | **Nullable** |
| -------- | ----------------- | ------------ |
| policies | Relationship.Data | &check;      |

#### Relationship.Data
| **Name** | **Type**                           | **Nullable** |
| -------- | ---------------------------------- | ------------ |
| data     | List<Relationship.Data.PolicyInfo> | &check;      |

#### Relationship.Data.PolicyInfo
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| type     | String   | &check;      |
