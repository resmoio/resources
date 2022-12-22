---
description: PlanetScale Organization
---
planetscale_organization
------------------------

| **Name**                     | **Type**            | **Nullable** |
| ---------------------------- | ------------------- | ------------ |
| admin_only_production_access | Boolean             | &check;      |
| billing_email                | String              | &check;      |
| can_create_databases         | Boolean             | &check;      |
| created_at                   | String              | &check;      |
| database_count               | Int                 | &check;      |
| features                     | Map<String,Boolean> | &check;      |
| flags                        | Map<String,String>  | &check;      |
| free_databases_remaining     | Int                 | &check;      |
| has_past_due_invoices        | Boolean             | &check;      |
| id                           | String              | &cross;      |
| name                         | String              | &cross;      |
| plan                         | String              | &check;      |
| single_tenancy               | Boolean             | &check;      |
| sleeping_database_count      | Int                 | &check;      |
| sso                          | Boolean             | &check;      |
| sso_directory                | Boolean             | &check;      |
| sso_portal_url               | String              | &check;      |
| updated_at                   | String              | &check;      |
| valid_billing_info           | Boolean             | &check;      |
