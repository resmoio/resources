---
description: Tailscale Access Control List
---
tailscale_access_control_list
-----------------------------

| **Name** | **Type**           | **Nullable** |
| -------- | ------------------ | ------------ |
| acls     | List<ACL>          | &check;      |
| groups   | Map<String,List>   | &check;      |
| hosts    | Map<String,String> | &check;      |

#### ACL
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| action   | String       | &cross;      |
| ports    | List<String> | &check;      |
| users    | List<String> | &check;      |
