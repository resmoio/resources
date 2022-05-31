---
description: Amazon Web Services CloudWatch Metric Filter
---
aws_cloudwatch_metric_filter
----------------------------

| **Name**              | **Type**                   | **Nullable** |
| --------------------- | -------------------------- | ------------ |
| creationTime          | Long                       | &check;      |
| filterName            | String                     | &cross;      |
| filterPattern         | String                     | &check;      |
| logGroupName          | String                     | &check;      |
| metricTransformations | List<MetricTransformation> | &cross;      |

#### MetricTransformation
| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| dimensions      | Map<String,String> | &check;      |
| metricName      | String             | &check;      |
| metricNamespace | String             | &check;      |
| metricValue     | String             | &check;      |
| unit            | String             | &check;      |
