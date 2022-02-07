---
description: ECS Task
---

# aws_ecs_task

Schema
```
{
	accountId: String,
	arn: String,
	attachments: List<Attachment>,
	attributes: List<Attribute>,
	capacityProviderName: String,
	clusterArn: String,
	connectivity: String,
	containerInstanceArn: String,
	containers: List<Container>,
	cpu: String,
	createdAt: String,
	desiredStatus: String,
	enableExecuteCommand: Boolean,
	ephemeralStorage: EphemeralStorage,
	executionStoppedAt: String,
	healthStatus: String,
	inferenceAccelerators: List<InferenceAccelerator>,
	launchType: String,
	memory: String,
	overrides: TaskOverride,
	platformFamily: String,
	platformVersion: String,
	region: String,
	startedAt: String,
	startedBy: String,
	stopCode: String,
	stoppedReason: String,
	tags: Map<String,String>,
	taskDefinitionArn: String,
	version: Long,
}
```
