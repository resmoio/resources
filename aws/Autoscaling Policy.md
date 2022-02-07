---
description: aws_autoscaling_policy
---

# Autoscaling Policy

Schema
```
{
	accountId: String,
	adjustmentType: String,
	alarms: List<String>,
	arn: String,
	autoScalingGroupName: String,
	cooldown: Int,
	enabled: Boolean,
	estimatedInstanceWarmup: Int,
	metricAggregationType: String,
	minAdjustmentMagnitude: Int,
	minAdjustmentStep: Int,
	name: String,
	predictiveScalingConfiguration: PredictiveScalingConfiguration,
	region: String,
	scalingAdjustment: Int,
	stepAdjustments: List<StepAdjustment>,
	targetTrackingConfiguration: TargetTrackingConfiguration,
	type: String,
}
```
