---
description: Amazon Web Services CloudWatch Metric Alarm
---
aws_cloudwatch_metric_alarm
---------------------------

| **Name**                           | **Type**        | **Nullable** |
| ---------------------------------- | --------------- | ------------ |
| accountId                          | String          | &cross;      |
| accountName                        | String          | &check;      |
| actionsEnabled                     | Boolean         | &check;      |
| alarmActions                       | List<String>    | &check;      |
| alarmArn                           | String          | &cross;      |
| alarmConfigurationUpdatedTimestamp | String          | &check;      |
| alarmDescription                   | String          | &check;      |
| alarmName                          | String          | &cross;      |
| comparisonOperator                 | String          | &check;      |
| datapointsToAlarm                  | Int             | &check;      |
| dimensions                         | List<Dimension> | &check;      |
| evaluateLowSampleCountPercentile   | String          | &check;      |
| evaluationPeriods                  | Int             | &check;      |
| extendedStatistic                  | String          | &check;      |
| insufficientDataActions            | List<String>    | &check;      |
| metricName                         | String          | &check;      |
| namespace                          | String          | &check;      |
| okActions                          | List<String>    | &check;      |
| period                             | Int             | &check;      |
| region                             | String          | &cross;      |
| statistic                          | String          | &check;      |
| threshold                          | Double          | &check;      |
| thresholdMetricId                  | String          | &check;      |
| treatMissingData                   | String          | &check;      |
| unit                               | String          | &check;      |

#### Dimension
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| value    | String   | &check;      |
