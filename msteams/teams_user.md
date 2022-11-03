---
description: Microsoft Teams User
---
teams_user
----------

| **Name**          | **Type**      | **Nullable** |
| ----------------- | ------------- | ------------ |
| businessPhones    | List<String>  | &check;      |
| channels          | List<Channel> | &check;      |
| displayName       | String        | &check;      |
| givenName         | String        | &check;      |
| id                | String        | &cross;      |
| jobTitle          | String        | &check;      |
| mail              | String        | &check;      |
| mobilePhone       | String        | &check;      |
| officeLocation    | String        | &check;      |
| preferredLanguage | String        | &check;      |
| surname           | String        | &check;      |
| userPrincipalName | String        | &check;      |

#### Channel
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| channelId    | String       | &cross;      |
| channelName  | String       | &check;      |
| channelRoles | List<String> | &check;      |
