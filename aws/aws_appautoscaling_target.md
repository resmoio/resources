---
description: Amazon Web Services Application Auto Scaling Target
---
aws_appautoscaling_target
-------------------------

| **Name**          | **Type**       | **Nullable** |
| ----------------- | -------------- | ------------ |
| accountId         | String         | &cross;      |
| accountName       | String         | &check;      |
| creationTime      | String         | &check;      |
| maxCapacity       | Int            | &check;      |
| minCapacity       | Int            | &check;      |
| region            | String         | &cross;      |
| resourceId        | String         | &cross;      |
| roleARN           | String         | &check;      |
| scalableDimension | String         | &check;      |
| serviceNamespace  | String         | &cross;      |
| suspendedState    | SuspendedState | &check;      |

#### SuspendedState
| **Name**                   | **Type** | **Nullable** |
| -------------------------- | -------- | ------------ |
| dynamicScalingInSuspended  | Boolean  | &check;      |
| dynamicScalingOutSuspended | Boolean  | &check;      |
| scheduledScalingSuspended  | Boolean  | &check;      |
