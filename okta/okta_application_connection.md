---
description: Okta Application Connection
---
okta_application_connection
---------------------------

| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| appId      | String   | &cross;      |
| authSchema | String   | &check;      |
| links      | Links    | &check;      |
| status     | String   | &check;      |

#### Links
| **Name**   | **Type**   | **Nullable** |
| ---------- | ---------- | ------------ |
| deactivate | Links.Link | &check;      |
| self       | Links.Link | &check;      |

#### Links.Link
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
