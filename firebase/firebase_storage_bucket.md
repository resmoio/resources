---
description: Firebase Storage Bucket
---
firebase_storage_bucket
-----------------------

| **Name**                | **Type**            | **Nullable** |
| ----------------------- | ------------------- | ------------ |
| acl                     | List<Acl>           | &check;      |
| cors                    | List<Cors>          | &check;      |
| createTime              | Long                | &check;      |
| defaultAcl              | List<Acl>           | &check;      |
| defaultEventBasedHold   | Boolean             | &check;      |
| defaultKmsKeyName       | String              | &check;      |
| etag                    | String              | &check;      |
| generatedId             | String              | &cross;      |
| iamConfiguration        | IamConfiguration    | &check;      |
| indexPage               | String              | &check;      |
| labels                  | Map<String,String>  | &check;      |
| lifecycleRules          | List<LifecycleRule> | &check;      |
| location                | String              | &check;      |
| locationType            | String              | &check;      |
| logging                 | Logging             | &check;      |
| metageneration          | Long                | &check;      |
| name                    | String              | &cross;      |
| notFoundPage            | String              | &check;      |
| owner                   | Entity              | &check;      |
| project                 | String              | &cross;      |
| requesterPays           | Boolean             | &check;      |
| retentionEffectiveTime  | Long                | &check;      |
| retentionPeriod         | Long                | &check;      |
| retentionPolicyIsLocked | Boolean             | &check;      |
| storageClass            | StorageClass        | &check;      |
| updateTime              | Long                | &check;      |
| versioningEnabled       | Boolean             | &check;      |

#### Acl
| **Name** | **Type**   | **Nullable** |
| -------- | ---------- | ------------ |
| entity   | Acl.Entity | &check;      |
| etag     | String     | &check;      |
| id       | String     | &check;      |
| role     | Acl.Role   | &check;      |

#### Acl.Entity
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |

#### Acl.Role
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |

#### Binding
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| condition | Condition    | &check;      |
| members   | List<String> | &check;      |
| role      | String       | &check;      |

#### Condition
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| expression  | String   | &check;      |
| title       | String   | &check;      |

#### Cors
| **Name**        | **Type**              | **Nullable** |
| --------------- | --------------------- | ------------ |
| maxAgeSeconds   | Int                   | &check;      |
| methods         | List<Cors.HttpMethod> | &check;      |
| origins         | List<Cors.Origin>     | &check;      |
| responseHeaders | List<String>          | &check;      |

#### Cors.HttpMethod
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |

#### Cors.Origin
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| value    | String   | &check;      |

#### Entity
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |

#### IAMPolicy
| **Name** | **Type**      | **Nullable** |
| -------- | ------------- | ------------ |
| bindings | List<Binding> | &check;      |
| etag     | String        | &check;      |
| version  | Int           | &check;      |

#### IamConfiguration
| **Name**                           | **Type**                                | **Nullable** |
| ---------------------------------- | --------------------------------------- | ------------ |
| isUniformBucketLevelAccessEnabled  | Boolean                                 | &check;      |
| publicAccessPrevention             | IamConfiguration.PublicAccessPrevention | &check;      |
| uniformBucketLevelAccessLockedTime | Long                                    | &check;      |

#### IamConfiguration.PublicAccessPrevention
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| value    | String   | &cross;      |

#### LifecycleCondition
| **Name**                | **Type**           | **Nullable** |
| ----------------------- | ------------------ | ------------ |
| age                     | Int                | &check;      |
| createdBefore           | String             | &check;      |
| customTimeBefore        | String             | &check;      |
| daysSinceCustomTime     | Int                | &check;      |
| daysSinceNoncurrentTime | Int                | &check;      |
| isLive                  | Boolean            | &check;      |
| matchesStorageClass     | List<StorageClass> | &check;      |
| noncurrentTimeBefore    | String             | &check;      |
| numberOfNewerVersions   | Int                | &check;      |

#### LifecycleRule
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| lifecycleAction    | String             | &check;      |
| lifecycleCondition | LifecycleCondition | &check;      |

#### Logging
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| logBucket       | String   | &cross;      |
| logObjectPrefix | String   | &cross;      |

#### StorageClass
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |
