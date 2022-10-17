---
description: Qualys User
---
qualys_user
-----------

| **Name**         | **Type**         | **Nullable** |
| ---------------- | ---------------- | ------------ |
| business_unit    | String           | &check;      |
| contact_info     | ContactInfo      | &check;      |
| creation_date    | String           | &check;      |
| last_login_date  | String           | &check;      |
| manager_poc      | String           | &check;      |
| notifications    | NotificationInfo | &cross;      |
| permissions      | PermissionInfo   | &check;      |
| unit_manager_poc | String           | &check;      |
| user_id          | String           | &cross;      |
| user_login       | String           | &cross;      |
| user_role        | String           | &check;      |
| user_status      | String           | &check;      |

#### ContactInfo
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| address1       | String   | &check;      |
| address2       | String   | &check;      |
| city           | String   | &check;      |
| company        | String   | &check;      |
| country        | String   | &check;      |
| email          | String   | &check;      |
| fax            | String   | &check;      |
| firstname      | String   | &check;      |
| lastname       | String   | &check;      |
| phone          | String   | &check;      |
| state          | String   | &check;      |
| time_zone_code | String   | &check;      |
| title          | String   | &check;      |
| zip_code       | String   | &check;      |

#### NotificationInfo
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| daily_tickets | String   | &check;      |
| latest_vuln   | String   | &check;      |
| map           | String   | &check;      |
| scan          | String   | &check;      |

#### PermissionInfo
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| add_assets              | String   | &check;      |
| create_option_profiles  | String   | &check;      |
| edit_auth_records       | String   | &check;      |
| edit_remediation_policy | String   | &check;      |
| purge_info              | String   | &check;      |
