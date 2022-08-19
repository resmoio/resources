---
description: Amazon Web Services RDS DB Snapshot
---
aws_rds_db_snapshot
-------------------

| **Name**                         | **Type**           | **Nullable** |
| -------------------------------- | ------------------ | ------------ |
| accountId                        | String             | &cross;      |
| accountName                      | String             | &check;      |
| allocatedStorage                 | Int                | &check;      |
| arn                              | String             | &cross;      |
| attributes                       | Map<String,List>   | &check;      |
| availabilityZone                 | String             | &check;      |
| dbInstanceIdentifier             | String             | &check;      |
| dbiResourceId                    | String             | &check;      |
| encrypted                        | Boolean            | &check;      |
| engine                           | String             | &check;      |
| engineVersion                    | String             | &check;      |
| iamDatabaseAuthenticationEnabled | Boolean            | &check;      |
| id                               | String             | &cross;      |
| instanceCreateTime               | String             | &check;      |
| iops                             | Int                | &check;      |
| kmsKeyId                         | String             | &check;      |
| licenseModel                     | String             | &check;      |
| masterUsername                   | String             | &check;      |
| optionGroupName                  | String             | &check;      |
| originalSnapshotCreateTime       | String             | &check;      |
| percentProgress                  | Int                | &check;      |
| port                             | Int                | &check;      |
| processorFeatures                | Map<String,String> | &check;      |
| region                           | String             | &cross;      |
| snapshotCreateTime               | String             | &check;      |
| snapshotTarget                   | String             | &check;      |
| snapshotType                     | String             | &check;      |
| sourceDBSnapshotIdentifier       | String             | &check;      |
| sourceRegion                     | String             | &check;      |
| status                           | String             | &check;      |
| storageType                      | String             | &check;      |
| tagList                          | Map<String,String> | &check;      |
| tdeCredentialArn                 | String             | &check;      |
| timezone                         | String             | &check;      |
| vpcId                            | String             | &check;      |
