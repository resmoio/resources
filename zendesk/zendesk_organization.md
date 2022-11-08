---
description: Zendesk Organization
---
zendesk_organization
--------------------

| **Name**            | **Type**           | **Nullable** |
| ------------------- | ------------------ | ------------ |
| account             | String             | &check;      |
| created_at          | String             | &check;      |
| details             | String             | &check;      |
| domain_names        | List<String>       | &check;      |
| external_id         | String             | &check;      |
| group_id            | String             | &check;      |
| id                  | String             | &cross;      |
| name                | String             | &check;      |
| notes               | String             | &check;      |
| organization_fields | Map<String,String> | &check;      |
| shared_comments     | Boolean            | &check;      |
| shared_tickets      | Boolean            | &check;      |
| tags                | List<String>       | &check;      |
| updated_at          | String             | &check;      |
| url                 | String             | &check;      |
