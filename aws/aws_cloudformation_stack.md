---
description: CloudFormation Stack
---

# aws_cloudformation_stack

Schema
```
{
	accountId: String,
	capabilities: List<String>,
	changeSetId: String,
	creationTime: String,
	deletionTime: String,
	description: String,
	disableRollback: Boolean,
	enableTerminationProtection: Boolean,
	id: String,
	name: String,
	outputs: List<String>,
	parentId: String,
	region: String,
	roleArn: String,
	rollbackConfiguration: RollbackConfiguration,
	rootId: String,
	status: String,
	statusReason: String,
	timeoutInMinutes: Int,
}
```
