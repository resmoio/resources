---
description: GitHub Team Repository
---
github_team_repo
----------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| organization | Organization | &check;      |
| permissions  | Permissions  | &cross;      |
| repository   | Repository   | &cross;      |
| roleName     | String       | &check;      |
| team         | Team         | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Owner
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &cross;      |
| login     | String   | &cross;      |
| nodeId    | String   | &cross;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |

#### Permissions
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| admin    | Boolean  | &check;      |
| maintain | Boolean  | &check;      |
| pull     | Boolean  | &check;      |
| push     | Boolean  | &check;      |
| triage   | Boolean  | &check;      |

#### Repository
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| fork        | Boolean  | &check;      |
| fullName    | String   | &cross;      |
| id          | Long     | &cross;      |
| name        | String   | &cross;      |
| nodeId      | String   | &cross;      |
| owner       | Owner    | &cross;      |
| private     | Boolean  | &check;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
