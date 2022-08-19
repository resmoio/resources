---
description: Amazon Web Services Autoscaling Policy
---
aws_autoscaling_policy
----------------------

| **Name**                       | **Type**                       | **Nullable** |
| ------------------------------ | ------------------------------ | ------------ |
| accountId                      | String                         | &cross;      |
| accountName                    | String                         | &check;      |
| adjustmentType                 | String                         | &check;      |
| alarms                         | List<String>                   | &check;      |
| arn                            | String                         | &cross;      |
| autoScalingGroupName           | String                         | &check;      |
| cooldown                       | Int                            | &check;      |
| enabled                        | Boolean                        | &check;      |
| estimatedInstanceWarmup        | Int                            | &check;      |
| metricAggregationType          | String                         | &check;      |
| minAdjustmentMagnitude         | Int                            | &check;      |
| minAdjustmentStep              | Int                            | &check;      |
| name                           | String                         | &cross;      |
| predictiveScalingConfiguration | PredictiveScalingConfiguration | &check;      |
| region                         | String                         | &cross;      |
| scalingAdjustment              | Int                            | &check;      |
| stepAdjustments                | List<StepAdjustment>           | &check;      |
| targetTrackingConfiguration    | TargetTrackingConfiguration    | &check;      |
| type                           | String                         | &cross;      |

#### CustomizedMetricSpecification
| **Name**   | **Type**           | **Nullable** |
| ---------- | ------------------ | ------------ |
| dimensions | Map<String,String> | &check;      |
| metricName | String             | &check;      |
| namespace  | String             | &check;      |
| statistic  | String             | &check;      |
| unit       | String             | &check;      |

#### PredefinedMetricSpecification
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| predefinedMetricType | String   | &check;      |
| resourceLabel        | String   | &check;      |

#### PredictiveScalingConfiguration
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| maxCapacityBreachBehavior | String   | &check;      |
| maxCapacityBuffer         | Int      | &check;      |
| mode                      | String   | &check;      |
| schedulingBufferTime      | Int      | &check;      |

#### StepAdjustment
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| metricIntervalLowerBound | Double   | &check;      |
| metricIntervalUpperBound | Double   | &check;      |
| scalingAdjustment        | Int      | &check;      |

#### TargetTrackingConfiguration
| **Name**                      | **Type**                      | **Nullable** |
| ----------------------------- | ----------------------------- | ------------ |
| customizedMetricSpecification | CustomizedMetricSpecification | &check;      |
| disableScaleIn                | Boolean                       | &check;      |
| predefinedMetricSpecification | PredefinedMetricSpecification | &check;      |
| targetValue                   | Double                        | &check;      |
