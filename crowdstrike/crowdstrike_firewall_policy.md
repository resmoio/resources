---
description: CrowdStrike Firewall Policy
---
crowdstrike_firewall_policy
---------------------------

| **Name**           | **Type**    | **Nullable** |
| ------------------ | ----------- | ------------ |
| channel_version    | Boolean     | &check;      |
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
| rule_set_id        | String      | &check;      |

#### Group
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
