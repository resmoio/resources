---
description: Amazon Web Services SSM Patch Baseline
---
aws_ssm_patch_baseline
----------------------

| **Name**                         | **Type**          | **Nullable** |
| -------------------------------- | ----------------- | ------------ |
| accountId                        | String            | &cross;      |
| accountName                      | String            | &check;      |
| approvalRules                    | PatchRuleGroup    | &check;      |
| approvedPatches                  | List<String>      | &check;      |
| approvedPatchesComplianceLevel   | String            | &check;      |
| approvedPatchesEnableNonSecurity | Boolean           | &check;      |
| baselineId                       | String            | &cross;      |
| createdDate                      | String            | &check;      |
| description                      | String            | &check;      |
| globalFilters                    | PatchFilterGroup  | &check;      |
| modifiedDate                     | String            | &check;      |
| name                             | String            | &check;      |
| operatingSystem                  | String            | &check;      |
| patchGroups                      | List<String>      | &check;      |
| region                           | String            | &cross;      |
| rejectedPatches                  | List<String>      | &check;      |
| rejectedPatchesAction            | String            | &check;      |
| sources                          | List<PatchSource> | &check;      |

#### PatchFilterGroup
| **Name**     | **Type**                           | **Nullable** |
| ------------ | ---------------------------------- | ------------ |
| patchFilters | List<PatchFilterGroup.PatchFilter> | &check;      |

#### PatchFilterGroup.PatchFilter
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| key      | String       | &check;      |
| values   | List<String> | &check;      |

#### PatchRuleGroup
| **Name**   | **Type**                       | **Nullable** |
| ---------- | ------------------------------ | ------------ |
| patchRules | List<PatchRuleGroup.PatchRule> | &check;      |

#### PatchRuleGroup.PatchRule
| **Name**          | **Type**         | **Nullable** |
| ----------------- | ---------------- | ------------ |
| approveAfterDays  | Int              | &check;      |
| approveUntilDate  | String           | &check;      |
| complianceLevel   | String           | &check;      |
| enableNonSecurity | Boolean          | &check;      |
| patchFilterGroup  | PatchFilterGroup | &check;      |

#### PatchSource
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| configuration | String       | &check;      |
| name          | String       | &check;      |
| products      | List<String> | &check;      |
