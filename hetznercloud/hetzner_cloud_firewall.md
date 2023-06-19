---
description: Hetzner Cloud Firewall
---
hetzner_cloud_firewall
----------------------

| **Name**   | **Type**           | **Nullable** |
| ---------- | ------------------ | ------------ |
| applied_to | AppliedTo          | &check;      |
| created    | String             | &check;      |
| id         | Long               | &check;      |
| labels     | Map<String,String> | &check;      |
| name       | String             | &check;      |
| rules      | List<Rule>         | &check;      |

#### AppliedTo
| **Name**             | **Type**                 | **Nullable** |
| -------------------- | ------------------------ | ------------ |
| applied_to_resources | List<AppliedTo.Resource> | &check;      |
| label_selector       | Map<String,String>       | &check;      |
| server               | Map<String,Long>         | &check;      |
| type                 | String                   | &check;      |

#### AppliedTo.Resource
| **Name** | **Type**         | **Nullable** |
| -------- | ---------------- | ------------ |
| server   | Map<String,Long> | &check;      |
| type     | String           | &check;      |

#### Rule
| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| description     | String       | &check;      |
| destination_ips | List<String> | &check;      |
| direction       | String       | &check;      |
| port            | String       | &check;      |
| protocol        | String       | &check;      |
| source_ips      | List<String> | &check;      |
