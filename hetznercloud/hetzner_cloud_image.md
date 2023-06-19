---
description: Hetzner Cloud Image
---
hetzner_cloud_image
-------------------

| **Name**     | **Type**           | **Nullable** |
| ------------ | ------------------ | ------------ |
| architecture | String             | &check;      |
| bound_to     | String             | &check;      |
| created      | String             | &check;      |
| created_from | CreatedFrom        | &check;      |
| deleted      | String             | &check;      |
| deprecated   | String             | &check;      |
| description  | String             | &check;      |
| disk_size    | Long               | &check;      |
| id           | Long               | &cross;      |
| image_size   | Double             | &check;      |
| labels       | Map<String,String> | &check;      |
| name         | String             | &check;      |
| os_flavor    | String             | &check;      |
| os_version   | String             | &check;      |
| protection   | Protection         | &check;      |
| rapid_deploy | Boolean            | &check;      |
| status       | String             | &check;      |
| type         | String             | &check;      |

#### CreatedFrom
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &check;      |
| name     | String   | &check;      |

#### Protection
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| delete   | Boolean  | &check;      |
