---
description: EventBridge Rule
---

# aws_eventbridge_rule

Schema
```
{
	accountId: String,
	arn: String,
	description: String,
	eventBusName: String,
	eventPattern: JSON,
	managedBy: String,
	name: String,
	region: String,
	roleArn: String,
	scheduleExpression: String,
	state: String,
	tags: Map<String,String>,
	targets: List<RuleTarget>,
}
```
