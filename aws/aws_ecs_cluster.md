---
description: Amazon Web Services ECS Cluster
---
aws_ecs_cluster
---------------

| **Name**                        | **Type**                              | **Nullable** |
| ------------------------------- | ------------------------------------- | ------------ |
| accountId                       | String                                | &cross;      |
| arn                             | String                                | &cross;      |
| attachmentStatus                | String                                | &check;      |
| attachments                     | List<Attachment>                      | &cross;      |
| capacityProviders               | List<String>                          | &check;      |
| configuration                   | Configuration                         | &check;      |
| defaultCapacityProviderStrategy | List<DefaultCapacityProviderStrategy> | &cross;      |
| name                            | String                                | &cross;      |
| region                          | String                                | &cross;      |
| settings                        | Map<String,String>                    | &check;      |
| status                          | String                                | &check;      |
| tags                            | Map<String,String>                    | &cross;      |

#### Attachment
| **Name** | **Type**           | **Nullable** |
| -------- | ------------------ | ------------ |
| details  | Map<String,String> | &check;      |
| id       | String             | &check;      |
| status   | String             | &check;      |
| type     | String             | &check;      |

#### Configuration
| **Name**             | **Type**                           | **Nullable** |
| -------------------- | ---------------------------------- | ------------ |
| kmsKeyId             | String                             | &check;      |
| logging              | String                             | &check;      |
| loggingConfiguration | Configuration.LoggingConfiguration | &check;      |

#### Configuration.LoggingConfiguration
| **Name**                    | **Type** | **Nullable** |
| --------------------------- | -------- | ------------ |
| cloudWatchEncryptionEnabled | Boolean  | &check;      |
| cloudWatchLogGroupName      | String   | &check;      |
| s3BucketEncryptionEnabled   | Boolean  | &check;      |
| s3BucketName                | String   | &check;      |
| s3KeyPrefix                 | String   | &check;      |

#### DefaultCapacityProviderStrategy
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| base             | Int      | &cross;      |
| capacityProvider | String   | &cross;      |
| weight           | Int      | &cross;      |
