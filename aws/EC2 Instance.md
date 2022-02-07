---
description: aws_ec2_instance
---

# EC2 Instance

Schema
```
{
	accountId: String,
	amiLaunchIndex: Int,
	architecture: String,
	blockDeviceMappings: List<BlockDeviceMapping>,
	capacityReservationSpecification: CapacityReservationSpecification,
	clientToken: String,
	cpuOptions: CpuOptions,
	ebsOptimized: Boolean,
	enaSupport: Boolean,
	enclaveOptions: EnclaveOptions,
	hibernateOptions: HibernateOptions,
	hypervisor: String,
	iamInstanceProfile: IamInstanceProfile,
	id: String,
	imageId: String,
	keyName: String,
	launchTime: String,
	metadataOptions: MetadataOptions,
	monitoring: Monitoring,
	networkInterfaces: List<NetworkInterface>,
	placement: Placement,
	platformDetails: String,
	privateDnsName: String,
	privateDnsNameOptions: PrivateDnsNameOptions,
	publicIpAddress: String,
	region: String,
	reservationId: String,
	rootDeviceName: String,
	rootDeviceType: String,
	securityGroups: List<SecurityGroup>,
	sourceDestCheck: Boolean,
	state: State,
	stateTransitionReason: String,
	subnetId: String,
	tags: Map<String,String>,
	type: String,
	usageOperation: String,
	usageOperationUpdateTime: String,
	virtualizationType: String,
	vpcId: String,
}
```
