---
description: JumpCloud Policy
---
jumpcloud_policy
----------------

| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| deviceGroups     | List<String> | &cross;      |
| id               | String       | &cross;      |
| name             | String       | &check;      |
| organizationId   | String       | &cross;      |
| organizationName | String       | &cross;      |
| policyGroups     | List<String> | &cross;      |
| template         | Template     | &check;      |
| values           | List<Value>  | &cross;      |

#### AppleRestrictions
| **Name**                 | **Type**     | **Nullable** |
| ------------------------ | ------------ | ------------ |
| requiresSupervision      | Boolean      | &check;      |
| supportedEnrollmentTypes | List<String> | &check;      |

#### Group
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| type     | String   | &cross;      |

#### OsRestriction
| **Name**              | **Type**              | **Nullable** |
| --------------------- | --------------------- | ------------ |
| withAppleRestrictions | WithAppleRestrictions | &check;      |

#### Template
| **Name**       | **Type**            | **Nullable** |
| -------------- | ------------------- | ------------ |
| activation     | String              | &check;      |
| alert          | String              | &check;      |
| behavior       | String              | &check;      |
| deliveryTypes  | List<String>        | &check;      |
| description    | String              | &check;      |
| displayName    | String              | &check;      |
| id             | String              | &check;      |
| name           | String              | &check;      |
| osMetaFamily   | String              | &check;      |
| osRestrictions | List<OsRestriction> | &check;      |
| reference      | String              | &check;      |
| state          | String              | &check;      |

#### Value
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| configFieldID | String   | &check;      |
| value         | String   | &check;      |

#### WithAppleRestrictions
| **Name**          | **Type**          | **Nullable** |
| ----------------- | ----------------- | ------------ |
| appleRestrictions | AppleRestrictions | &check;      |
| deprecatedVersion | String            | &check;      |
| earliestVersion   | String            | &check;      |
| osName            | String            | &check;      |
