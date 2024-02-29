---
description: Jamf Pro User Group
---
jamf_user_group
---------------

| **Name**         | **Type**   | **Nullable** |
| ---------------- | ---------- | ------------ |
| id               | Int        | &cross;      |
| isNotifyOnChange | Boolean    | &check;      |
| isSmart          | Boolean    | &check;      |
| name             | String     | &check;      |
| serverName       | String     | &cross;      |
| site             | Site       | &check;      |
| users            | List<User> | &cross;      |

#### Site
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### User
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| email_address | String   | &check;      |
| full_name     | String   | &check;      |
| id            | Int      | &cross;      |
| phone_number  | String   | &check;      |
| username      | String   | &check;      |
