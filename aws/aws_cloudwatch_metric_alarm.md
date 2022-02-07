---
description: CloudWatch Metric Alarm
---

# aws_cloudwatch_metric_alarm

Schema
```
{
	accountId: String,
	actionsEnabled: Boolean,
	alarmActions: List<String>,
	alarmArn: String,
	alarmConfigurationUpdatedTimestamp: String,
	alarmDescription: String,
	alarmName: String,
	comparisonOperator: String,
	datapointsToAlarm: Int,
	dimensions: List<Dimension>,
	evaluateLowSampleCountPercentile: String,
	evaluationPeriods: Int,
	extendedStatistic: String,
	insufficientDataActions: List<String>,
	metricName: String,
	namespace: String,
	okActions: List<String>,
	period: Int,
	region: String,
	statistic: String,
	threshold: Double,
	thresholdMetricId: String,
	treatMissingData: String,
	unit: String,
}
```
