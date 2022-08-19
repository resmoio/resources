---
description: Amazon Web Services EFS Access Point
---
aws_efs_access_point
--------------------

| **Name**       | **Type**           | **Nullable** |
| -------------- | ------------------ | ------------ |
| accessPointArn | String             | &check;      |
| accessPointId  | String             | &cross;      |
| accountId      | String             | &cross;      |
| accountName    | String             | &check;      |
| clientToken    | String             | &check;      |
| fileSystemId   | String             | &check;      |
| lifeCycleState | String             | &check;      |
| name           | String             | &check;      |
| ownerId        | String             | &check;      |
| posixUser      | PosixUser          | &check;      |
| region         | String             | &cross;      |
| rootDirectory  | RootDirectory      | &check;      |
| tags           | Map<String,String> | &check;      |

#### PosixUser
| **Name**      | **Type**   | **Nullable** |
| ------------- | ---------- | ------------ |
| gid           | Long       | &check;      |
| secondaryGids | List<Long> | &check;      |
| uid           | Long       | &check;      |

#### RootDirectory
| **Name**     | **Type**                   | **Nullable** |
| ------------ | -------------------------- | ------------ |
| creationInfo | RootDirectory.CreationInfo | &check;      |
| path         | String                     | &check;      |

#### RootDirectory.CreationInfo
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| ownerGid    | Long     | &check;      |
| ownerUid    | Long     | &check;      |
| permissions | String   | &check;      |
