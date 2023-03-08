---
description: DigitalOcean Database Cluster
---
digitalocean_database_cluster
-----------------------------

| **Name**                    | **Type**           | **Nullable** |
| --------------------------- | ------------------ | ------------ |
| connection                  | Connection         | &check;      |
| created_at                  | String             | &check;      |
| db_names                    | List<String>       | &check;      |
| engine                      | String             | &check;      |
| id                          | String             | &cross;      |
| maintenance_window          | MaintenanceWindow  | &check;      |
| name                        | String             | &check;      |
| num_nodes                   | Int                | &check;      |
| private_connection          | Connection         | &check;      |
| private_network_uuid        | String             | &check;      |
| project_id                  | String             | &check;      |
| region                      | String             | &check;      |
| rules                       | List<FirewallRule> | &check;      |
| size                        | String             | &check;      |
| status                      | String             | &check;      |
| tags                        | List<String>       | &check;      |
| users                       | List<User>         | &check;      |
| version                     | String             | &check;      |
| version_end_of_availability | String             | &check;      |
| version_end_of_life         | String             | &check;      |

#### Connection
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| database | String   | &check;      |
| host     | String   | &check;      |
| port     | String   | &check;      |
| ssl      | String   | &check;      |
| uri      | String   | &check;      |
| user     | String   | &check;      |

#### FirewallRule
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| cluster_uuid | String   | &check;      |
| created_at   | String   | &check;      |
| uuid         | String   | &check;      |
| value        | String   | &check;      |

#### MaintenanceWindow
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| day         | String   | &check;      |
| description | String   | &check;      |
| hour        | String   | &check;      |
| pending     | Boolean  | &check;      |

#### User
| **Name**      | **Type**      | **Nullable** |
| ------------- | ------------- | ------------ |
| mysql_settins | User.Settings | &check;      |
| name          | String        | &check;      |
| role          | String        | &check;      |

#### User.Settings
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| auth_plugin | String   | &check;      |
