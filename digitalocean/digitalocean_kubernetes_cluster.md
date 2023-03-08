---
description: DigitalOcean Kubernetes Cluster
---
digitalocean_kubernetes_cluster
-------------------------------

| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| auto_upgrade       | Boolean      | &check;      |
| cluster_subnet     | String       | &check;      |
| created_at         | String       | &check;      |
| endpoint           | String       | &check;      |
| ha                 | Boolean      | &check;      |
| id                 | String       | &cross;      |
| ipv4               | String       | &check;      |
| maintenance_policy | Policy       | &check;      |
| name               | String       | &check;      |
| node_pools         | JSON         | &check;      |
| region             | String       | &check;      |
| registry_enabled   | Boolean      | &check;      |
| service_subnet     | String       | &check;      |
| status             | Status       | &check;      |
| surge_upgrade      | Boolean      | &check;      |
| tags               | List<String> | &check;      |
| updated_at         | String       | &check;      |
| version            | String       | &check;      |
| vpc_uuid           | String       | &check;      |

#### Policy
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| day        | String   | &check;      |
| duration   | String   | &check;      |
| start_time | String   | &check;      |

#### Status
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| message  | String   | &check;      |
| state    | String   | &check;      |
