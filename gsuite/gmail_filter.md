---
description: Google Workspace Filter
---
gmail_filter
------------

| **Name**   | **Type**       | **Nullable** |
| ---------- | -------------- | ------------ |
| action     | FilterAction   | &check;      |
| criteria   | FilterCriteria | &check;      |
| customerId | String         | &cross;      |
| id         | String         | &cross;      |
| userEmail  | String         | &cross;      |
| userId     | String         | &cross;      |

#### FilterAction
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| addLabelIds    | List<String> | &check;      |
| forward        | String       | &check;      |
| removeLabelIds | List<String> | &check;      |

#### FilterCriteria
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| excludeChats   | Boolean  | &check;      |
| from           | String   | &check;      |
| hasAttachment  | Boolean  | &check;      |
| negatedQuery   | String   | &check;      |
| query          | String   | &check;      |
| size           | Int      | &check;      |
| sizeComparison | String   | &check;      |
| subject        | String   | &check;      |
| to             | String   | &check;      |
