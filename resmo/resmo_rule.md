---
description: Resmo Rule
---
resmo_rule
----------

| **Name**              | **Type**     | **Nullable** |
| --------------------- | ------------ | ------------ |
| accountId             | String       | &check;      |
| affectedResourceType  | String       | &check;      |
| createdAt             | Timestamp    | &check;      |
| createdBy             | String       | &check;      |
| description           | String       | &check;      |
| id                    | String       | &cross;      |
| integrations          | List<String> | &check;      |
| labels                | List<String> | &check;      |
| name                  | String       | &check;      |
| queryId               | String       | &check;      |
| referredResourceTypes | List<String> | &check;      |
| remediation           | String       | &check;      |
| severity              | String       | &check;      |
| updatedAt             | Timestamp    | &check;      |

#### Query
| **Name** | **Type**  | **Nullable** |
| -------- | --------- | ------------ |
| label    | String    | &check;      |
| raw      | Query.Raw | &check;      |
| ref      | Query.Ref | &check;      |

#### Query.Raw
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| sql      | String   | &cross;      |

#### Query.Ref
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
