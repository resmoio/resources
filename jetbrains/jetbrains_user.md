---
description: JetBrains User
---
jetbrains_user
--------------

| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| email     | String   | &cross;      |
| lastSeen  | LastSeen | &check;      |
| licenseId | String   | &cross;      |
| name      | String   | &check;      |
| team      | Team     | &check;      |
| type      | String   | &check;      |

#### LastSeen
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| isOfflineCodeGenerated | Boolean  | &check;      |
| lastAssignmentDate     | String   | &check;      |
| lastSeenDate           | String   | &check;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &check;      |
| name     | String   | &check;      |
