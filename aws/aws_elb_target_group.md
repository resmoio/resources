---
description: aws_elb_target_group
---

# ELB Target Group

Schema
```
{
	accountId: String,
	attributes: Map<String,String>,
	healthCheckEnabled: Boolean,
	healthCheckIntervalSeconds: Int,
	healthCheckPath: String,
	healthCheckPort: String,
	healthCheckProtocol: String,
	healthCheckTimeoutSeconds: Int,
	healthyThresholdCount: Int,
	ipAddressType: String,
	loadBalancerArns: List<String>,
	matcher: Matcher,
	port: Int,
	protocolVersion: String,
	region: String,
	targetGroupArn: String,
	targetGroupName: String,
	targetType: String,
	unhealthyThresholdCount: Int,
	vpcId: String,
}
```
