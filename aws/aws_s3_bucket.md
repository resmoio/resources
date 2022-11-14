---
description: Amazon Web Services S3 Bucket
---
aws_s3_bucket
-------------

| **Name**                       | **Type**                  | **Nullable** |
| ------------------------------ | ------------------------- | ------------ |
| accountId                      | String                    | &cross;      |
| accountName                    | String                    | &check;      |
| acl                            | ACL                       | &cross;      |
| creationDate                   | String                    | &cross;      |
| hostname                       | String                    | &check;      |
| kmsMasterKeyID                 | String                    | &check;      |
| lifeCycleConfig                | List<JSON>                | &check;      |
| logging                        | LoggingEnabled            | &check;      |
| mfaDelete                      | String                    | &check;      |
| name                           | String                    | &cross;      |
| notificationConfiguration      | NotificationConfiguration | &check;      |
| policy                         | JSON                      | &check;      |
| policyStatus                   | PolicyStatus              | &check;      |
| publicAccessBlockConfiguration | PublicAccessConfiguration | &check;      |
| region                         | String                    | &cross;      |
| sseAlgorithm                   | String                    | &check;      |
| tags                           | Map<String,String>        | &cross;      |
| versioning                     | String                    | &check;      |

#### ACL
| **Name** | **Type**         | **Nullable** |
| -------- | ---------------- | ------------ |
| grants   | List<ACL.Grants> | &cross;      |
| owner    | String           | &cross;      |

#### ACL.Grants
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| id         | String   | &check;      |
| permission | String   | &check;      |
| type       | String   | &check;      |
| uri        | String   | &check;      |

#### LambdaFunctionConfiguration
| **Name**          | **Type**                        | **Nullable** |
| ----------------- | ------------------------------- | ------------ |
| events            | List<String>                    | &check;      |
| filter            | NotificationConfigurationFilter | &check;      |
| id                | String                          | &check;      |
| lambdaFunctionArn | String                          | &check;      |

#### LoggingEnabled
| **Name**     | **Type**                   | **Nullable** |
| ------------ | -------------------------- | ------------ |
| targetBucket | String                     | &check;      |
| targetGrants | List<LoggingEnabled.Grant> | &cross;      |
| targetPrefix | String                     | &check;      |

#### LoggingEnabled.Grant
| **Name**   | **Type**                     | **Nullable** |
| ---------- | ---------------------------- | ------------ |
| grantee    | LoggingEnabled.Grant.Grantee | &check;      |
| permission | String                       | &check;      |

#### LoggingEnabled.Grant.Grantee
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| displayName  | String   | &check;      |
| emailAddress | String   | &check;      |
| id           | String   | &check;      |
| type         | String   | &check;      |
| uri          | String   | &check;      |

#### NotificationConfiguration
| **Name**                     | **Type**                          | **Nullable** |
| ---------------------------- | --------------------------------- | ------------ |
| eventBridgeConfiguration     | JSON                              | &check;      |
| lambdaFunctionConfigurations | List<LambdaFunctionConfiguration> | &check;      |
| queueConfigurations          | List<QueueConfiguration>          | &check;      |
| topicConfigurations          | List<TopicConfiguration>          | &check;      |

#### NotificationConfigurationFilter
| **Name** | **Type**                                    | **Nullable** |
| -------- | ------------------------------------------- | ------------ |
| key      | NotificationConfigurationFilter.S3KeyFilter | &check;      |

#### NotificationConfigurationFilter.FilterRule
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| value    | String   | &check;      |

#### NotificationConfigurationFilter.S3KeyFilter
| **Name**    | **Type**                                         | **Nullable** |
| ----------- | ------------------------------------------------ | ------------ |
| filterRules | List<NotificationConfigurationFilter.FilterRule> | &check;      |

#### PolicyStatus
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| isPublic | Boolean  | &cross;      |

#### PublicAccessConfiguration
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| blockPublicAcls       | Boolean  | &cross;      |
| blockPublicPolicy     | Boolean  | &cross;      |
| ignorePublicAcls      | Boolean  | &cross;      |
| restrictPublicBuckets | Boolean  | &cross;      |

#### QueueConfiguration
| **Name** | **Type**                        | **Nullable** |
| -------- | ------------------------------- | ------------ |
| events   | List<String>                    | &check;      |
| filter   | NotificationConfigurationFilter | &check;      |
| id       | String                          | &check;      |
| queueArn | String                          | &check;      |

#### ResourceCustomComparable
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |


#### TopicConfiguration
| **Name** | **Type**                        | **Nullable** |
| -------- | ------------------------------- | ------------ |
| events   | List<String>                    | &check;      |
| filter   | NotificationConfigurationFilter | &check;      |
| id       | String                          | &check;      |
| topicArn | String                          | &check;      |
