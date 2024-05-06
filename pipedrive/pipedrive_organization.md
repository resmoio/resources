---
description: PipeDrive Organization
---
pipedrive_organization
----------------------

| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| activeFlag              | Boolean  | &check;      |
| activitiesCount         | Int      | &check;      |
| addTime                 | String   | &check;      |
| address                 | String   | &check;      |
| addressAdminAreaLevel1  | String   | &check;      |
| addressAdminAreaLevel2  | String   | &check;      |
| addressCountry          | String   | &check;      |
| addressFormattedAddress | String   | &check;      |
| addressPostalCode       | String   | &check;      |
| addressRoute            | String   | &check;      |
| addressStreetNumber     | String   | &check;      |
| addressSublocality      | String   | &check;      |
| addressSubpremise       | String   | &check;      |
| ccEmail                 | String   | &check;      |
| closedDealsCount        | Int      | &check;      |
| companyId               | Long     | &check;      |
| countryCode             | String   | &check;      |
| doneActivitiesCount     | Int      | &check;      |
| emailMessagesCount      | Int      | &check;      |
| filesCount              | Int      | &check;      |
| followersCount          | Int      | &check;      |
| id                      | Long     | &cross;      |
| label                   | Int      | &check;      |
| lastActivityDate        | String   | &check;      |
| lastActivityId          | Long     | &check;      |
| name                    | String   | &check;      |
| nextActivityDate        | String   | &check;      |
| nextActivityId          | Long     | &check;      |
| nextActivityTime        | String   | &check;      |
| notesCount              | Int      | &check;      |
| openDealsCount          | Int      | &check;      |
| owner                   | Owner    | &check;      |
| ownerName               | String   | &check;      |
| peopleCount             | Int      | &check;      |
| relatedClosedDealsCount | Int      | &check;      |
| relatedLostDealsCount   | Int      | &check;      |
| relatedOpenDealsCount   | Int      | &check;      |
| undoneActivitiesCount   | Int      | &check;      |
| updateTime              | String   | &check;      |
| visibleTo               | String   | &check;      |
| wonDealsCount           | Int      | &check;      |

#### Owner
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| activeFlag | Boolean  | &check;      |
| email      | String   | &check;      |
| id         | Long     | &check;      |
| name       | String   | &check;      |
| value      | Int      | &check;      |
