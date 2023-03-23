---
description: CrowdStrike Response Policy
---
crowdstrike_response_policy
---------------------------

| **Name**           | **Type**       | **Nullable** |
| ------------------ | -------------- | ------------ |
| cid                | String         | &check;      |
| created_by         | String         | &check;      |
| created_timestamp  | String         | &check;      |
| description        | String         | &check;      |
| enabled            | Boolean        | &check;      |
| groups             | List<Group>    | &check;      |
| id                 | String         | &cross;      |
| modified_by        | String         | &check;      |
| modified_timestamp | String         | &check;      |
| name               | String         | &check;      |
| platform_name      | String         | &check;      |
| settings           | List<Settings> | &check;      |

#### Group
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |

#### Settings
| **Name** | **Type**                      | **Nullable** |
| -------- | ----------------------------- | ------------ |
| name     | String                        | &cross;      |
| settings | List<Settings.SettingsDetail> | &cross;      |

#### Settings.SettingsDetail
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| id          | String   | &check;      |
| name        | String   | &check;      |
| type        | String   | &check;      |
| value       | JSON     | &check;      |
