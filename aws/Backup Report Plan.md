---
description: aws_backup_report_plan
---

# Backup Report Plan

Schema
```
{
	accountId: String,
	arn: String,
	creationTime: Date,
	deliveryChannel: ReportDeliveryChannel,
	deploymentStatus: String,
	description: String,
	lastAttemptedExecutionTime: Date,
	lastSuccessfulExecutionTime: Date,
	name: String,
	region: String,
	setting: ReportSetting,
}
```
