---
description: Qualys Web App Finding
---
qualys_web_app_finding
----------------------

| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| findingType       | String   | &check;      |
| firstDetectedDate | String   | &check;      |
| id                | String   | &check;      |
| isIgnored         | Boolean  | &check;      |
| lastDetectedDate  | String   | &check;      |
| lastTestedDate    | String   | &check;      |
| name              | String   | &check;      |
| potential         | String   | &check;      |
| qid               | String   | &check;      |
| severity          | String   | &check;      |
| type              | String   | &check;      |
| uniqueId          | String   | &cross;      |
| webApp            | WebApp   | &check;      |

#### WebApp
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| url      | String   | &check;      |
