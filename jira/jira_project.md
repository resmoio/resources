---
description: JIRA Project
---
jira_project
------------

| **Name**          | **Type**         | **Nullable** |
| ----------------- | ---------------- | ------------ |
| archived          | Boolean          | &check;      |
| archivedBy        | String           | &check;      |
| archivedDate      | String           | &check;      |
| assigneeType      | String           | &check;      |
| components        | List<Component>  | &check;      |
| deleted           | Boolean          | &check;      |
| deletedBy         | String           | &check;      |
| deletedDate       | String           | &check;      |
| description       | String           | &check;      |
| favourite         | Boolean          | &check;      |
| id                | Int              | &cross;      |
| insight           | Insight          | &check;      |
| isPrivate         | Boolean          | &check;      |
| issueTypes        | List<IssueType>  | &check;      |
| key               | String           | &check;      |
| lead              | String           | &check;      |
| name              | String           | &check;      |
| permissionScheme  | PermissionScheme | &check;      |
| projectCategory   | Category         | &check;      |
| projectKeys       | List<String>     | &check;      |
| projectTypeKey    | String           | &check;      |
| retentionTillDate | String           | &check;      |
| roles             | List<String>     | &check;      |
| simplified        | Boolean          | &check;      |
| site              | String           | &cross;      |
| style             | String           | &check;      |
| uuid              | String           | &check;      |
| versions          | List<Version>    | &check;      |

#### Category
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| id          | Int      | &check;      |
| name        | String   | &check;      |

#### Component
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| assignee            | String   | &check;      |
| assigneeType        | String   | &check;      |
| description         | String   | &check;      |
| id                  | Int      | &check;      |
| isAssigneeTypeValid | Boolean  | &check;      |
| lead                | String   | &check;      |
| name                | String   | &check;      |
| realAssignee        | String   | &check;      |
| realAssigneeType    | String   | &check;      |

#### Insight
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| lastIssueUpdateTime | String   | &check;      |
| totalIssueCount     | Int      | &check;      |

#### IssueType
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| description    | String   | &check;      |
| hierarchyLevel | Int      | &check;      |
| id             | Int      | &check;      |
| name           | String   | &check;      |
| subtask        | Boolean  | &check;      |

#### PermissionScheme
| **Name**    | **Type**                          | **Nullable** |
| ----------- | --------------------------------- | ------------ |
| description | String                            | &check;      |
| id          | Int                               | &check;      |
| name        | String                            | &check;      |
| permissions | List<PermissionScheme.Permission> | &check;      |
| scope       | String                            | &check;      |

#### PermissionScheme.Permission
| **Name**   | **Type**                           | **Nullable** |
| ---------- | ---------------------------------- | ------------ |
| holder     | PermissionScheme.Permission.Holder | &check;      |
| id         | String                             | &check;      |
| permission | String                             | &check;      |

#### PermissionScheme.Permission.BasicUser
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| accountId    | String   | &check;      |
| accountType  | String   | &check;      |
| active       | Boolean  | &check;      |
| displayName  | String   | &check;      |
| emailAddress | String   | &check;      |

#### PermissionScheme.Permission.Holder
| **Name**    | **Type**                                | **Nullable** |
| ----------- | --------------------------------------- | ------------ |
| group       | String                                  | &check;      |
| parameter   | String                                  | &check;      |
| projectRole | PermissionScheme.Permission.ProjectRole | &check;      |
| type        | String                                  | &check;      |
| user        | PermissionScheme.Permission.BasicUser   | &check;      |

#### PermissionScheme.Permission.ProjectRole
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| id          | String   | &check;      |
| name        | String   | &check;      |

#### Version
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| archived        | Boolean  | &check;      |
| description     | String   | &check;      |
| id              | String   | &check;      |
| name            | String   | &check;      |
| releaseDate     | String   | &check;      |
| released        | Boolean  | &check;      |
| userReleaseDate | String   | &check;      |
