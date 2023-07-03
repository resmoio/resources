---
description: Amazon Web Services Lambda Event Source Mapping
---
aws_lambda_event_source_mapping
-------------------------------

| **Name**                            | **Type**                        | **Nullable** |
| ----------------------------------- | ------------------------------- | ------------ |
| accountId                           | String                          | &cross;      |
| accountName                         | String                          | &check;      |
| amazonManagedKafkaEventSourceConfig | KafkaEventSourceConfig          | &check;      |
| batchSize                           | Int                             | &check;      |
| bisectBatchOnFunctionError          | Boolean                         | &check;      |
| destinationConfig                   | DestinationConfig               | &check;      |
| eventSourceArn                      | String                          | &check;      |
| filterCriteria                      | FilterCriteria                  | &check;      |
| functionArn                         | String                          | &check;      |
| functionResponseTypes               | List<String>                    | &check;      |
| lastModified                        | String                          | &check;      |
| lastProcessingResult                | String                          | &check;      |
| maximumBatchingWindowInSeconds      | Int                             | &check;      |
| maximumRecordAgeInSeconds           | Int                             | &check;      |
| maximumRetryAttempts                | Int                             | &check;      |
| parallelizationFactor               | Int                             | &check;      |
| queues                              | List<String>                    | &check;      |
| region                              | String                          | &cross;      |
| selfManagedEventSource              | SelfManagedEventSource          | &check;      |
| selfManagedKafkaEventSourceConfig   | KafkaEventSourceConfig          | &check;      |
| sourceAccessConfigurations          | List<SourceAccessConfiguration> | &check;      |
| startingPosition                    | String                          | &check;      |
| state                               | String                          | &check;      |
| stateTransitionReason               | String                          | &check;      |
| topics                              | List<String>                    | &check;      |
| tumblingWindowInSeconds             | Int                             | &check;      |
| uuid                                | String                          | &cross;      |

#### DestinationConfig
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| onFailureDestination | String   | &check;      |
| onSuccessDestination | String   | &check;      |

#### FilterCriteria
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| filterPatterns | List<String> | &check;      |

#### KafkaEventSourceConfig
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| consumerGroupId | String   | &check;      |

#### SelfManagedEventSource
| **Name**  | **Type**         | **Nullable** |
| --------- | ---------------- | ------------ |
| endpoints | Map<String,List> | &cross;      |

#### SourceAccessConfiguration
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |
| uri      | String   | &check;      |
