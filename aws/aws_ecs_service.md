---
description: aws_ecs_service
---

# ECS Service

Schema
```
{
	accountId: String,
	arn: String,
	capacityProviderStrategy: List<CapacityProviderStrategy>,
	clusterArn: String,
	createdAt: String,
	createdBy: String,
	deploymentConfiguration: DeploymentConfiguration,
	deploymentController: DeploymentController,
	deployments: List<Deployment>,
	desiredCount: Int,
	enableECSManagedTags: Boolean,
	enableExecuteCommand: Boolean,
	healthCheckGracePeriodSeconds: Int,
	launchType: String,
	loadBalancers: List<LoadBalancer>,
	name: String,
	networkConfiguration: NetworkConfiguration,
	placementConstraints: List<PlacementConstraint>,
	placementStrategy: List<PlacementStrategy>,
	platformFamily: String,
	platformVersion: String,
	propagateTasks: String,
	region: String,
	roleArn: String,
	schedulingStrategy: String,
	serviceRegistries: List<ServiceRegistry>,
	taskDefinition: String,
}
```
