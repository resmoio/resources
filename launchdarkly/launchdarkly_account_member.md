---
description: LaunchDarkly Account Member
---
launchdarkly_account_member
---------------------------

| **Name**           | **Type**              | **Nullable** |
| ------------------ | --------------------- | ------------ |
| _id                | String                | &cross;      |
| _lastSeen          | Long                  | &check;      |
| _pendingEmail      | String                | &check;      |
| _pendingInvite     | Boolean               | &check;      |
| _verified          | Boolean               | &check;      |
| creationDate       | Long                  | &check;      |
| customRoles        | List<String>          | &check;      |
| email              | String                | &check;      |
| excludedDashboards | List<String>          | &check;      |
| firstName          | String                | &check;      |
| lastName           | String                | &check;      |
| mfa                | String                | &check;      |
| oauthProviders     | List<String>          | &check;      |
| permissionGrants   | List<PermissionGrant> | &check;      |
| role               | String                | &check;      |
| teams              | List<Team>            | &check;      |

#### PermissionGrant
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| actionSet | String       | &check;      |
| actions   | List<String> | &check;      |
| resource  | String       | &check;      |

#### Team
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| customRoleKeys | List<String> | &check;      |
| key            | String       | &cross;      |
| name           | String       | &check;      |
