---
description: S3 Bucket
---

# aws_s3_bucket

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
