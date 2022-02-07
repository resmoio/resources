---
description: Autoscaling Launch Configuration
---

# aws_autoscaling_launch_configuration

Schema
```
{
	accountId: String,
	arn: String,
	associatePublicIpAddress: Boolean,
	blockDeviceMappings: List<BlockDeviceMapping>,
	classicLinkVPCId: String,
	classicLinkVPCSecurityGroups: List<String>,
	createdTime: String,
	ebsOptimized: Boolean,
	iamInstanceProfile: String,
	imageId: String,
	instanceMonitoring: Boolean,
	instanceType: String,
	kernelId: String,
	keyName: String,
	metadataOptions: InstanceMetadataOptions,
	name: String,
	placementTenancy: String,
	ramdiskId: String,
	region: String,
	securityGroups: List<String>,
	spotPrice: String,
	userData: String,
}
```
