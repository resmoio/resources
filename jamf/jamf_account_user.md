---
description: Jamf Pro Account User
---
jamf_account_user
-----------------

| **Name**            | **Type**   | **Nullable** |
| ------------------- | ---------- | ------------ |
| accessLevel         | String     | &check;      |
| directoryUser       | Boolean    | &check;      |
| email               | String     | &check;      |
| emailAddress        | String     | &check;      |
| enabled             | String     | &check;      |
| forcePasswordChange | Boolean    | &check;      |
| fullName            | String     | &check;      |
| id                  | Int        | &cross;      |
| name                | String     | &check;      |
| passwordSha256      | String     | &check;      |
| privilegeSet        | String     | &check;      |
| privileges          | Privileges | &check;      |
| serverName          | String     | &cross;      |

#### Privileges
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| casperAdmin  | List<String> | &check;      |
| casperRemote | List<String> | &check;      |
| jssActions   | List<String> | &check;      |
| jssObjects   | List<String> | &check;      |
| jssSettings  | List<String> | &check;      |
| recon        | List<String> | &check;      |
