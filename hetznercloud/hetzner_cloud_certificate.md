---
description: Hetzner Cloud Certificate
---
hetzner_cloud_certificate
-------------------------

| **Name**         | **Type**           | **Nullable** |
| ---------------- | ------------------ | ------------ |
| created          | String             | &check;      |
| domain_names     | List<String>       | &check;      |
| fingerprint      | String             | &check;      |
| id               | Long               | &cross;      |
| labels           | Map<String,String> | &check;      |
| name             | String             | &check;      |
| not_valid_after  | String             | &check;      |
| not_valid_before | String             | &check;      |
| status           | String             | &check;      |
| type             | String             | &check;      |
| used_by          | List<Map>          | &check;      |
