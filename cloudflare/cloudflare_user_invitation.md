---
description: Cloudflare User Invitation
---
cloudflare_user_invitation
--------------------------

| **Name**                            | **Type**     | **Nullable** |
| ----------------------------------- | ------------ | ------------ |
| expires_on                          | String       | &check;      |
| id                                  | String       | &cross;      |
| invited_by                          | String       | &check;      |
| invited_member_email                | String       | &check;      |
| invited_member_id                   | String       | &check;      |
| invited_on                          | String       | &check;      |
| organization_id                     | String       | &check;      |
| organization_is_enforcing_twofactor | Boolean      | &cross;      |
| organization_name                   | String       | &check;      |
| roles                               | List<String> | &check;      |
| status                              | String       | &check;      |
