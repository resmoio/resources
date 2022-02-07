---
description: Autoscaling Group
---

# aws_autoscaling_group

Schema
```
{
	accountId: String,
	arn: String,
	availabilityZones: List<String>,
	capacityRebalance: Boolean,
	context: String,
	createdTime: String,
	defaultCooldown: Int,
	desiredCapacity: Int,
	desiredCapacityType: String,
	enabledMetrics: List<EnabledMetric>,
	healthCheckGracePeriod: Int,
	healthCheckType: String,
	launchConfigurationName: String,
	launchTemplate: LaunchTemplateSpec,
	loadBalancerNames: List<String>,
	maxInstanceLifetime: Int,
	maxSize: Int,
	minSize: Int,
	name: String,
	newInstancesProtectedFromScaleIn: Boolean,
	placementGroup: String,
	predictedCapacity: Int,
	region: String,
	serviceLinkedRoleARN: String,
	status: String,
	suspendedProcesses: List<SuspendedProcess>,
	targetGroupARNs: List<String>,
	terminationPolicies: List<String>,
	vpcZoneIdentifier: String,
	warmPoolConfiguration: WarmPoolConfiguration,
	warmPoolSize: Int,
}
```
