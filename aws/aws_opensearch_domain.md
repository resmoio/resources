---
description: Amazon Web Services OpenSearch Domain
---
aws_opensearch_domain
---------------------

| **Name**                    | **Type**                        | **Nullable** |
| --------------------------- | ------------------------------- | ------------ |
| accessPolicies              | JSON                            | &check;      |
| accountId                   | String                          | &cross;      |
| advancedOptions             | Map<String,String>              | &check;      |
| advancedSecurityOptions     | AdvancedSecurityOptions         | &check;      |
| arn                         | String                          | &cross;      |
| associatedPackages          | List<AssociatedPackage>         | &check;      |
| autoTuneOptions             | AutoTuneOptionsOutput           | &check;      |
| clusterConfig               | ClusterConfig                   | &check;      |
| cognitoOptions              | CognitoOptions                  | &cross;      |
| created                     | Boolean                         | &cross;      |
| deleted                     | Boolean                         | &cross;      |
| domainEndpointOptions       | DomainEndpointOptions           | &check;      |
| domainId                    | String                          | &cross;      |
| domainName                  | String                          | &cross;      |
| ebsOptions                  | EBSOptions                      | &check;      |
| encryptionAtRestOptions     | EncryptionAtRestOptions         | &check;      |
| endpoint                    | String                          | &check;      |
| endpoints                   | Map<String,String>              | &cross;      |
| engineVersion               | String                          | &cross;      |
| logPublishingOptions        | Map<String,LogPublishingOption> | &cross;      |
| nodeToNodeEncryptionOptions | NodeToNodeEncryptionOptions     | &check;      |
| processing                  | Boolean                         | &cross;      |
| region                      | String                          | &cross;      |
| serviceSoftwareOptions      | ServiceSoftwareOptions          | &check;      |
| snapshotOptions             | SnapshotOptions                 | &check;      |
| tags                        | Map<String,String>              | &cross;      |
| upgradeProcessing           | Boolean                         | &cross;      |
| vpcOptions                  | VPCDerivedInfo                  | &check;      |

#### AdvancedSecurityOptions
| **Name**                    | **Type**                                  | **Nullable** |
| --------------------------- | ----------------------------------------- | ------------ |
| enabled                     | Boolean                                   | &check;      |
| internalUserDatabaseEnabled | Boolean                                   | &check;      |
| samlOptions                 | AdvancedSecurityOptions.SAMLOptionsOutput | &check;      |

#### AdvancedSecurityOptions.SAMLOptionsOutput
| **Name**              | **Type**                                          | **Nullable** |
| --------------------- | ------------------------------------------------- | ------------ |
| enabled               | Boolean                                           | &check;      |
| idp                   | AdvancedSecurityOptions.SAMLOptionsOutput.SAMLIdp | &check;      |
| rolesKey              | String                                            | &check;      |
| sessionTimeoutMinutes | Int                                               | &check;      |
| subjectKey            | String                                            | &check;      |

#### AdvancedSecurityOptions.SAMLOptionsOutput.SAMLIdp
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| entityId        | String   | &check;      |
| metadataContent | String   | &check;      |

#### AssociatedPackage
| **Name**            | **Type**                       | **Nullable** |
| ------------------- | ------------------------------ | ------------ |
| domainPackageStatus | String                         | &check;      |
| errorDetails        | AssociatedPackage.ErrorDetails | &check;      |
| lastUpdated         | String                         | &check;      |
| packageId           | String                         | &check;      |
| packageType         | String                         | &check;      |
| packageVersion      | String                         | &cross;      |
| referencePath       | String                         | &check;      |

#### AssociatedPackage.ErrorDetails
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| message  | String   | &check;      |
| type     | String   | &check;      |

#### AutoTuneOptionsOutput
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| errorMessage | String   | &check;      |
| state        | String   | &cross;      |

#### ClusterConfig
| **Name**               | **Type**                          | **Nullable** |
| ---------------------- | --------------------------------- | ------------ |
| coldStorageOptions     | ClusterConfig.ColdStorageOptions  | &cross;      |
| dedicatedMasterCount   | Int                               | &check;      |
| dedicatedMasterEnabled | Boolean                           | &cross;      |
| dedicatedMasterType    | String                            | &check;      |
| instanceCount          | Int                               | &cross;      |
| instanceType           | String                            | &cross;      |
| warmCount              | Int                               | &check;      |
| warmEnabled            | Boolean                           | &cross;      |
| warmType               | String                            | &check;      |
| zoneAwarenessConfig    | ClusterConfig.ZoneAwarenessConfig | &check;      |
| zoneAwarenessEnabled   | Boolean                           | &cross;      |

#### ClusterConfig.ColdStorageOptions
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &cross;      |

#### ClusterConfig.ZoneAwarenessConfig
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| availabilityZoneCount | Int      | &cross;      |

#### CognitoOptions
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| enabled        | Boolean  | &cross;      |
| identityPoolId | String   | &check;      |
| roleArn        | String   | &check;      |
| userPoolId     | String   | &check;      |

#### DomainEndpointOptions
| **Name**                     | **Type** | **Nullable** |
| ---------------------------- | -------- | ------------ |
| customEndpoint               | String   | &check;      |
| customEndpointCertificateArn | String   | &check;      |
| customEndpointEnabled        | Boolean  | &check;      |
| enforceHTTPS                 | Boolean  | &check;      |
| tlsSecurityPolicy            | String   | &check;      |

#### EBSOptions
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| ebsEnabled | Boolean  | &cross;      |
| iops       | Int      | &check;      |
| volumeSize | Int      | &cross;      |
| volumeType | String   | &cross;      |

#### EncryptionAtRestOptions
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |
| kmsKeyId | String   | &check;      |

#### LogPublishingOption
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| cloudWatchLogsLogGroupArn | String   | &check;      |
| enabled                   | Boolean  | &cross;      |

#### NodeToNodeEncryptionOptions
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &cross;      |

#### ServiceSoftwareOptions
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| automatedUpdateDate | String   | &check;      |
| cancellable         | Boolean  | &check;      |
| currentVersion      | String   | &check;      |
| description         | String   | &check;      |
| newVersion          | String   | &check;      |
| optionalDeployment  | Boolean  | &check;      |
| updateAvailable     | Boolean  | &check;      |
| updateStatus        | String   | &check;      |

#### SnapshotOptions
| **Name**                   | **Type** | **Nullable** |
| -------------------------- | -------- | ------------ |
| automatedSnapshotStartHour | Long     | &check;      |

#### VPCDerivedInfo
| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| availabilityZones | List<String> | &cross;      |
| securityGroupIds  | List<String> | &cross;      |
| subnetIds         | List<String> | &cross;      |
| vpcId             | String       | &cross;      |
