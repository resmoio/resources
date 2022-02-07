---
description: aws_kms_grant
---

# KMS Grant

Schema
```
{
	accountId: String,
	constraints: GrantConstraints,
	creationDate: Date,
	granteePrincipal: String,
	id: String,
	issuingAccount: String,
	keyId: String,
	name: String,
	operations: List<String>,
	region: String,
	retiringPrincipal: String,
}
```
