---
description: Amazon Web Services SSM Resource Compliance
---
aws_ssm_resource_compliance
---------------------------

| **Name**         | **Type**                   | **Nullable** |
| ---------------- | -------------------------- | ------------ |
| accountId        | String                     | &cross;      |
| accountName      | String                     | &check;      |
| complianceType   | String                     | &check;      |
| executionSummary | ComplianceExecutionSummary | &check;      |
| overallSeverity  | String                     | &check;      |
| region           | String                     | &cross;      |
| resourceId       | String                     | &cross;      |
| resourceType     | String                     | &check;      |
| status           | String                     | &check;      |

#### ComplianceExecutionSummary
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| executionId   | String   | &check;      |
| executionTime | String   | &check;      |
| executionType | String   | &check;      |
