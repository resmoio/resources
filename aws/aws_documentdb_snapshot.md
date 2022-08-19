---
description: Amazon Web Services DocumentDB Snapshot
---
aws_documentdb_snapshot
-----------------------

| **Name**                    | **Type**     | **Nullable** |
| --------------------------- | ------------ | ------------ |
| accountId                   | String       | &cross;      |
| accountName                 | String       | &check;      |
| availabilityZones           | List<String> | &check;      |
| clusterCreateTime           | String       | &check;      |
| dbClusterIdentifier         | String       | &check;      |
| dbClusterSnapshotArn        | String       | &check;      |
| dbClusterSnapshotIdentifier | String       | &cross;      |
| engine                      | String       | &check;      |
| engineVersion               | String       | &check;      |
| kmsKeyId                    | String       | &check;      |
| masterUsername              | String       | &check;      |
| port                        | Int          | &check;      |
| region                      | String       | &cross;      |
| snapshotCreateTime          | String       | &check;      |
| snapshotType                | String       | &check;      |
| sourceDBClusterSnapshotArn  | String       | &check;      |
| status                      | String       | &check;      |
| storageEncrypted            | Boolean      | &check;      |
| vpcId                       | String       | &check;      |
