---
description: Duo Integration
---
duo_integration
---------------

| **Name**                      | **Type**     | **Nullable** |
| ----------------------------- | ------------ | ------------ |
| adminapi_admins               | Int          | &check;      |
| adminapi_info                 | Int          | &check;      |
| adminapi_integrations         | Int          | &check;      |
| adminapi_read_log             | Int          | &check;      |
| adminapi_read_resource        | Int          | &check;      |
| adminapi_settings             | Int          | &check;      |
| adminapi_write_resource       | Int          | &check;      |
| enroll_policy                 | String       | &check;      |
| frameless_auth_prompt_enabled | Int          | &check;      |
| groups_allowed                | List<String> | &check;      |
| integrationKey                | String       | &cross;      |
| ip_whitelist                  | List<String> | &check;      |
| ip_whitelist_enroll_policy    | String       | &check;      |
| missing_web_referer_policy    | String       | &check;      |
| name                          | String       | &check;      |
| notes                         | String       | &check;      |
| self_service_allowed          | Boolean      | &check;      |
| trusted_device_days           | Int          | &check;      |
| type                          | String       | &cross;      |
| username_normalization_policy | String       | &check;      |
| web_referers_enabled          | Int          | &check;      |
