---
description: Linear Team
---
linear_team
-----------

| **Name**                      | **Type**     | **Nullable** |
| ----------------------------- | ------------ | ------------ |
| archivedAt                    | String       | &check;      |
| autoArchivePeriod             | Int          | &check;      |
| autoClosePeriod               | Int          | &check;      |
| autoCloseStateId              | String       | &check;      |
| createdAt                     | String       | &check;      |
| cycleCalenderUrl              | String       | &check;      |
| cycleCooldownTime             | Int          | &check;      |
| cycleDuration                 | Int          | &check;      |
| cycleIssueAutoAssignCompleted | Boolean      | &check;      |
| cycleIssueAutoAssignStarted   | Boolean      | &check;      |
| cycleLockToActive             | Boolean      | &check;      |
| cycleStartDay                 | Int          | &check;      |
| cyclesEnabled                 | Boolean      | &check;      |
| defaultIssueEstimate          | Int          | &check;      |
| description                   | String       | &check;      |
| groupIssueHistory             | Boolean      | &check;      |
| id                            | String       | &cross;      |
| inviteHash                    | String       | &check;      |
| issueEstimationAllowZero      | Boolean      | &check;      |
| issueEstimationExtended       | Boolean      | &check;      |
| issueEstimationType           | String       | &check;      |
| issueOrderingNoPriorityFirst  | Boolean      | &check;      |
| issueSortOrderDefaultToBottom | Boolean      | &check;      |
| key                           | String       | &check;      |
| name                          | String       | &check;      |
| organization                  | Organization | &check;      |
| private                       | Boolean      | &check;      |
| slackIssueComments            | Boolean      | &check;      |
| slackIssueStatuses            | Boolean      | &check;      |
| slackNewIssue                 | Boolean      | &check;      |
| timezone                      | String       | &check;      |
| triageEnabled                 | Boolean      | &check;      |
| upcomingCycleCount            | Int          | &check;      |
| updatedAt                     | String       | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
