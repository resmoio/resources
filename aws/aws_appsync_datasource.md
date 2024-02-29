---
description: Amazon Web Services AppSync Datasource
---
aws_appsync_datasource
----------------------

| **Name**                 | **Type**                           | **Nullable** |
| ------------------------ | ---------------------------------- | ------------ |
| accountId                | String                             | &cross;      |
| accountName              | String                             | &check;      |
| apiId                    | String                             | &cross;      |
| dataSourceArn            | String                             | &cross;      |
| description              | String                             | &check;      |
| dynamodbConfig           | DynamodbDataSourceConfig           | &check;      |
| elasticsearchConfig      | ElasticsearchDataSourceConfig      | &check;      |
| eventBridgeConfig        | EventBridgeDataSourceConfig        | &check;      |
| httpConfig               | HttpDataSourceConfig               | &check;      |
| lambdaConfig             | LambdaDataSourceConfig             | &check;      |
| name                     | String                             | &check;      |
| openSearchServiceConfig  | OpenSearchServiceDataSourceConfig  | &check;      |
| region                   | String                             | &cross;      |
| relationalDatabaseConfig | RelationalDatabaseDataSourceConfig | &check;      |
| serviceRoleArn           | String                             | &check;      |
| type                     | String                             | &check;      |

#### AuthorizationConfig
| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| authorizationType | String       | &check;      |
| awsIamConfig      | AwsIamConfig | &check;      |

#### AwsIamConfig
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| signingRegion      | String   | &check;      |
| signingServiceName | String   | &check;      |

#### DeltaSyncConfig
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| baseTableTTL       | Long     | &check;      |
| deltaSyncTableName | String   | &check;      |
| deltaSyncTableTTL  | Long     | &check;      |

#### DynamodbDataSourceConfig
| **Name**             | **Type**        | **Nullable** |
| -------------------- | --------------- | ------------ |
| awsRegion            | String          | &check;      |
| deltaSyncConfig      | DeltaSyncConfig | &check;      |
| tableName            | String          | &check;      |
| useCallerCredentials | Boolean         | &check;      |
| versioned            | Boolean         | &check;      |

#### ElasticsearchDataSourceConfig
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| awsRegion | String   | &check;      |
| endpoint  | String   | &check;      |

#### EventBridgeDataSourceConfig
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| eventBusArn | String   | &check;      |

#### HttpDataSourceConfig
| **Name**            | **Type**            | **Nullable** |
| ------------------- | ------------------- | ------------ |
| authorizationConfig | AuthorizationConfig | &check;      |
| endpoint            | String              | &check;      |

#### LambdaDataSourceConfig
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| lambdaFunctionArn | String   | &check;      |

#### OpenSearchServiceDataSourceConfig
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| awsRegion | String   | &check;      |
| endpoint  | String   | &check;      |

#### RdsHttpEndpointConfig
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| awsRegion           | String   | &check;      |
| awsSecretStoreArn   | String   | &check;      |
| databaseName        | String   | &check;      |
| dbClusterIdentifier | String   | &check;      |
| schema              | String   | &check;      |

#### RelationalDatabaseDataSourceConfig
| **Name**                     | **Type**              | **Nullable** |
| ---------------------------- | --------------------- | ------------ |
| rdsHttpEndpointConfig        | RdsHttpEndpointConfig | &check;      |
| relationalDatabaseSourceType | String                | &check;      |
