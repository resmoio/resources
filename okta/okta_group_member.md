---
description: Okta Group Member
---
okta_group_member
-----------------

| **Name**        | **Type**    | **Nullable** |
| --------------- | ----------- | ------------ |
| activated       | String      | &check;      |
| created         | String      | &check;      |
| credentials     | Credentials | &check;      |
| groupId         | String      | &cross;      |
| id              | String      | &cross;      |
| lastUpdated     | String      | &check;      |
| passwordChanged | String      | &check;      |
| profile         | Profile     | &check;      |
| status          | String      | &check;      |
| statusChanged   | String      | &check;      |
| type            | Type        | &check;      |

#### Credentials
| **Name** | **Type**             | **Nullable** |
| -------- | -------------------- | ------------ |
| provider | Credentials.Provider | &check;      |

#### Credentials.Provider
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### Profile
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| email     | String   | &check;      |
| firstName | String   | &check;      |
| lastName  | String   | &check;      |
| login     | String   | &check;      |

#### Type
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
