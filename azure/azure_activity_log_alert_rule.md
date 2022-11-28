---
description: Azure Activity Log Alert Rule
---
azure_activity_log_alert_rule
-----------------------------

| **Name**          | **Type**           | **Nullable** |
| ----------------- | ------------------ | ------------ |
| actionGroupIds    | List<String>       | &check;      |
| description       | String             | &check;      |
| enabled           | Boolean            | &check;      |
| equalsConditions  | Map<String,String> | &check;      |
| id                | String             | &cross;      |
| location          | String             | &check;      |
| name              | String             | &cross;      |
| resourceGroupName | String             | &cross;      |
| scopes            | List<String>       | &check;      |
| subscriptionId    | String             | &cross;      |
| tags              | Map<String,String> | &check;      |
| type              | String             | &cross;      |
