---
description: Fastly Account
---
fastly_account
--------------

| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| billing_contact_id        | String   | &check;      |
| billing_network_type      | String   | &check;      |
| billing_ref               | String   | &check;      |
| can_configure_wordpress   | Boolean  | &check;      |
| can_request_io            | Boolean  | &check;      |
| can_reset_passwords       | Boolean  | &check;      |
| can_upload_vcl            | Boolean  | &check;      |
| created_at                | String   | &check;      |
| deleted_at                | String   | &check;      |
| force_2fa                 | Boolean  | &check;      |
| force_sso                 | Boolean  | &check;      |
| has_account_panel         | Boolean  | &check;      |
| has_api_key               | Boolean  | &check;      |
| has_improved_events       | Boolean  | &check;      |
| has_improved_ssl_config   | Boolean  | &check;      |
| has_openstack_logging     | Boolean  | &check;      |
| has_pci                   | Boolean  | &check;      |
| has_pci_passwords         | Boolean  | &check;      |
| id                        | String   | &cross;      |
| ip_whitelist              | String   | &check;      |
| legal_contact_id          | String   | &check;      |
| logentries_provisioned_by | String   | &check;      |
| max_tokens_per_user       | Int      | &check;      |
| name                      | String   | &cross;      |
| owner_id                  | String   | &check;      |
| phone_number              | String   | &check;      |
| postal_address            | String   | &check;      |
| pricing_plan              | String   | &check;      |
| pricing_plan_id           | String   | &check;      |
| rate_limit                | Int      | &check;      |
| readonly                  | Boolean  | &check;      |
| requires_support_email    | Boolean  | &check;      |
| san_domains               | Int      | &check;      |
| security_contact_id       | String   | &check;      |
| technical_contact_id      | String   | &check;      |
| updated_at                | String   | &check;      |
