---
description: ECS Cluster
---

# aws_ecs_cluster

Schema
```
{
	accountId: String,
	arn: String,
	attachmentStatus: String,
	attachments: List<Attachment>,
	capacityProviders: List<String>,
	configuration: Configuration,
	defaultCapacityProviderStrategy: List<DefaultCapacityProviderStrategy>,
	name: String,
	region: String,
	settings: Map<String,String>,
	status: String,
	tags: Map<String,String>,
}
```
