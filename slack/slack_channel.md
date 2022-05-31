---
description: Slack Channel
---
slack_channel
-------------

| **Name**                | **Type**     | **Nullable** |
| ----------------------- | ------------ | ------------ |
| connectedLimitedTeamIds | List<String> | &check;      |
| connectedTeamIds        | List<String> | &check;      |
| conversationHostId      | String       | &check;      |
| created                 | Int          | &check;      |
| creator                 | String       | &check;      |
| enterpriseId            | String       | &check;      |
| globalShared            | Boolean      | &check;      |
| id                      | String       | &cross;      |
| internalTeamIds         | List<String> | &check;      |
| isArchived              | Boolean      | &check;      |
| isChannel               | Boolean      | &check;      |
| isExtShared             | Boolean      | &check;      |
| isGeneral               | Boolean      | &check;      |
| isGroup                 | Boolean      | &check;      |
| isIm                    | Boolean      | &check;      |
| isMember                | Boolean      | &check;      |
| isMoved                 | Int          | &check;      |
| isMpim                  | Boolean      | &check;      |
| isNonThreadable         | Boolean      | &check;      |
| isOrgShared             | Boolean      | &check;      |
| isPendingExtShared      | Boolean      | &check;      |
| isPrivate               | Boolean      | &check;      |
| isReadOnly              | Boolean      | &check;      |
| isShared                | Boolean      | &check;      |
| isThreadOnly            | Boolean      | &check;      |
| isUserDeleted           | Boolean      | &check;      |
| locale                  | String       | &check;      |
| name                    | String       | &cross;      |
| nameNormalized          | String       | &check;      |
| open                    | Boolean      | &check;      |
| orgDefault              | Boolean      | &check;      |
| orgMandatory            | Boolean      | &check;      |
| parentConversation      | String       | &check;      |
| pendingConnectedTeamIds | List<String> | &check;      |
| pendingShared           | List<String> | &check;      |
| previousNames           | List<String> | &check;      |
| priority                | Double       | &check;      |
| purpose                 | Topic        | &check;      |
| sharedTeamIds           | List<String> | &check;      |
| teamId                  | String       | &cross;      |
| topic                   | Topic        | &check;      |
| unlinked                | Int          | &check;      |
| user                    | String       | &check;      |

#### Topic
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| creator  | String   | &cross;      |
| lastSet  | Int      | &cross;      |
| value    | String   | &cross;      |
