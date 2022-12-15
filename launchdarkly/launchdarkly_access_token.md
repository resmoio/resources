---
description: LaunchDarkly Access Token
---
launchdarkly_access_token
-------------------------

| **Name**          | **Type**         | **Nullable** |
| ----------------- | ---------------- | ------------ |
| _id               | String           | &cross;      |
| _member           | Member           | &check;      |
| creationDate      | Long             | &check;      |
| customRoleIds     | List<String>     | &check;      |
| defaultApiVersion | Int              | &check;      |
| description       | String           | &check;      |
| inlineRole        | List<InlineRole> | &check;      |
| lastModified      | Long             | &check;      |
| lastUsed          | Long             | &check;      |
| memberId          | String           | &check;      |
| name              | String           | &check;      |
| ownerId           | String           | &check;      |
| role              | String           | &check;      |
| serviceToken      | Boolean          | &check;      |
| token             | String           | &check;      |

#### InlineRole
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| actions      | List<String> | &check;      |
| effect       | String       | &check;      |
| notActions   | List<String> | &check;      |
| notResources | List<String> | &check;      |
| resources    | List<String> | &check;      |

#### Member
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| _id       | String       | &check;      |
| _links    | Member.Links | &check;      |
| email     | String       | &check;      |
| firstName | String       | &check;      |
| lastName  | String       | &check;      |
| role      | String       | &check;      |

#### Member.Links
| **Name** | **Type**          | **Nullable** |
| -------- | ----------------- | ------------ |
| self     | Member.Links.Self | &check;      |

#### Member.Links.Self
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| type     | String   | &check;      |
