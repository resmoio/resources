---
description: aws_rds_cluster_snapshot
---

# RDS Cluster Snapshot

Schema
```
{
	accountId: String,
	allocatedStorage: Int,
	arn: String,
	attributes: Map<String,List>,
	availabilityZones: List<String>,
	clusterCreateTime: String,
	dbClusterIdentifier: String,
	engine: String,
	engineMode: String,
	engineVersion: String,
	iamDatabaseAuthenticationEnabled: Boolean,
	id: String,
	kmsKeyId: String,
	licenseModel: String,
	masterUsername: String,
	percentProgress: Int,
	port: Int,
	region: String,
	snapshotCreateTime: String,
	snapshotType: String,
	sourceDBClusterSnapshotArn: String,
	status: String,
	storageEncrypted: Boolean,
	tagList: Map<String,String>,
	vpcId: String,
}
```
