---
description: Miro User
---
miro_user
---------

| **Name**            | **Type**            | **Nullable** |
| ------------------- | ------------------- | ------------ |
| active              | Boolean             | &check;      |
| displayName         | String              | &check;      |
| email               | String              | &check;      |
| emails              | List<Email>         | &check;      |
| enterpriseExtension | EnterpriseExtension | &check;      |
| groups              | List<Group>         | &check;      |
| id                  | String              | &cross;      |
| license             | String              | &check;      |
| meta                | Meta                | &check;      |
| name                | UserName            | &check;      |
| role                | String              | &check;      |
| schemas             | List<String>        | &check;      |
| userName            | String              | &check;      |

#### Email
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| display  | String   | &cross;      |
| primary  | Boolean  | &cross;      |
| value    | String   | &cross;      |

#### EnterpriseExtension
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| costCenter     | String   | &cross;      |
| department     | String   | &cross;      |
| division       | String   | &cross;      |
| employeeNumber | String   | &cross;      |
| manager        | Manager  | &cross;      |
| organization   | String   | &cross;      |

#### Group
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| display  | String   | &cross;      |
| value    | String   | &cross;      |

#### Manager
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &cross;      |
| value       | String   | &cross;      |

#### Meta
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| location     | String   | &cross;      |
| resourceType | String   | &cross;      |

#### UserName
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| familyName | String   | &cross;      |
| givenName  | String   | &cross;      |
