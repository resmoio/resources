---
description: Amazon Web Services RDS Cluster Snapshot
---
aws_rds_cluster_snapshot
------------------------

| **Name**                         | **Type**           | **Nullable** |
| -------------------------------- | ------------------ | ------------ |
| accountId                        | String             | &cross;      |
| allocatedStorage                 | Int                | &check;      |
| arn                              | String             | &cross;      |
| attributes                       | Map<String,List>   | &check;      |
| availabilityZones                | List<String>       | &check;      |
| clusterCreateTime                | String             | &check;      |
| dbClusterIdentifier              | String             | &cross;      |
| engine                           | String             | &check;      |
| engineMode                       | String             | &check;      |
| engineVersion                    | String             | &check;      |
| iamDatabaseAuthenticationEnabled | Boolean            | &check;      |
| id                               | String             | &cross;      |
| kmsKeyId                         | String             | &check;      |
| licenseModel                     | String             | &check;      |
| masterUsername                   | String             | &check;      |
| percentProgress                  | Int                | &check;      |
| port                             | Int                | &check;      |
| region                           | String             | &cross;      |
| snapshotCreateTime               | String             | &check;      |
| snapshotType                     | String             | &check;      |
| sourceDBClusterSnapshotArn       | String             | &check;      |
| status                           | String             | &check;      |
| storageEncrypted                 | Boolean            | &check;      |
| tagList                          | Map<String,String> | &check;      |
| vpcId                            | String             | &check;      |
