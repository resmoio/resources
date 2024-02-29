---
description: Google Workspace User Usage Report
---
gsuite_user_usage_report
------------------------

| **Name**     | **Type**                              | **Nullable** |
| ------------ | ------------------------------------- | ------------ |
| customerId   | String                                | &cross;      |
| date         | String                                | &cross;      |
| parameters   | Map<String,UsageReportParameterValue> | &cross;      |
| primaryEmail | String                                | &cross;      |

#### UsageReportParameterValue
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| boolValue     | Boolean  | &check;      |
| datetimeValue | String   | &check;      |
| intValue      | Long     | &check;      |
| stringValue   | String   | &check;      |
