---
description: Linear Project
---
linear_project
--------------

| **Name**                            | **Type**           | **Nullable** |
| ----------------------------------- | ------------------ | ------------ |
| archivedAt                          | String             | &check;      |
| autoArchivedAt                      | String             | &check;      |
| canceledAt                          | String             | &check;      |
| completedAt                         | String             | &check;      |
| completedIssueCountHistory          | List<Double>       | &check;      |
| completedScopeHistory               | List<Double>       | &check;      |
| convertedFromIssue                  | ConvertedFromIssue | &check;      |
| createdAt                           | String             | &check;      |
| creator                             | Creator            | &check;      |
| description                         | String             | &check;      |
| id                                  | String             | &cross;      |
| inProgressScopeHistory              | List<Double>       | &check;      |
| issueCountHistory                   | List<Double>       | &check;      |
| lead                                | Lead               | &check;      |
| members                             | Members            | &check;      |
| name                                | String             | &check;      |
| progress                            | Int                | &check;      |
| projectUpdateRemindersPausedUntilAt | String             | &check;      |
| scope                               | Double             | &check;      |
| scopeHistory                        | List<Double>       | &check;      |
| slackIssueComments                  | Boolean            | &check;      |
| slackIssueStatuses                  | Boolean            | &check;      |
| slackNewIssue                       | Boolean            | &check;      |
| slugId                              | String             | &check;      |
| sortOrder                           | Double             | &check;      |
| startDate                           | String             | &check;      |
| startedAt                           | String             | &check;      |
| state                               | String             | &check;      |
| targetDate                          | String             | &check;      |
| teams                               | Teams              | &check;      |
| updatedAt                           | String             | &check;      |
| url                                 | String             | &check;      |

#### ConvertedFromIssue
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| title    | String   | &check;      |

#### Creator
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Lead
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Member
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Members
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| nodes    | List<Member> | &check;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Teams
| **Name** | **Type**   | **Nullable** |
| -------- | ---------- | ------------ |
| nodes    | List<Team> | &check;      |
