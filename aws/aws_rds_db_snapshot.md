---
description: RDS DB Snapshot
---

# aws_rds_db_snapshot

Schema
```
{
	accountId: String,
	allocatedStorage: Int,
	arn: String,
	attributes: Map<String,List>,
	availabilityZone: String,
	dbInstanceIdentifier: String,
	dbiResourceId: String,
	encrypted: Boolean,
	engine: String,
	engineVersion: String,
	iamDatabaseAuthenticationEnabled: Boolean,
	id: String,
	instanceCreateTime: String,
	iops: Int,
	kmsKeyId: String,
	licenseModel: String,
	masterUsername: String,
	optionGroupName: String,
	originalSnapshotCreateTime: String,
	percentProgress: Int,
	port: Int,
	processorFeatures: Map<String,String>,
	region: String,
	snapshotCreateTime: String,
	snapshotTarget: String,
	snapshotType: String,
	sourceDBSnapshotIdentifier: String,
	sourceRegion: String,
	status: String,
	storageType: String,
	tagList: Map<String,String>,
	tdeCredentialArn: String,
	timezone: String,
	vpcId: String,
}
```
