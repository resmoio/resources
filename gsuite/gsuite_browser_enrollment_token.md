---
description: Google Workspace Browser Enrollment Token
---
gsuite_browser_enrollment_token
-------------------------------

| **Name**         | **Type**   | **Nullable** |
| ---------------- | ---------- | ------------ |
| creationTime     | String     | &check;      |
| creatorId        | String     | &check;      |
| expiration       | Expiration | &check;      |
| orgUnitPath      | String     | &check;      |
| revokeTime       | String     | &check;      |
| revokerId        | String     | &check;      |
| state            | String     | &check;      |
| tokenPermanentId | String     | &cross;      |
| tokenType        | String     | &cross;      |

#### Expiration
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| expireTime | String   | &check;      |
| ttl        | Long     | &check;      |
