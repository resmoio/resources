---
description: Bitbucket Repository Webhook
---
bitbucket_repository_webhook
----------------------------

| **Name**               | **Type**     | **Nullable** |
| ---------------------- | ------------ | ------------ |
| active                 | Boolean      | &cross;      |
| created_at             | String       | &check;      |
| description            | String       | &check;      |
| events                 | List<String> | &check;      |
| history_enabled        | Boolean      | &cross;      |
| read_only              | String       | &check;      |
| repository_id          | String       | &cross;      |
| skip_cert_verification | Boolean      | &cross;      |
| source                 | String       | &check;      |
| subject                | Subject      | &check;      |
| type                   | String       | &check;      |
| url                    | String       | &check;      |
| uuid                   | String       | &cross;      |
| workspace_id           | String       | &cross;      |

#### Subject
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| full_name | String   | &check;      |
| name      | String   | &check;      |
| type      | String   | &check;      |
| uuid      | String   | &check;      |
