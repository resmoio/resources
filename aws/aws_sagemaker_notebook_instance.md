---
description: Amazon Web Services SageMaker Notebook Instance
---
aws_sagemaker_notebook_instance
-------------------------------

| **Name**                             | **Type**                             | **Nullable** |
| ------------------------------------ | ------------------------------------ | ------------ |
| acceleratorTypes                     | List<String>                         | &check;      |
| accountId                            | String                               | &cross;      |
| accountName                          | String                               | &check;      |
| additionalCodeRepositories           | List<String>                         | &check;      |
| creationTime                         | String                               | &check;      |
| defaultCodeRepository                | String                               | &check;      |
| directInternetAccess                 | String                               | &check;      |
| failureReason                        | String                               | &check;      |
| instanceMetadataServiceConfiguration | InstanceMetadataServiceConfiguration | &check;      |
| instanceType                         | String                               | &check;      |
| kmsKeyId                             | String                               | &check;      |
| lastModifiedTime                     | String                               | &check;      |
| networkInterfaceId                   | String                               | &check;      |
| notebookInstanceArn                  | String                               | &cross;      |
| notebookInstanceLifecycleConfigName  | String                               | &check;      |
| notebookInstanceName                 | String                               | &check;      |
| notebookInstanceStatus               | String                               | &check;      |
| platformIdentifier                   | String                               | &check;      |
| region                               | String                               | &cross;      |
| roleArn                              | String                               | &check;      |
| rootAccess                           | String                               | &check;      |
| securityGroups                       | List<String>                         | &check;      |
| subnetId                             | String                               | &check;      |
| url                                  | String                               | &check;      |
| volumeSizeInGB                       | Int                                  | &check;      |

#### InstanceMetadataServiceConfiguration
| **Name**                              | **Type** | **Nullable** |
| ------------------------------------- | -------- | ------------ |
| minimumInstanceMetadataServiceVersion | String   | &check;      |
