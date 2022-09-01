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
| logging                        | LoggingEnabled            | &check;      |
| mfaDelete                      | String                    | &check;      |
| name                           | String                    | &cross;      |
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

#### ResourceCustomComparable
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |

