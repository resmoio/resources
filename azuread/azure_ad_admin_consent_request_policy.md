---
description: Azure Active Directory Admin Consent Request Policy
---
azure_ad_admin_consent_request_policy
-------------------------------------

| **Name**              | **Type**                        | **Nullable** |
| --------------------- | ------------------------------- | ------------ |
| id                    | String                          | &cross;      |
| isEnabled             | Boolean                         | &check;      |
| notifyReviewers       | Boolean                         | &check;      |
| oDataType             | String                          | &check;      |
| remindersEnabled      | Boolean                         | &check;      |
| requestDurationInDays | Int                             | &check;      |
| reviewers             | List<AccessReviewReviewerScope> | &check;      |
| version               | Int                             | &check;      |

#### AccessReviewReviewerScope
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| oDataType | String   | &check;      |
| query     | String   | &check;      |
| queryRoot | String   | &check;      |
| queryType | String   | &check;      |

#### DirectoryObject
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| oDataType | String   | &check;      |
