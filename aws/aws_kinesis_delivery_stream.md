---
description: Amazon Web Services Kinesis Delivery Stream
---
aws_kinesis_delivery_stream
---------------------------

| **Name**                              | **Type**                              | **Nullable** |
| ------------------------------------- | ------------------------------------- | ------------ |
| accountId                             | String                                | &cross;      |
| createTimestamp                       | String                                | &check;      |
| deliveryStreamARN                     | String                                | &cross;      |
| deliveryStreamEncryptionConfiguration | DeliveryStreamEncryptionConfiguration | &check;      |
| deliveryStreamName                    | String                                | &check;      |
| deliveryStreamStatus                  | String                                | &check;      |
| deliveryStreamType                    | String                                | &check;      |
| destinations                          | List<DestinationDescription>          | &check;      |
| failureDescription                    | FailureDescription                    | &check;      |
| hasMoreDestinations                   | Boolean                               | &check;      |
| lastUpdateTimestamp                   | String                                | &check;      |
| region                                | String                                | &cross;      |
| source                                | SourceDescription                     | &check;      |
| versionId                             | String                                | &check;      |

#### AmazonopensearchserviceBufferingHints
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| intervalInSeconds | Int      | &check;      |
| sizeInMBs         | Int      | &check;      |

#### AmazonopensearchserviceDestinationDescription
| **Name**                    | **Type**                              | **Nullable** |
| --------------------------- | ------------------------------------- | ------------ |
| bufferingHints              | AmazonopensearchserviceBufferingHints | &check;      |
| cloudWatchLoggingOptions    | CloudWatchLoggingOptions              | &check;      |
| clusterEndpoint             | String                                | &check;      |
| domainARN                   | String                                | &check;      |
| indexName                   | String                                | &check;      |
| indexRotationPeriod         | String                                | &check;      |
| processingConfiguration     | ProcessingConfiguration               | &check;      |
| retryOptions                | AmazonopensearchserviceRetryOptions   | &check;      |
| roleARN                     | String                                | &check;      |
| s3BackupMode                | String                                | &check;      |
| s3DestinationDescription    | S3DestinationDescription              | &check;      |
| typeName                    | String                                | &check;      |
| vpcConfigurationDescription | VpcConfigurationDescription           | &check;      |

#### AmazonopensearchserviceRetryOptions
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| durationInSeconds | Int      | &check;      |

#### BufferingHints
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| intervalInSeconds | Int      | &check;      |
| sizeInMBs         | Int      | &check;      |

#### CloudWatchLoggingOptions
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| enabled       | Boolean  | &check;      |
| logGroupName  | String   | &check;      |
| logStreamName | String   | &check;      |

#### CopyCommand
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| copyOptions      | String   | &check;      |
| dataTableColumns | String   | &check;      |
| dataTableName    | String   | &check;      |

#### DeliveryStreamEncryptionConfiguration
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| failureDescription | FailureDescription | &check;      |
| keyARN             | String             | &check;      |
| keyType            | String             | &check;      |
| status             | String             | &check;      |

#### DestinationDescription
| **Name**                                      | **Type**                                      | **Nullable** |
| --------------------------------------------- | --------------------------------------------- | ------------ |
| amazonopensearchserviceDestinationDescription | AmazonopensearchserviceDestinationDescription | &check;      |
| destinationId                                 | String                                        | &check;      |
| elasticsearchDestinationDescription           | ElasticsearchDestinationDescription           | &check;      |
| extendedS3DestinationDescription              | ExtendedS3DestinationDescription              | &check;      |
| httpEndpointDestinationDescription            | HttpEndpointDestinationDescription            | &check;      |
| redshiftDestinationDescription                | RedshiftDestinationDescription                | &check;      |
| s3DestinationDescription                      | S3DestinationDescription                      | &check;      |
| splunkDestinationDescription                  | SplunkDestinationDescription                  | &check;      |

#### DynamicPartitioningConfiguration
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| enabled      | Boolean      | &check;      |
| retryOptions | RetryOptions | &check;      |

#### ElasticsearchBufferingHints
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| intervalInSeconds | Int      | &check;      |
| sizeInMBs         | Int      | &check;      |

#### ElasticsearchDestinationDescription
| **Name**                    | **Type**                    | **Nullable** |
| --------------------------- | --------------------------- | ------------ |
| bufferingHints              | ElasticsearchBufferingHints | &check;      |
| cloudWatchLoggingOptions    | CloudWatchLoggingOptions    | &check;      |
| clusterEndpoint             | String                      | &check;      |
| domainARN                   | String                      | &check;      |
| indexName                   | String                      | &check;      |
| indexRotationPeriod         | String                      | &check;      |
| processingConfiguration     | ProcessingConfiguration     | &check;      |
| retryOptions                | ElasticsearchRetryOptions   | &check;      |
| roleARN                     | String                      | &check;      |
| s3BackupMode                | String                      | &check;      |
| s3DestinationDescription    | S3DestinationDescription    | &check;      |
| typeName                    | String                      | &check;      |
| vpcConfigurationDescription | VpcConfigurationDescription | &check;      |

#### ElasticsearchRetryOptions
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| durationInSeconds | Int      | &check;      |

#### EncryptionConfiguration
| **Name**            | **Type**            | **Nullable** |
| ------------------- | ------------------- | ------------ |
| kmsEncryptionConfig | KMSEncryptionConfig | &check;      |
| noEncryptionConfig  | String              | &check;      |

