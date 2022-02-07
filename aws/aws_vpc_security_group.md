---
description: aws_vpc_security_group
---

# VPC Security Group

Schema
```
{
	accountId: String,
	description: String,
	egress: List<IPPermission>,
	id: String,
	ingress: List<IPPermission>,
	name: String,
	region: String,
	tags: Map<String,String>,
	vpcId: String,
}
```
