---
description: CrowdStrike Sensor Update Policy
---
crowdstrike_sensor_update_policy
--------------------------------

| **Name**           | **Type**    | **Nullable** |
| ------------------ | ----------- | ------------ |
| cid                | String      | &check;      |
| created_by         | String      | &check;      |
| created_timestamp  | String      | &check;      |
| description        | String      | &check;      |
| enabled            | Boolean     | &check;      |
| groups             | List<Group> | &check;      |
| id                 | String      | &cross;      |
| modified_by        | String      | &check;      |
| modified_timestamp | String      | &check;      |
| name               | String      | &check;      |
| platform_name      | String      | &check;      |
| settings           | Settings    | &check;      |

#### Group
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |

#### Settings
| **Name**                  | **Type**               | **Nullable** |
| ------------------------- | ---------------------- | ------------ |
| build                     | String                 | &check;      |
| scheduler                 | Settings.Scheduler     | &check;      |
| sensor_version            | String                 | &check;      |
| show_early_adapter_builds | Boolean                | &check;      |
| stage                     | String                 | &check;      |
| uninstall_protection      | String                 | &check;      |
| variants                  | List<Settings.Variant> | &check;      |

#### Settings.Scheduler
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| enabled   | Boolean  | &check;      |
| schedules | JSON     | &check;      |
| timezone  | String   | &check;      |

#### Settings.Variant
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| build          | String   | &check;      |
| platform       | String   | &check;      |
| sensor_version | String   | &check;      |
| stage          | String   | &check;      |
