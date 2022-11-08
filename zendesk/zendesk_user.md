---
description: Zendesk User
---
zendesk_user
------------

| **Name**                | **Type**           | **Nullable** |
| ----------------------- | ------------------ | ------------ |
| account                 | String             | &check;      |
| active                  | Boolean            | &check;      |
| alias                   | String             | &check;      |
| created_at              | String             | &check;      |
| custom_role_id          | Long               | &check;      |
| default_group_id        | Long               | &check;      |
| details                 | String             | &check;      |
| email                   | String             | &check;      |
| external_id             | String             | &check;      |
| groups                  | List<String>       | &check;      |
| iana_time_zone          | String             | &check;      |
| id                      | String             | &cross;      |
| last_login_at           | String             | &check;      |
| locale                  | String             | &check;      |
| locale_id               | String             | &check;      |
| moderator               | Boolean            | &check;      |
| name                    | String             | &check;      |
| notes                   | String             | &check;      |
| only_private_comments   | Boolean            | &check;      |
| organization_id         | Long               | &check;      |
| organizations           | List<String>       | &check;      |
| phone                   | String             | &check;      |
| photo                   | Photo              | &check;      |
| report_csv              | Boolean            | &check;      |
| restricted_agent        | Boolean            | &check;      |
| role                    | String             | &check;      |
| role_type               | String             | &check;      |
| shared                  | Boolean            | &check;      |
| shared_agent            | Boolean            | &check;      |
| shared_phone_number     | Boolean            | &check;      |
| signature               | String             | &check;      |
| suspended               | Boolean            | &check;      |
| tags                    | List<String>       | &check;      |
| ticket_restriction      | String             | &check;      |
| time_zone               | String             | &check;      |
| two_factor_auth_enabled | Boolean            | &check;      |
| updated_at              | String             | &check;      |
| url                     | String             | &check;      |
| user_fields             | Map<String,String> | &check;      |
| verified                | Boolean            | &check;      |

#### Photo
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| content_type       | String   | &check;      |
| content_url        | String   | &check;      |
| deleted            | Boolean  | &check;      |
| file_name          | String   | &check;      |
| height             | Int      | &check;      |
| id                 | Long     | &check;      |
| inline             | Boolean  | &check;      |
| mapped_content_url | String   | &check;      |
| size               | Int      | &check;      |
| url                | String   | &check;      |
| width              | Int      | &check;      |
