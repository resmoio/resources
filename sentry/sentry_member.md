---
description: Sentry Member
---
sentry_member
-------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| dateCreated  | String       | &check;      |
| email        | String       | &check;      |
| expired      | Boolean      | &check;      |
| flags        | Flag         | &check;      |
| id           | String       | &cross;      |
| inviteStatus | String       | &check;      |
| inviterName  | String       | &check;      |
| orgRole      | String       | &check;      |
| organization | Organization | &check;      |
| pending      | Boolean      | &check;      |
| role         | String       | &check;      |
| roleName     | String       | &check;      |
| user         | User         | &check;      |

#### Email
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| email       | String   | &check;      |
| id          | String   | &cross;      |
| is_verified | Boolean  | &check;      |

#### Flag
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| memberLimitRestricted | Boolean  | &check;      |
| ssoInvalid            | Boolean  | &check;      |
| ssoLinked             | Boolean  | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| slug     | String   | &check;      |

#### User
| **Name**        | **Type**    | **Nullable** |
| --------------- | ----------- | ------------ |
| dateJoined      | String      | &check;      |
| email           | String      | &check;      |
| emails          | List<Email> | &check;      |
| has2fa          | Boolean     | &check;      |
| hasPasswordAuth | Boolean     | &check;      |
| id              | String      | &cross;      |
| isActive        | Boolean     | &check;      |
| isManaged       | Boolean     | &check;      |
| isStaff         | Boolean     | &check;      |
| isSuperuser     | Boolean     | &check;      |
| lastActive      | String      | &check;      |
| lastLogin       | String      | &check;      |
| name            | String      | &check;      |
| username        | String      | &check;      |
