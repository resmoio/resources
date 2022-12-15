---
description: LaunchDarkly Environment
---
launchdarkly_environment
------------------------

| **Name**           | **Type**         | **Nullable** |
| ------------------ | ---------------- | ------------ |
| _id                | String           | &cross;      |
| apiKey             | String           | &check;      |
| approvalSettings   | ApprovalSettings | &check;      |
| color              | String           | &check;      |
| confirmChanges     | Boolean          | &check;      |
| defaultTrackEvents | Boolean          | &check;      |
| defaultTtl         | Int              | &check;      |
| key                | String           | &check;      |
| mobileKey          | String           | &check;      |
| name               | String           | &check;      |
| projectKey         | String           | &check;      |
| requireComments    | Boolean          | &check;      |
| secureMode         | Boolean          | &check;      |
| tags               | List<String>     | &check;      |

#### ApprovalSettings
| **Name**                         | **Type**                       | **Nullable** |
| -------------------------------- | ------------------------------ | ------------ |
| bypassApprovalsForPendingChanges | Boolean                        | &check;      |
| canApplyDeclinedChanges          | Boolean                        | &check;      |
| canReviewOwnRequest              | Boolean                        | &check;      |
| minNumApprovals                  | Int                            | &check;      |
| required                         | Boolean                        | &check;      |
| requiredApprovalTags             | List<String>                   | &check;      |
| serviceConfig                    | ApprovalSettings.ServiceConfig | &check;      |
| serviceKind                      | String                         | &check;      |

#### ApprovalSettings.ServiceConfig
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |

