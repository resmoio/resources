---
description: SQS Queue
---

# aws_sqs_queue

Schema
```
{
	accountId: String,
	arn: String,
	createdTimestamp: String,
	deduplicationScope: String,
	delaySeconds: Int,
	fifoQueue: Boolean,
	fifoThroughputLimit: String,
	kmsDataKeyReusePeriodSeconds: Int,
	kmsMasterKeyId: String,
	maxMessageSize: Int,
	name: String,
	policy: JSON,
	region: String,
	retentionPeriod: Int,
	sqsManagedSseEnabled: Boolean,
	visibilityTimeout: Int,
}
```
