---
description: Amazon Web Services Support Case
---
aws_support_case
----------------

| **Name**             | **Type**                 | **Nullable** |
| -------------------- | ------------------------ | ------------ |
| accountId            | String                   | &cross;      |
| caseId               | String                   | &cross;      |
| categoryCode         | String                   | &check;      |
| ccEmailAddresses     | List<String>             | &check;      |
| displayId            | String                   | &check;      |
| language             | String                   | &check;      |
| recentCommunications | RecentCaseCommunications | &check;      |
| serviceCode          | String                   | &check;      |
| severityCode         | String                   | &check;      |
| status               | String                   | &check;      |
| subject              | String                   | &check;      |
| submittedBy          | String                   | &check;      |
| timeCreated          | String                   | &check;      |

#### Communication
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| caseId      | String   | &check;      |
| submittedBy | String   | &check;      |
| timeCreated | String   | &check;      |

#### RecentCaseCommunications
| **Name**       | **Type**            | **Nullable** |
| -------------- | ------------------- | ------------ |
| communications | List<Communication> | &check;      |
