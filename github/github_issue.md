---
description: GitHub Issue
---
github_issue
------------

| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| assignee          | User         | &check;      |
| assignees         | List<User>   | &check;      |
| authorAssociation | String       | &check;      |
| body              | String       | &check;      |
| closedAt          | Date         | &check;      |
| closedBy          | User         | &check;      |
| comments          | Int          | &check;      |
| createdAt         | Date         | &check;      |
| id                | Long         | &cross;      |
| labels            | List<Label>  | &check;      |
| locked            | Boolean      | &check;      |
| milestone         | Milestone    | &check;      |
| nodeId            | String       | &cross;      |
| number            | Long         | &cross;      |
| organization      | Organization | &cross;      |
| organizationId    | String       | &cross;      |
| repository        | Repository   | &cross;      |
| repositoryId      | String       | &cross;      |
| state             | String       | &check;      |
| title             | String       | &check;      |
| updatedAt         | Date         | &check;      |
| user              | User         | &check;      |

#### Label
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| color       | String   | &check;      |
| default     | Boolean  | &check;      |
| description | String   | &check;      |
| id          | Long     | &check;      |
| name        | String   | &check;      |
| nodeId      | String   | &check;      |

#### Milestone
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| closedAt     | Date     | &check;      |
| closedIssues | Long     | &check;      |
| createdAt    | Date     | &check;      |
| creator      | User     | &check;      |
| description  | String   | &check;      |
| dueOn        | Date     | &check;      |
| id           | Long     | &cross;      |
| nodeId       | String   | &cross;      |
| number       | Long     | &cross;      |
| openIssues   | Long     | &check;      |
| state        | String   | &check;      |
| title        | String   | &check;      |
| updatedAt    | Date     | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &cross;      |
| login    | String   | &cross;      |

#### Owner
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &cross;      |
| login     | String   | &cross;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |

#### Repository
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &cross;      |
| name     | String   | &cross;      |

#### User
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &check;      |
| login     | String   | &check;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |
