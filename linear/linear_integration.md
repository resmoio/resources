---
description: Linear Integration
---
linear_integration
------------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| archivedAt   | String       | &check;      |
| createdAt    | String       | &check;      |
| creator      | Creator      | &check;      |
| id           | String       | &cross;      |
| organization | Organization | &check;      |
| service      | String       | &check;      |
| team         | Team         | &check;      |
| updatedAt    | String       | &check;      |

#### Creator
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
