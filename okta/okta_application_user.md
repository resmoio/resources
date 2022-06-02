---
description: Okta Application User
---
okta_application_user
---------------------

| **Name**        | **Type**    | **Nullable** |
| --------------- | ----------- | ------------ |
| appId           | String      | &cross;      |
| created         | String      | &check;      |
| credentials     | Credentials | &check;      |
| externalId      | String      | &check;      |
| id              | String      | &cross;      |
| lastSync        | String      | &check;      |
| lastUpdated     | String      | &check;      |
| passwordChanged | String      | &check;      |
| profile         | JSON        | &check;      |
| scope           | String      | &check;      |
| status          | String      | &check;      |
| statusChanged   | String      | &check;      |
| syncState       | String      | &check;      |

#### Credentials
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| username | String   | &check;      |
