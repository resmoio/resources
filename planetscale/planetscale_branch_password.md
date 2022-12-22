---
description: PlanetScale Branch Password
---
planetscale_branch_password
---------------------------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| access_host_url    | String             | &check;      |
| actor              | Actor              | &check;      |
| connection_strings | Map<String,String> | &check;      |
| created_at         | String             | &check;      |
| database_branch    | DatabaseBranch     | &check;      |
| deleted_at         | String             | &check;      |
| display_name       | String             | &check;      |
| expires_at         | String             | &check;      |
| id                 | String             | &cross;      |
| integrations       | List<Integration>  | &check;      |
| region             | Region             | &check;      |
| renewable          | Boolean            | &check;      |
| role               | String             | &check;      |
| ttl_seconds        | String             | &check;      |
| username           | String             | &check;      |

#### Actor
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| display_name | String   | &check;      |
| id           | String   | &check;      |

#### DatabaseBranch
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| access_host_url | String   | &check;      |
| id              | String   | &check;      |
| name            | String   | &check;      |
| production      | Boolean  | &check;      |

#### Integration
| **Name** | **Type**           | **Nullable** |
| -------- | ------------------ | ------------ |
| content  | Map<String,String> | &check;      |
| name     | String             | &check;      |
| type     | String             | &check;      |

#### Region
| **Name**            | **Type**     | **Nullable** |
| ------------------- | ------------ | ------------ |
| display_name        | String       | &check;      |
| enabled             | String       | &check;      |
| id                  | String       | &check;      |
| location            | String       | &check;      |
| provider            | String       | &check;      |
| public_ip_addresses | List<String> | &check;      |
| slug                | String       | &check;      |
