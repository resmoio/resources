---
description: CrowdStrike Device Control Policy
---
crowdstrike_device_control_policy
---------------------------------

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
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| classes                | JSON     | &check;      |
| end_user_notification  | String   | &check;      |
| enforcement_mode       | String   | &check;      |
| enhanced_file_metadata | String   | &check;      |
