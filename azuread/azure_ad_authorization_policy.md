---
description: Azure Active Directory Authorization Policy
---
azure_ad_authorization_policy
-----------------------------

| **Name**                                  | **Type**                   | **Nullable** |
| ----------------------------------------- | -------------------------- | ------------ |
| allowEmailVerifiedUsersToJoinOrganization | Boolean                    | &check;      |
| allowInvitesFrom                          | String                     | &check;      |
| allowedToSignUpEmailBasedSubscriptions    | Boolean                    | &check;      |
| allowedToUseSSPR                          | Boolean                    | &check;      |
| blockMsolPowerShell                       | Boolean                    | &check;      |
| defaultUserRolePermissions                | DefaultUserRolePermissions | &check;      |
| description                               | String                     | &check;      |
| displayName                               | String                     | &check;      |
| guestUserRoleId                           | String                     | &check;      |
| id                                        | String                     | &cross;      |
| oDataType                                 | String                     | &check;      |

#### DefaultUserRolePermissions
| **Name**                        | **Type**     | **Nullable** |
| ------------------------------- | ------------ | ------------ |
| allowedToCreateApps             | Boolean      | &check;      |
| allowedToCreateSecurityGroups   | Boolean      | &check;      |
| allowedToReadOtherUsers         | Boolean      | &check;      |
| oDataType                       | String       | &check;      |
| permissionGrantPoliciesAssigned | List<String> | &check;      |
