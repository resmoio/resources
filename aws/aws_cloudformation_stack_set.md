---
description: aws_cloudformation_stack_set
---

# CloudFormation StackSet

Schema
```
{
	accountId: String,
	administrationRoleArn: String,
	arn: String,
	autoDeployment: AutoDeployment,
	capabilities: List<String>,
	description: String,
	id: String,
	managedExecution: ManagedExecution,
	name: String,
	organizationalUnitIds: List<String>,
	permissionModel: String,
	region: String,
	status: String,
	tags: Map<String,String>,
	templateBody: JSON,
}
```
