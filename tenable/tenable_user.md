---
description: Tenable.io User
---
tenable_user
------------

| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| container_uuid     | String       | &check;      |
| email              | String       | &check;      |
| enabled            | Boolean      | &check;      |
| group_uuids        | List<String> | &check;      |
| id                 | String       | &cross;      |
| last_login_attempt | String       | &check;      |
| lastlogin          | String       | &check;      |
| lockout            | Int          | &check;      |
| login_fail_count   | Int          | &check;      |
| login_fail_total   | Int          | &check;      |
| name               | String       | &check;      |
| permissions        | Int          | &check;      |
| preferences        | Preferences  | &check;      |
| two_factor         | TwoFactor    | &check;      |
| type               | String       | &check;      |
| undeletable        | Boolean      | &check;      |
| user_name          | String       | &check;      |
| username           | String       | &check;      |
| uuid               | String       | &cross;      |
| uuid_id            | String       | &cross;      |

#### Preferences
| **Name**                       | **Type** | **Nullable** |
| ------------------------------ | -------- | ------------ |
| enableAssetWorkbench           | String   | &check;      |
| enableExplore                  | String   | &check;      |
| enableUnifiedScanConfiguration | String   | &check;      |
| enableVMWorkbench              | String   | &check;      |
| enableWebAppWorkbench          | String   | &check;      |
| tenableGridState               | String   | &check;      |

#### TwoFactor
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| activated     | Date     | &check;      |
| email_enabled | Int      | &check;      |
| sms_enabled   | Int      | &check;      |
| sms_phone     | String   | &check;      |
| totp_enabled  | Int      | &check;      |
