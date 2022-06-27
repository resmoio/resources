---
description: Amazon Web Services Glue Crawler
---
aws_glue_crawler
----------------

| **Name**                     | **Type**                   | **Nullable** |
| ---------------------------- | -------------------------- | ------------ |
| accountId                    | String                     | &cross;      |
| classifiers                  | List<String>               | &check;      |
| configuration                | String                     | &check;      |
| crawlElapsedTime             | Long                       | &check;      |
| crawlerSecurityConfiguration | String                     | &check;      |
| creationTime                 | String                     | &check;      |
| databaseName                 | String                     | &check;      |
| description                  | String                     | &check;      |
| lakeFormationConfiguration   | LakeFormationConfiguration | &check;      |
| lastCrawl                    | LastCrawlInfo              | &check;      |
| lastUpdated                  | String                     | &check;      |
| lineageConfiguration         | LineageConfiguration       | &check;      |
| name                         | String                     | &cross;      |
| recrawlPolicy                | RecrawlPolicy              | &check;      |
| region                       | String                     | &cross;      |
| role                         | String                     | &check;      |
| schedule                     | Schedule                   | &check;      |
| schemaChangePolicy           | SchemaChangePolicy         | &check;      |
| state                        | String                     | &check;      |
| tablePrefix                  | String                     | &check;      |
| targets                      | CrawlerTargets             | &check;      |
| version                      | Long                       | &check;      |

#### CatalogTarget
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| connectionName | String       | &check;      |
| databaseName   | String       | &check;      |
| tables         | List<String> | &check;      |

#### CrawlerTargets
| **Name**        | **Type**             | **Nullable** |
| --------------- | -------------------- | ------------ |
| catalogTargets  | List<CatalogTarget>  | &check;      |
| deltaTargets    | List<DeltaTarget>    | &check;      |
| dynamoDBTargets | List<DynamoDBTarget> | &check;      |
| jdbcTargets     | List<JdbcTarget>     | &check;      |
| mongoDBTargets  | List<MongoDBTarget>  | &check;      |
| s3Targets       | List<S3Target>       | &check;      |

#### DeltaTarget
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| connectionName | String       | &check;      |
| deltaTables    | List<String> | &check;      |
| writeManifest  | Boolean      | &check;      |

#### DynamoDBTarget
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| path     | String   | &check;      |
| scanAll  | Boolean  | &check;      |
| scanRate | Double   | &check;      |

#### JdbcTarget
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| connectionName | String       | &check;      |
| exclusions     | List<String> | &check;      |
| path           | String       | &check;      |

#### LakeFormationConfiguration
| **Name**                    | **Type** | **Nullable** |
| --------------------------- | -------- | ------------ |
| accountId                   | String   | &check;      |
| useLakeFormationCredentials | Boolean  | &check;      |

#### LastCrawlInfo
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| errorMessage  | String   | &check;      |
| logGroup      | String   | &check;      |
| logStream     | String   | &check;      |
| messagePrefix | String   | &check;      |
| startTime     | String   | &check;      |
| status        | String   | &check;      |

#### LineageConfiguration
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| crawlerLineageSettings | String   | &check;      |

#### MongoDBTarget
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| connectionName | String   | &check;      |
| path           | String   | &check;      |
| scanAll        | Boolean  | &check;      |

#### RecrawlPolicy
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| recrawlBehavior | String   | &check;      |

#### S3Target
| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| connectionName   | String       | &check;      |
| dlqEventQueueArn | String       | &check;      |
| eventQueueArn    | String       | &check;      |
| exclusions       | List<String> | &check;      |
| path             | String       | &check;      |
| sampleSize       | Int          | &check;      |

#### Schedule
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| scheduleExpression | String   | &check;      |
| state              | String   | &check;      |

#### SchemaChangePolicy
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| deleteBehavior | String   | &check;      |
| updateBehavior | String   | &check;      |
