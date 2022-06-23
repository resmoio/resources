---
description: Jamf Pro Account Group
---
jamf_account_group
------------------

| **Name**     | **Type**          | **Nullable** |
| ------------ | ----------------- | ------------ |
| accessLevel  | String            | &check;      |
| id           | Int               | &cross;      |
| members      | List<GroupMember> | &check;      |
| name         | String            | &check;      |
| privilegeSet | String            | &check;      |
| privileges   | Privileges        | &check;      |
| serverName   | String            | &cross;      |
| site         | Site              | &check;      |

#### GroupMember
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### Privileges
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| casperAdmin  | List<String> | &check;      |
| casperRemote | List<String> | &check;      |
| jssActions   | List<String> | &check;      |
| jssObjects   | List<String> | &check;      |
| jssSettings  | List<String> | &check;      |
| recon        | List<String> | &check;      |

#### Site
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |
