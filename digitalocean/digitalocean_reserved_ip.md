---
description: DigitalOcean Reserved IP
---
digitalocean_reserved_ip
------------------------

| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| droplet    | Droplet  | &check;      |
| ip         | String   | &cross;      |
| locked     | Boolean  | &check;      |
| project_id | String   | &check;      |
| region     | Region   | &check;      |

#### Droplet
| **Name**           | **Type**             | **Nullable** |
| ------------------ | -------------------- | ------------ |
| backup_ids         | List<Int>            | &check;      |
| created_at         | String               | &check;      |
| disk               | Long                 | &check;      |
| features           | List<String>         | &check;      |
| id                 | String               | &check;      |
| image              | Droplet.Image        | &check;      |
| locked             | Boolean              | &check;      |
| memory             | Long                 | &check;      |
| name               | String               | &check;      |
| networks           | Droplet.Network      | &check;      |
| next_backup_window | Droplet.BackupWindow | &check;      |
| region             | Droplet.Region       | &check;      |
| snapshot_ids       | List<String>         | &check;      |
| status             | String               | &check;      |
| tags               | List<String>         | &check;      |
| vcpus              | Long                 | &check;      |
| volume_ids         | List<String>         | &check;      |
| vpc_uuid           | String               | &check;      |

#### Droplet.BackupWindow
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| end      | String   | &check;      |
| start    | String   | &check;      |

#### Droplet.Image
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

#### Droplet.Network
| **Name** | **Type**                  | **Nullable** |
| -------- | ------------------------- | ------------ |
| v4       | List<Droplet.NetworkInfo> | &check;      |
| v6       | List<Droplet.NetworkInfo> | &check;      |

#### Droplet.NetworkInfo
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| gateway    | String   | &check;      |
| ip_address | String   | &check;      |
| netmask    | String   | &check;      |
| type       | String   | &check;      |

#### Droplet.Region
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| available | String       | &check;      |
| features  | List<String> | &check;      |
| name      | String       | &check;      |
| sizes     | List<String> | &check;      |
| slug      | String       | &check;      |

#### Region
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| available | Boolean      | &check;      |
| features  | List<String> | &check;      |
| name      | String       | &check;      |
| sizes     | List<String> | &check;      |
| slug      | String       | &check;      |
