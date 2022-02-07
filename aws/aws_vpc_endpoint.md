---
description: VPC Endpoint
---

# aws_vpc_endpoint

Schema
```
{
	accountId: String,
	creationTimestamp: String,
	dnsEntries: List<DnsEntry>,
	groups: List<Group>,
	id: String,
	networkInterfaceIds: List<String>,
	ownerId: String,
	policyDocument: JSON,
	privateDnsEnabled: Boolean,
	region: String,
	requesterManaged: Boolean,
	routeTableIds: List<String>,
	serviceName: String,
	state: String,
	subnetIds: List<String>,
	tags: Map<String,String>,
	type: String,
}
```
