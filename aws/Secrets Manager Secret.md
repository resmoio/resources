---
description: aws_secretsmanager_secret
---

# Secrets Manager Secret

Schema
```
{
	accountId: String,
	arn: String,
	createdDate: Date,
	deletedDate: Date,
	description: String,
	kmsKeyId: String,
	lastAccessedDate: Date,
	lastChangedDate: Date,
	lastRotatedDate: Date,
	name: String,
	owningService: String,
	primaryRegion: String,
	region: String,
	resourcePolicy: JSON,
	rotationEnabled: Boolean,
	rotationLambdaARN: String,
	rotationRules: RotationRulesType,
	tags: Map<String,String>,
	versionsToStages: Map<String,List>,
}
```
