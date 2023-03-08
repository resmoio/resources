---
description: DigitalOcean Droplet
---
digitalocean_droplet
--------------------

| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| backup_ids         | List<Int>    | &check;      |
| created_at         | String       | &check;      |
| disk               | Long         | &check;      |
| features           | List<String> | &check;      |
| id                 | String       | &cross;      |
| image              | Image        | &check;      |
| locked             | Boolean      | &check;      |
| memory             | Long         | &check;      |
| name               | String       | &check;      |
| networks           | Network      | &check;      |
| next_backup_window | BackupWindow | &check;      |
| region             | Region       | &check;      |
| snapshot_ids       | List<String> | &check;      |
| status             | String       | &check;      |
| tags               | List<String> | &check;      |
| vcpus              | Long         | &check;      |
| volume_ids         | List<String> | &check;      |
| vpc_uuid           | String       | &check;      |

#### BackupWindow
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| end      | String   | &check;      |
| start    | String   | &check;      |

#### Image
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| created_at    | String       | &check;      |
| description   | String       | &check;      |
| distribution  | String       | &check;      |
| error_message | String       | &check;      |
| id            | String       | &check;      |
| min_disk_size | Long         | &check;      |
| name          | String       | &check;      |
| public        | Boolean      | &check;      |
| regions       | List<String> | &check;      |
| slug          | String       | &check;      |
| status        | String       | &check;      |
| tags          | List<String> | &check;      |
| type          | String       | &check;      |

#### Network
| **Name** | **Type**          | **Nullable** |
| -------- | ----------------- | ------------ |
| v4       | List<NetworkInfo> | &check;      |
| v6       | List<NetworkInfo> | &check;      |

#### NetworkInfo
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| gateway    | String   | &check;      |
| ip_address | String   | &check;      |
| netmask    | String   | &check;      |
| type       | String   | &check;      |

#### Region
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| available | String       | &check;      |
| features  | List<String> | &check;      |
| name      | String       | &check;      |
| sizes     | List<String> | &check;      |
| slug      | String       | &check;      |
