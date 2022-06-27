---
description: Amazon Web Services Autoscaling Scheduled Action
---
aws_autoscaling_scheduled_action
--------------------------------

| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| accountId            | String   | &cross;      |
| autoScalingGroupName | String   | &check;      |
| desiredCapacity      | Int      | &check;      |
| endTime              | String   | &check;      |
| maxSize              | Int      | &check;      |
| minSize              | Int      | &check;      |
| recurrence           | String   | &check;      |
| region               | String   | &cross;      |
| scheduledActionARN   | String   | &cross;      |
| scheduledActionName  | String   | &check;      |
| startTime            | String   | &check;      |
| time                 | String   | &check;      |
| timeZone             | String   | &check;      |
