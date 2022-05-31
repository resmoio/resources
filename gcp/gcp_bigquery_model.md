---
description: Google Cloud Platform BigQuery Model
---
gcp_bigquery_model
------------------

| **Name**                | **Type**                | **Nullable** |
| ----------------------- | ----------------------- | ------------ |
| creationTime            | Long                    | &check;      |
| description             | String                  | &check;      |
| encryptionConfiguration | EncryptionConfiguration | &check;      |
| expirationTime          | Long                    | &check;      |
| featureColumnList       | List<StandardSQLField>  | &check;      |
| friendlyName            | String                  | &check;      |
| labelColumnList         | List<StandardSQLField>  | &check;      |
| labels                  | Map<String,String>      | &check;      |
| lastModifiedTime        | Long                    | &check;      |
| location                | String                  | &check;      |
| modelId                 | ModelId                 | &cross;      |
| modelType               | String                  | &check;      |
| project                 | String                  | &cross;      |
| trainingRunList         | List<TrainingRun>       | &check;      |

#### EncryptionConfiguration
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| kmsKeyName | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### ModelId
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| dataset  | String   | &cross;      |
| model    | String   | &cross;      |
| project  | String   | &cross;      |

#### StandardSQLField
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| dataType | JSON     | &check;      |
| name     | String   | &check;      |

#### TrainingRun
| **Name**          | **Type**                          | **Nullable** |
| ----------------- | --------------------------------- | ------------ |
| dataSplitResult   | TrainingRun.DataSplitResult       | &check;      |
| evaluationMetrics | JSON                              | &check;      |
| results           | List<TrainingRun.IterationResult> | &check;      |
| startTime         | String                            | &check;      |
| trainingOptions   | TrainingRun.TrainingOptions       | &check;      |

#### TrainingRun.DataSplitResult
| **Name**        | **Type**                                   | **Nullable** |
| --------------- | ------------------------------------------ | ------------ |
| evaluationTable | TrainingRun.DataSplitResult.TableReference | &check;      |
| trainingTable   | TrainingRun.DataSplitResult.TableReference | &check;      |

#### TrainingRun.DataSplitResult.TableReference
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| datasetId | String   | &check;      |
| projectId | String   | &check;      |
| tableId   | String   | &check;      |

#### TrainingRun.IterationResult
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| durationMs   | Long     | &check;      |
| evalLoss     | Double   | &check;      |
| index        | Int      | &check;      |
| learnRate    | Double   | &check;      |
| trainingLoss | Double   | &check;      |

#### TrainingRun.TrainingOptions
| **Name**                   | **Type**           | **Nullable** |
| -------------------------- | ------------------ | ------------ |
| adjustStepChanges          | Boolean            | &check;      |
| autoArima                  | Boolean            | &check;      |
| autoArimaMaxOrder          | Long               | &check;      |
| batchSize                  | Long               | &check;      |
| boosterType                | String             | &check;      |
| cleanSpikesAndDips         | Boolean            | &check;      |
| colsampleBylevel           | Double             | &check;      |
| colsampleBynode            | Double             | &check;      |
| colsampleBytree            | Double             | &check;      |
| dartNormalizeType          | String             | &check;      |
| dataFrequency              | String             | &check;      |
| dataSplitColumn            | String             | &check;      |
| dataSplitEvalFraction      | Double             | &check;      |
| dataSplitMethod            | String             | &check;      |
| decomposeTimeSeries        | Boolean            | &check;      |
| distanceType               | String             | &check;      |
| dropout                    | Double             | &check;      |
| earlyStop                  | Boolean            | &check;      |
| feedbackType               | String             | &check;      |
| hiddenUnits                | List<Long>         | &check;      |
| holidayRegion              | String             | &check;      |
| horizon                    | Long               | &check;      |
| includeDrift               | Boolean            | &check;      |
| initialLearnRate           | Double             | &check;      |
| inputLabelColumns          | List<String>       | &check;      |
| itemColumn                 | String             | &check;      |
| kmeansInitializationColumn | String             | &check;      |
| kmeansInitializationMethod | String             | &check;      |
| l1Regularization           | Double             | &check;      |
| l2Regularization           | Double             | &check;      |
| labelClassWeights          | Map<String,Double> | &check;      |
| learnRate                  | Double             | &check;      |
| learnRateStrategy          | String             | &check;      |
| lossType                   | String             | &check;      |
| maxIterations              | Long               | &check;      |
| maxTreeDepth               | Long               | &check;      |
| minRelativeProgress        | Double             | &check;      |
| minSplitLoss               | Double             | &check;      |
| minTreeChildWeight         | Long               | &check;      |
| modelUri                   | String             | &check;      |
| numClusters                | Long               | &check;      |
| numFactors                 | Long               | &check;      |
| numParallelTree            | Long               | &check;      |
| optimizationStrategy       | String             | &check;      |
| preserveInputStructs       | Boolean            | &check;      |
| subsample                  | Double             | &check;      |
| timeSeriesDataColumn       | String             | &check;      |
| timeSeriesIdColumn         | String             | &check;      |
| timeSeriesIdColumns        | List<String>       | &check;      |
| timeSeriesTimestampColumn  | String             | &check;      |
| treeMethod                 | String             | &check;      |
| userColumn                 | String             | &check;      |
| walsAlpha                  | Double             | &check;      |
| warmStart                  | Boolean            | &check;      |
