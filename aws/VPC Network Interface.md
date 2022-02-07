---
description: aws_vpc_network_interface
---

# VPC Network Interface

Schema
```
{
	accountId: String,
	association: Association,
	attachment: Attachment,
	availabilityZone: String,
	description: String,
	groups: List<Group>,
	id: String,
	interfaceType: String,
	ipv6Addresses: List<String>,
	macAddress: String,
	ownerId: String,
	privateDnsName: String,
	privateIpAddress: String,
	privateIpAddresses: List<PrivateAddress>,
	region: String,
	requesterId: String,
	requesterManaged: Boolean,
	sourceDestCheck: Boolean,
	status: String,
	subnetId: String,
	tagSet: Map<String,String>,
	vpcId: String,
}
```