#### ExtendedS3DestinationDescription
| **Name**                          | **Type**                         | **Nullable** |
| --------------------------------- | -------------------------------- | ------------ |
| bucketARN                         | String                           | &check;      |
| bufferingHints                    | BufferingHints                   | &check;      |
| cloudWatchLoggingOptions          | CloudWatchLoggingOptions         | &check;      |
| compressionFormat                 | String                           | &check;      |
| dataFormatConversionConfiguration | JSON                             | &check;      |
| dynamicPartitioningConfiguration  | DynamicPartitioningConfiguration | &check;      |
| encryptionConfiguration           | EncryptionConfiguration          | &check;      |
| errorOutputPrefix                 | String                           | &check;      |
| prefix                            | String                           | &check;      |
| processingConfiguration           | ProcessingConfiguration          | &check;      |
| roleARN                           | String                           | &check;      |
| s3BackupDescription               | S3DestinationDescription         | &check;      |
| s3BackupMode                      | String                           | &check;      |

#### FailureDescription
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| details  | String   | &check;      |
| type     | String   | &check;      |

#### HttpEndpointBufferingHints
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| intervalInSeconds | Int      | &check;      |
| sizeInMBs         | Int      | &check;      |

#### HttpEndpointCommonAttribute
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| attributeName  | String   | &check;      |
| attributeValue | String   | &check;      |

#### HttpEndpointDescription
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| url      | String   | &check;      |

#### HttpEndpointDestinationDescription
| **Name**                 | **Type**                         | **Nullable** |
| ------------------------ | -------------------------------- | ------------ |
| bufferingHints           | HttpEndpointBufferingHints       | &check;      |
| cloudWatchLoggingOptions | CloudWatchLoggingOptions         | &check;      |
| endpointConfiguration    | HttpEndpointDescription          | &check;      |
| processingConfiguration  | ProcessingConfiguration          | &check;      |
| requestConfiguration     | HttpEndpointRequestConfiguration | &check;      |
| retryOptions             | HttpEndpointRetryOptions         | &check;      |
| roleARN                  | String                           | &check;      |
| s3BackupMode             | String                           | &check;      |
| s3DestinationDescription | S3DestinationDescription         | &check;      |

#### HttpEndpointRequestConfiguration
| **Name**         | **Type**                          | **Nullable** |
| ---------------- | --------------------------------- | ------------ |
| commonAttributes | List<HttpEndpointCommonAttribute> | &check;      |
| contentEncoding  | String                            | &check;      |

#### HttpEndpointRetryOptions
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| durationInSeconds | Int      | &check;      |

#### KMSEncryptionConfig
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| awskmsKeyARN | String   | &check;      |

#### KinesisStreamSourceDescription
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| deliveryStartTimestamp | String   | &check;      |
| kinesisStreamARN       | String   | &check;      |
| roleARN                | String   | &check;      |

#### ProcessingConfiguration
| **Name**   | **Type**        | **Nullable** |
| ---------- | --------------- | ------------ |
| enabled    | Boolean         | &check;      |
| processors | List<Processor> | &check;      |

#### Processor
| **Name**   | **Type**                 | **Nullable** |
| ---------- | ------------------------ | ------------ |
| parameters | List<ProcessorParameter> | &check;      |
| type       | String                   | &check;      |

#### ProcessorParameter
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| parameterName  | String   | &check;      |
| parameterValue | String   | &check;      |

#### RedshiftDestinationDescription
| **Name**                 | **Type**                 | **Nullable** |
| ------------------------ | ------------------------ | ------------ |
| cloudWatchLoggingOptions | CloudWatchLoggingOptions | &check;      |
| clusterJDBCURL           | String                   | &check;      |
| copyCommand              | CopyCommand              | &check;      |
| processingConfiguration  | ProcessingConfiguration  | &check;      |
| retryOptions             | RedshiftRetryOptions     | &check;      |
| roleARN                  | String                   | &check;      |
| s3BackupDescription      | S3DestinationDescription | &check;      |
| s3BackupMode             | String                   | &check;      |
| s3DestinationDescription | S3DestinationDescription | &check;      |
| username                 | String                   | &check;      |

#### RedshiftRetryOptions
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| durationInSeconds | Int      | &check;      |

#### RetryOptions
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| durationInSeconds | Int      | &check;      |

#### S3DestinationDescription
| **Name**                 | **Type**                 | **Nullable** |
| ------------------------ | ------------------------ | ------------ |
| bucketARN                | String                   | &check;      |
| bufferingHints           | BufferingHints           | &check;      |
| cloudWatchLoggingOptions | CloudWatchLoggingOptions | &check;      |
| encryptionConfiguration  | EncryptionConfiguration  | &check;      |
| errorOutputPrefix        | String                   | &check;      |
| prefix                   | String                   | &check;      |
| roleARN                  | String                   | &check;      |

#### SourceDescription
| **Name**                       | **Type**                       | **Nullable** |
| ------------------------------ | ------------------------------ | ------------ |
| kinesisStreamSourceDescription | KinesisStreamSourceDescription | &check;      |

#### SplunkDestinationDescription
| **Name**                          | **Type**                 | **Nullable** |
| --------------------------------- | ------------------------ | ------------ |
| cloudWatchLoggingOptions          | CloudWatchLoggingOptions | &check;      |
| hecAcknowledgmentTimeoutInSeconds | String                   | &check;      |
| hecEndpoint                       | String                   | &check;      |
| hecEndpointType                   | String                   | &check;      |
| hecToken                          | String                   | &check;      |
| processingConfiguration           | ProcessingConfiguration  | &check;      |
| retryOptions                      | SplunkRetryOptions       | &check;      |
| s3BackupMode                      | String                   | &check;      |
| s3DestinationDescription          | S3DestinationDescription | &check;      |

#### SplunkRetryOptions
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| durationInSeconds | Int      | &check;      |

#### VpcConfigurationDescription
| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| roleARN          | String       | &check;      |
| securityGroupIds | List<String> | &check;      |
| subnetIds        | List<String> | &check;      |
| vpcId            | String       | &check;      |
