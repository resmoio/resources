---
description: ECS Task Definition
---

# aws_ecs_task_definition

Schema
```
{
	accountId: String,
	arn: String,
	compatibilities: List<String>,
	containerDefinitions: List<ContainerDefinition>,
	cpu: String,
	deregisteredAt: String,
	ephemeralStorage: EphemeralStorage,
	executionRoleArn: String,
	family: String,
	inferenceAccelerators: List<InferenceAccelerator>,
	ipcMode: String,
	memory: String,
	networkMode: String,
	pidMode: String,
	placementConstraints: List<PlacementConstraint>,
	proxyConfiguration: ProxyConfiguration,
	region: String,
	registeredAt: String,
	registeredBy: String,
	requiresAttributes: List<RequireAttribute>,
	revision: Int,
	taskDefinitionArn: String,
	taskRoleArn: String,
	volumes: List<Volume>,
}
```
