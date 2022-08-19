---
description: Amazon Web Services TrustedAdvisor Check Result
---
aws_trustedadvisor_check_result
-------------------------------

| **Name**                   | **Type**                              | **Nullable** |
| -------------------------- | ------------------------------------- | ------------ |
| accountId                  | String                                | &cross;      |
| accountName                | String                                | &check;      |
| categorySpecificSummary    | TrustedAdvisorCategorySpecificSummary | &check;      |
| checkId                    | String                                | &cross;      |
| hasFlaggedResources        | Boolean                               | &check;      |
| millisUntilNextRefreshable | String                                | &check;      |
| resourcesSummary           | TrustedAdvisorResourcesSummary        | &check;      |
| status                     | String                                | &check;      |

#### TrustedAdvisorCategorySpecificSummary
| **Name**       | **Type**                            | **Nullable** |
| -------------- | ----------------------------------- | ------------ |
| costOptimizing | TrustedAdvisorCostOptimizingSummary | &check;      |

#### TrustedAdvisorCostOptimizingSummary
| **Name**                       | **Type** | **Nullable** |
| ------------------------------ | -------- | ------------ |
| estimatedMonthlySavings        | Double   | &check;      |
| estimatedPercentMonthlySavings | Double   | &check;      |

#### TrustedAdvisorResourcesSummary
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| resourcesFlagged    | Long     | &check;      |
| resourcesIgnored    | Long     | &check;      |
| resourcesProcessed  | Long     | &check;      |
| resourcesSuppressed | Long     | &check;      |
