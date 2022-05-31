---
description: New Relic Account
---
newrelic_account
----------------

| **Name**            | **Type**                         | **Nullable** |
| ------------------- | -------------------------------- | ------------ |
| agentConfiguration  | AgentConfiguration               | &check;      |
| id                  | Int                              | &cross;      |
| linkedAccounts      | List<LinkedAccountConfiguration> | &check;      |
| logConfiguration    | LogConfiguration                 | &check;      |
| name                | String                           | &cross;      |
| reportingEventTypes | List<String>                     | &check;      |

#### AgentConfiguration
| **Name**                | **Type**               | **Nullable** |
| ----------------------- | ---------------------- | ------------ |
| agentSettingsAttributes | List<AttributeSetting> | &check;      |
| environmentAttributes   | List<AttributeSetting> | &check;      |
| modules                 | List<ModuleSetting>    | &check;      |

#### Attribute
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| attribute | String   | &cross;      |
| value     | String   | &cross;      |

#### AttributeSetting
| **Name**         | **Type**        | **Nullable** |
| ---------------- | --------------- | ------------ |
| applicationGuids | List<String>    | &cross;      |
| attributes       | List<Attribute> | &cross;      |
| details          | Detail          | &cross;      |

#### DataPartitionRuleConfiguration
| **Name**            | **Type**                                        | **Nullable** |
| ------------------- | ----------------------------------------------- | ------------ |
| createdAt           | String                                          | &check;      |
| createdBy           | Int                                             | &check;      |
| deleted             | Boolean                                         | &cross;      |
| description         | String                                          | &check;      |
| enabled             | Boolean                                         | &cross;      |
| id                  | String                                          | &cross;      |
| matchingCriteria    | DataPartitionRuleConfiguration.MatchingCriteria | &cross;      |
| retentionPolicy     | String                                          | &cross;      |
| targetDataPartition | String                                          | &cross;      |
| updatedAt           | String                                          | &check;      |
| updatedBy           | Int                                             | &check;      |

#### DataPartitionRuleConfiguration.MatchingCriteria
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| attributeName      | String   | &cross;      |
| matchingExpression | String   | &cross;      |
| matchingOperator   | String   | &cross;      |

#### Detail
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| host     | String   | &cross;      |
| id       | String   | &cross;      |
| language | String   | &cross;      |
| name     | String   | &cross;      |

#### LinkedAccountConfiguration
| **Name**             | **Type**                                     | **Nullable** |
| -------------------- | -------------------------------------------- | ------------ |
| authLabel            | String                                       | &check;      |
| createdAt            | Date                                         | &check;      |
| disabled             | Boolean                                      | &cross;      |
| externalId           | String                                       | &cross;      |
| id                   | Int                                          | &check;      |
| integrations         | List<LinkedAccountConfiguration.Integration> | &check;      |
| metricCollectionMode | String                                       | &check;      |
| name                 | String                                       | &check;      |
| nrAccountId          | Int                                          | &check;      |
| updatedAt            | Date                                         | &check;      |

#### LinkedAccountConfiguration.Integration
| **Name**  | **Type**                                       | **Nullable** |
| --------- | ---------------------------------------------- | ------------ |
| createdAt | Date                                           | &check;      |
| id        | Int                                            | &cross;      |
| name      | String                                         | &cross;      |
| service   | LinkedAccountConfiguration.Integration.Service | &cross;      |

#### LinkedAccountConfiguration.Integration.Service
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| createdAt | Date     | &check;      |
| id        | Int      | &check;      |
| isEnabled | Boolean  | &check;      |
| name      | String   | &check;      |
| slug      | String   | &check;      |
| updatedAt | Date     | &check;      |

#### LogConfiguration
| **Name**              | **Type**                             | **Nullable** |
| --------------------- | ------------------------------------ | ------------ |
| dataPartitionRules    | List<DataPartitionRuleConfiguration> | &check;      |
| parsingRules          | List<ParsingRuleConfiguration>       | &check;      |
| pipelineConfiguration | PipelineConfiguration                | &check;      |

#### ModuleSetting
| **Name**   | **Type**        | **Nullable** |
| ---------- | --------------- | ------------ |
| attributes | List<Attribute> | &cross;      |
| name       | String          | &cross;      |
| version    | String          | &check;      |

#### ParsingRuleConfiguration
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| accountId   | Int      | &cross;      |
| createdBy   | Int      | &check;      |
| deleted     | Boolean  | &cross;      |
| description | String   | &cross;      |
| enabled     | Boolean  | &cross;      |
| grok        | String   | &cross;      |
| id          | String   | &cross;      |
| lucene      | String   | &cross;      |
| nrql        | String   | &cross;      |
| updatedAt   | String   | &check;      |
| updatedBy   | Int      | &check;      |

#### PipelineConfiguration
| **Name**                     | **Type** | **Nullable** |
| ---------------------------- | -------- | ------------ |
| accountId                    | Int      | &cross;      |
| enrichmentDisabled           | Boolean  | &cross;      |
| jsonParsingDisabled          | Boolean  | &cross;      |
| obfuscationDisabled          | Boolean  | &cross;      |
| parsingDisabled              | Boolean  | &cross;      |
| patternsEnabled              | Boolean  | &cross;      |
| recursiveJsonParsingDisabled | Boolean  | &cross;      |
| transformationDisabled       | Boolean  | &cross;      |
| updatedAt                    | String   | &check;      |
| updatedBy                    | Int      | &check;      |
