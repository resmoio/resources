---
description: aws_elb_load_balancer
---

# ELB Load Balancer

Schema
```
{
	accountId: String,
	attributes: Map<String,String>,
	availabilityZones: List<AvailabilityZone>,
	canonicalHostedZoneId: String,
	createdTime: String,
	customerOwnedIpv4Pool: String,
	dnsName: String,
	ipAddressType: String,
	listeners: List<Listener>,
	loadBalancerArn: String,
	loadBalancerName: String,
	region: String,
	scheme: String,
	securityGroups: List<String>,
	type: String,
	vpcId: String,
}
```
