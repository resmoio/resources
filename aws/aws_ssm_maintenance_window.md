---
description: Amazon Web Services SSM Maintenance Window
---
aws_ssm_maintenance_window
--------------------------

| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| accountId         | String   | &cross;      |
| accountName       | String   | &check;      |
| cutoff            | Int      | &check;      |
| description       | String   | &check;      |
| duration          | Int      | &check;      |
| enabled           | Boolean  | &check;      |
| endDate           | String   | &check;      |
| name              | String   | &check;      |
| nextExecutionTime | String   | &check;      |
| region            | String   | &cross;      |
| schedule          | String   | &check;      |
| scheduleOffset    | Int      | &check;      |
| scheduleTimezone  | String   | &check;      |
| startDate         | String   | &check;      |
| windowId          | String   | &cross;      |
