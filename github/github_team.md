---
description: GitHub Team
---
github_team
-----------

| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| createdAt      | Date         | &check;      |
| description    | String       | &check;      |
| id             | Long         | &cross;      |
| membersCount   | Long         | &check;      |
| name           | String       | &cross;      |
| nodeId         | String       | &cross;      |
| organization   | Organization | &check;      |
| organizationId | String       | &cross;      |
| parent         | Parent       | &check;      |
| permission     | String       | &check;      |
| privacy        | String       | &check;      |
| reposCount     | Long         | &check;      |
| slug           | String       | &cross;      |
| updatedAt      | Date         | &check;      |

#### Organization
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| id          | Long     | &cross;      |
| login       | String   | &cross;      |
| name        | String   | &check;      |
| nodeId      | String   | &cross;      |
| type        | String   | &check;      |

#### Parent
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| id          | Long     | &cross;      |
| name        | String   | &cross;      |
| nodeId      | String   | &check;      |
| permission  | String   | &check;      |
| privacy     | String   | &check;      |
| slug        | String   | &check;      |

#### Repository
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| fullName | String   | &check;      |
| id       | Long     | &cross;      |
| name     | String   | &cross;      |
| nodeId   | String   | &check;      |
| private  | Boolean  | &check;      |

#### User
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &cross;      |
| login     | String   | &cross;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |
