---
description: SaaS App Account
---
app_account
-----------

| **Name**         | **Type**       | **Nullable** |
| ---------------- | -------------- | ------------ |
| app              | String         | &check;      |
| deletedAt        | String         | &check;      |
| displayName      | String         | &check;      |
| domain           | String         | &check;      |
| identifier       | String         | &cross;      |
| lastLogin        | String         | &check;      |
| lastUsed         | String         | &check;      |
| loginMethods     | Set            | &check;      |
| owner            | String         | &check;      |
| parentUser       | ParentUser     | &check;      |
| scopesByProvider | ProviderScopes | &check;      |
| sources          | Set            | &check;      |
| status           | String         | &check;      |
| statusReason     | String         | &check;      |
| username         | String         | &check;      |

#### LoginType
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |
| type     | String   | &cross;      |

#### ParentUser
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| reason   | String   | &check;      |

#### ProviderScopes
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| github    | List<String> | &check;      |
| google    | List<String> | &check;      |
| microsoft | List<String> | &check;      |

#### Source
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| groupKey      | String   | &check;      |
| integrationId | String   | &check;      |
| recordId      | String   | &check;      |
| resourceId    | String   | &check;      |
| resourceType  | String   | &check;      |

#### SourceComparable
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| groupKey      | String   | &check;      |
| integrationId | String   | &check;      |
| resourceId    | String   | &check;      |
| resourceType  | String   | &check;      |

#### Status
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |
