---
description: JetBrains License
---
jetbrains_license
-----------------

| **Name**                   | **Type**     | **Nullable** |
| -------------------------- | ------------ | ------------ |
| assignee                   | Assignee     | &check;      |
| isAvailableToAssign        | Boolean      | &check;      |
| isSuspended                | Boolean      | &check;      |
| isTransferableBetweenTeams | Boolean      | &check;      |
| isTrial                    | Boolean      | &check;      |
| lastSeen                   | LastSeen     | &check;      |
| licenseId                  | String       | &cross;      |
| product                    | Product      | &cross;      |
| subscription               | Subscription | &check;      |
| team                       | Team         | &check;      |

#### Assignee
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &cross;      |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### LastSeen
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| isOfflineCodeGenerated | Boolean  | &check;      |
| lastAssignmentDate     | String   | &check;      |
| lastSeenDate           | String   | &check;      |

#### Product
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | String   | &cross;      |
| name     | String   | &cross;      |

#### Subscription
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| isAutomaticallyRenewed | Boolean  | &check;      |
| isOutdated             | Boolean  | &check;      |
| subscriptionPackRef    | String   | &check;      |
| validUntilDate         | String   | &check;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &cross;      |
| name     | String   | &cross;      |
