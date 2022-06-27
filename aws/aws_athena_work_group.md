---
description: Amazon Web Services Athena Work Group
---
aws_athena_work_group
---------------------

| **Name**      | **Type**               | **Nullable** |
| ------------- | ---------------------- | ------------ |
| accountId     | String                 | &cross;      |
| configuration | WorkGroupConfiguration | &check;      |
| creationTime  | String                 | &check;      |
| description   | String                 | &check;      |
| name          | String                 | &cross;      |
| region        | String                 | &cross;      |
| state         | String                 | &check;      |

#### WorkGroupConfiguration
| **Name**                        | **Type**                                   | **Nullable** |
| ------------------------------- | ------------------------------------------ | ------------ |
| bytesScannedCutoffPerQuery      | Long                                       | &check;      |
| enforceWorkGroupConfiguration   | Boolean                                    | &check;      |
| engineVersion                   | WorkGroupConfiguration.EngineVersion       | &check;      |
| publishCloudWatchMetricsEnabled | Boolean                                    | &check;      |
| requesterPaysEnabled            | Boolean                                    | &check;      |
| resultConfiguration             | WorkGroupConfiguration.ResultConfiguration | &check;      |

#### WorkGroupConfiguration.AclConfiguration
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| s3AclOption | String   | &check;      |

#### WorkGroupConfiguration.EncryptionConfiguration
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| encryptionOption | String   | &check;      |
| kmsKey           | String   | &check;      |

#### WorkGroupConfiguration.EngineVersion
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| effectiveEngineVersion | String   | &check;      |
| selectedEngineVersion  | String   | &check;      |

#### WorkGroupConfiguration.ResultConfiguration
| **Name**                | **Type**                                       | **Nullable** |
| ----------------------- | ---------------------------------------------- | ------------ |
| aclConfiguration        | WorkGroupConfiguration.AclConfiguration        | &check;      |
| encryptionConfiguration | WorkGroupConfiguration.EncryptionConfiguration | &check;      |
| expectedBucketOwner     | String                                         | &check;      |
| outputLocation          | String                                         | &check;      |
