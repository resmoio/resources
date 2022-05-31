---
description: Slack User
---
slack_user
----------

| **Name**               | **Type**       | **Nullable** |
| ---------------------- | -------------- | ------------ |
| admin                  | Boolean        | &check;      |
| appUser                | Boolean        | &check;      |
| billingActive          | Boolean        | &check;      |
| bot                    | Boolean        | &check;      |
| color                  | String         | &check;      |
| deleted                | Boolean        | &check;      |
| emailConfirmed         | Boolean        | &check;      |
| enterpriseUser         | EnterpriseUser | &check;      |
| has2fa                 | Boolean        | &check;      |
| hasFiles               | Boolean        | &check;      |
| id                     | String         | &cross;      |
| invitedUser            | Boolean        | &check;      |
| locale                 | String         | &check;      |
| name                   | String         | &check;      |
| owner                  | Boolean        | &check;      |
| presence               | String         | &check;      |
| primaryOwner           | Boolean        | &check;      |
| profile                | Profile        | &check;      |
| realName               | String         | &check;      |
| restricted             | Boolean        | &check;      |
| stranger               | Boolean        | &check;      |
| teamId                 | String         | &cross;      |
| twoFactorType          | String         | &check;      |
| ultraRestricted        | Boolean        | &check;      |
| whoCanShareContactCard | String         | &check;      |
| workflowBot            | Boolean        | &check;      |

#### EnterpriseUser
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| enterpriseId   | String       | &check;      |
| enterpriseName | String       | &check;      |
| id             | String       | &cross;      |
| isAdmin        | Boolean      | &check;      |
| isOwner        | Boolean      | &check;      |
| teams          | List<String> | &check;      |

#### Profile
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| alwaysActive          | Boolean  | &check;      |
| apiAppId              | String   | &check;      |
| botId                 | String   | &check;      |
| displayName           | String   | &check;      |
| displayNameNormalized | String   | &check;      |
| email                 | String   | &check;      |
| guestChannels         | String   | &check;      |
| guestExpirationTs     | Long     | &check;      |
| guestInvitedBy        | String   | &check;      |
| phone                 | String   | &check;      |
| realName              | String   | &check;      |
| realNameNormalized    | String   | &check;      |
| skype                 | String   | &check;      |
| team                  | String   | &check;      |
| title                 | String   | &check;      |
