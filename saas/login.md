---
description: SaaS Browser Login
---
login
-----

| **Name**           | **Type**         | **Nullable** |
| ------------------ | ---------------- | ------------ |
| appName            | String           | &cross;      |
| browserId          | String           | &cross;      |
| deletedAt          | String           | &check;      |
| email              | String           | &cross;      |
| firstLogin         | String           | &check;      |
| identifier         | String           | &cross;      |
| lastLogin          | String           | &cross;      |
| passwordSharedWith | List<SharedInfo> | &check;      |
| passwordStrength   | String           | &check;      |
| permission         | List<String>     | &check;      |
| ssoProvider        | String           | &check;      |
| status             | String           | &cross;      |
| type               | String           | &cross;      |
| url                | String           | &cross;      |

#### SharedInfo
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| appName    | String   | &cross;      |
| identifier | String   | &cross;      |
