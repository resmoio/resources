---
description: Cloudflare Zone DNS Record
---
cloudflare_zone_dnsrecord
-------------------------

| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| content    | String   | &check;      |
| created_on | String   | &check;      |
| id         | String   | &cross;      |
| locked     | Boolean  | &cross;      |
| meta       | Meta     | &check;      |
| name       | String   | &check;      |
| proxiable  | Boolean  | &cross;      |
| proxied    | Boolean  | &cross;      |
| ttl        | Number   | &check;      |
| type       | String   | &check;      |
| zone_id    | String   | &cross;      |
| zone_name  | String   | &check;      |

#### Meta
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| auto_added             | Boolean  | &check;      |
| managed_by_apps        | Boolean  | &check;      |
| managed_by_argo_tunnel | Boolean  | &check;      |
| source                 | String   | &check;      |
