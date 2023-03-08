---
description: DigitalOcean Volume
---
digitalocean_volume
-------------------

| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| created_at       | String       | &check;      |
| description      | String       | &check;      |
| droplet_ids      | List<Int>    | &check;      |
| filesystem_label | String       | &check;      |
| filesystem_type  | String       | &check;      |
| id               | String       | &cross;      |
| name             | String       | &check;      |
| region           | Region       | &check;      |
| size_gigabytes   | Long         | &check;      |
| tags             | List<String> | &check;      |

#### Region
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| available | Boolean      | &check;      |
| features  | List<String> | &check;      |
| name      | String       | &check;      |
| sizes     | List<String> | &check;      |
| slug      | String       | &check;      |
