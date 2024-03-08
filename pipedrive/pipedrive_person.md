---
description: PipeDrive Person
---
pipedrive_person
----------------

| **Name**                    | **Type**     | **Nullable** |
| --------------------------- | ------------ | ------------ |
| activeFlag                  | Boolean      | &check;      |
| activitiesCount             | Int          | &check;      |
| addTime                     | String       | &check;      |
| ccEmail                     | String       | &check;      |
| companyId                   | Long         | &check;      |
| doneActivitiesCount         | Int          | &check;      |
| email                       | Email        | &check;      |
| emailsMessagesCount         | Int          | &check;      |
| filesCount                  | Int          | &check;      |
| firstName                   | String       | &check;      |
| followersCount              | Int          | &check;      |
| id                          | Long         | &cross;      |
| label                       | Int          | &check;      |
| lastActivityDate            | String       | &check;      |
| lastActivityId              | String       | &check;      |
| lastIncomingMailTime        | String       | &check;      |
| lastName                    | String       | &check;      |
| lastOutgoingMailTime        | String       | &check;      |
| lostDealsCount              | Int          | &check;      |
| marketingStatus             | String       | &check;      |
| name                        | String       | &check;      |
| nextActivityDate            | String       | &check;      |
| nextActivityId              | String       | &check;      |
| nextActivityTime            | String       | &check;      |
| notesCount                  | Int          | &check;      |
| openDealsCount              | Int          | &check;      |
| orgName                     | String       | &check;      |
| organization                | Organization | &check;      |
| owner                       | Owner        | &check;      |
| ownerName                   | String       | &check;      |
| participantClosedDealsCount | Int          | &check;      |
| participantOpenDealsCount   | Int          | &check;      |
| phone                       | Phone        | &check;      |
| primaryEmail                | String       | &check;      |
| relatedLostDealsCount       | Int          | &check;      |
| relatedOpenDealsCount       | Int          | &check;      |
| relatedWonDealsCount        | Int          | &check;      |
| undoneActivitiesCount       | Int          | &check;      |
| updateTime                  | String       | &check;      |
| visibleTo                   | String       | &check;      |
| wonDealsCount               | Int          | &check;      |

#### Email
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| label    | String   | &check;      |
| primary  | Boolean  | &check;      |
| value    | Long     | &check;      |

#### Organization
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| activeFlag  | Boolean  | &check;      |
| address     | String   | &check;      |
| ccEmail     | String   | &check;      |
| name        | String   | &check;      |
| ownerId     | Long     | &check;      |
| peopleCount | Int      | &check;      |
| value       | Long     | &check;      |

#### Owner
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| activeFlag | Boolean  | &check;      |
| email      | String   | &check;      |
| id         | Long     | &check;      |
| name       | String   | &check;      |
| value      | Long     | &check;      |

#### Phone
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| label    | String   | &check;      |
| primary  | Boolean  | &check;      |
| value    | Long     | &check;      |
