---
description: DynamoDB Table
---

# aws_dynamodb_table

Schema
```
{
	accountId: String,
	arn: String,
	attributes: List<Attribute>,
	backup: ContinuousBackupsDescription,
	billingMode: String,
	capacity: Capacity,
	classSummary: ClassSummary,
	creationDate: String,
	encryption: Encryption,
	globalTableVersion: String,
	gsi: List<GSI>,
	keySchema: List<KeySchema>,
	name: String,
	region: String,
	replicas: List<Replica>,
	status: String,
	streamType: String,
}
```
