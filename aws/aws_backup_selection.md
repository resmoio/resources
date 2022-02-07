---
description: aws_backup_selection
---

# Backup Selection

Schema
```
{
	accountId: String,
	backupPlanId: String,
	conditions: Conditions,
	creationDate: Date,
	creatorRequestId: String,
	iamRoleArn: String,
	id: String,
	listOfTags: List<Condition>,
	name: String,
	notResources: List<String>,
	region: String,
	resources: List<String>,
}
```
