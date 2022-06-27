---
description: Amazon Web Services EFS File System
---
aws_efs_file_system
-------------------

| **Name**                     | **Type**           | **Nullable** |
| ---------------------------- | ------------------ | ------------ |
| accountId                    | String             | &cross;      |
| availabilityZoneId           | String             | &check;      |
| availabilityZoneName         | String             | &check;      |
| creationTime                 | String             | &check;      |
| creationToken                | String             | &check;      |
| encrypted                    | Boolean            | &check;      |
| fileSystemArn                | String             | &check;      |
| fileSystemId                 | String             | &cross;      |
| kmsKeyId                     | String             | &check;      |
| lifeCycleState               | String             | &check;      |
| name                         | String             | &check;      |
| numberOfMountTargets         | Int                | &check;      |
| ownerId                      | String             | &check;      |
| performanceMode              | String             | &check;      |
| policy                       | JSON               | &check;      |
| provisionedThroughputInMibps | Double             | &check;      |
| region                       | String             | &cross;      |
| tags                         | Map<String,String> | &check;      |
| throughputMode               | String             | &check;      |
