---
description: PipeDrive User
---
pipedrive_user
--------------

| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| access            | List<Access> | &check;      |
| activated         | Boolean      | &check;      |
| activeFlag        | Boolean      | &check;      |
| created           | String       | &check;      |
| defaultCurrency   | String       | &check;      |
| email             | String       | &check;      |
| hasCreatedCompany | Boolean      | &check;      |
| id                | Long         | &cross;      |
| isYou             | Boolean      | &check;      |
| lang              | Int          | &check;      |
| lastLogin         | String       | &check;      |
| locale            | String       | &check;      |
| modified          | String       | &check;      |
| name              | String       | &check;      |
| phone             | String       | &check;      |
| roleId            | Int          | &check;      |
| roleIds           | List<Long>   | &check;      |
| timezoneName      | String       | &check;      |
| timezoneOffset    | String       | &check;      |

#### Access
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| admin           | Boolean  | &check;      |
| app             | String   | &check;      |
| permissionSetId | String   | &check;      |
