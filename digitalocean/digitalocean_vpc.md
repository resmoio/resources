---
description: DigitalOcean VPC
---
digitalocean_vpc
----------------

| **Name**    | **Type**        | **Nullable** |
| ----------- | --------------- | ------------ |
| created_at  | String          | &check;      |
| default     | Boolean         | &check;      |
| description | String          | &check;      |
| id          | String          | &cross;      |
| ip_range    | String          | &check;      |
| members     | List<VpcMember> | &check;      |
| name        | String          | &check;      |
| region      | String          | &check;      |
| urn         | String          | &check;      |

#### VpcMember
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| created_at | String   | &check;      |
| name       | String   | &check;      |
| urn        | String   | &check;      |
