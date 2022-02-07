---
description: aws_s3_bucket
---

# S3 Bucket

Schema
```
{
	accountId: String,
	acl: ACL,
	creationDate: String,
	kmsMasterKeyID: String,
	name: String,
	policy: JSON,
	policyStatus: PolicyStatus,
	publicAccessBlockConfiguration: PublicAccessConfiguration,
	region: String,
	sseAlgorithm: String,
	tags: Map<String,String>,
	versioning: String,
}
```
