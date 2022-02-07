---
description: VPC Security Group
---

# aws_vpc_security_group

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
