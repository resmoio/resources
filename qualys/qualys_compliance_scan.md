---
description: Qualys Compliance Scan
---
qualys_compliance_scan
----------------------

| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| duration        | String   | &check;      |
| id              | String   | &cross;      |
| launch_datetime | String   | &check;      |
| policy          | Policy   | &check;      |
| processed       | String   | &check;      |
| ref             | String   | &check;      |
| status          | Status   | &check;      |
| target          | String   | &check;      |
| title           | String   | &check;      |
| type            | String   | &check;      |
| user_login      | String   | &check;      |

#### Policy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| title    | String   | &check;      |

#### Status
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| state     | String   | &check;      |
| sub_state | String   | &check;      |
