---
description: MongoDB Atlas Cluster
---
mongodb_cluster
---------------

| **Name**                 | **Type**                 | **Nullable** |
| ------------------------ | ------------------------ | ------------ |
| advancedOptions          | AdvancedOptions          | &check;      |
| autoScaling              | AutoScaling              | &check;      |
| backupEnabled            | Boolean                  | &check;      |
| biConnector              | BiConnector              | &check;      |
| clusterType              | String                   | &check;      |
| connectionStrings        | ConnectionStrings        | &check;      |
| createDate               | String                   | &check;      |
| diskSizeGB               | Double                   | &check;      |
| encryptionAtRestProvider | String                   | &check;      |
| groupId                  | String                   | &cross;      |
| id                       | String                   | &cross;      |
| labels                   | List<String>             | &cross;      |
| links                    | List<Link>               | &cross;      |
| mongoDBMajorVersion      | String                   | &check;      |
| mongoDBVersion           | String                   | &check;      |
| mongoURI                 | String                   | &check;      |
| mongoURIUpdated          | String                   | &check;      |
| mongoURIWithOptions      | String                   | &check;      |
| name                     | String                   | &cross;      |
| numShards                | Int                      | &check;      |
| paused                   | Boolean                  | &check;      |
| pitEnabled               | Boolean                  | &check;      |
| project                  | Project                  | &cross;      |
| providerBackupEnabled    | Boolean                  | &check;      |
| providerSettings         | ProviderSettings         | &check;      |
| replicationFactor        | Int                      | &check;      |
| replicationSpec          | Map<String,RegionConfig> | &check;      |
| replicationSpecs         | List<ReplicationSpec>    | &cross;      |
| rootCertType             | String                   | &check;      |
| srvAddress               | String                   | &check;      |
| stateName                | String                   | &check;      |
| versionReleaseSystem     | String                   | &check;      |

#### AdvancedOptions
| **Name**                         | **Type** | **Nullable** |
| -------------------------------- | -------- | ------------ |
| defaultReadConcern               | String   | &check;      |
| defaultWriteConcern              | String   | &check;      |
| failIndexKeyTooLong              | Boolean  | &check;      |
| javascriptEnabled                | Boolean  | &check;      |
| minimumEnabledTlsProtocol        | String   | &check;      |
| noTableScan                      | Boolean  | &check;      |
| oplogSizeMB                      | Int      | &check;      |
| sampleRefreshIntervalBIConnector | Long     | &check;      |
| sampleSizeBIConnector            | Long     | &check;      |

#### AutoScaling
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| autoIndexingEnabled | Boolean  | &check;      |
| compute             | Compute  | &check;      |
| diskGBEnabled       | Boolean  | &check;      |

#### BiConnector
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| enabled        | Boolean  | &check;      |
| readPreference | String   | &check;      |

#### Compute
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| enabled          | Boolean  | &check;      |
| maxInstanceSize  | String   | &check;      |
| minInstanceSize  | String   | &check;      |
| scaleDownEnabled | Boolean  | &check;      |

#### ConnectionStrings
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| standard    | String   | &check;      |
| standardSrv | String   | &check;      |

#### Link
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| rel      | String   | &check;      |

#### Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |

#### ProviderSettings
| **Name**            | **Type**    | **Nullable** |
| ------------------- | ----------- | ------------ |
| autoScaling         | AutoScaling | &check;      |
| backingProviderName | String      | &check;      |
| instanceSizeName    | String      | &check;      |
| providerName        | String      | &check;      |
| regionName          | String      | &check;      |

#### RegionConfig
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| analyticsNodes | Int      | &check;      |
| electableNodes | Int      | &check;      |
| priority       | Int      | &check;      |
| readOnlyNodes  | Int      | &check;      |

#### ReplicationSpec
| **Name**      | **Type**                 | **Nullable** |
| ------------- | ------------------------ | ------------ |
| id            | String                   | &check;      |
| numShards     | Int                      | &check;      |
| regionsConfig | Map<String,RegionConfig> | &check;      |
| zoneName      | String                   | &check;      |
