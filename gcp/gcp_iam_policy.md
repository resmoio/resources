---
description: Google Cloud Platform IAM Policy
---
gcp_iam_policy
--------------

| **Name**     | **Type**          | **Nullable** |
| ------------ | ----------------- | ------------ |
| auditConfigs | List<AuditConfig> | &check;      |
| bindings     | List<Binding>     | &check;      |
| project      | String            | &cross;      |
| version      | Int               | &check;      |

#### AuditConfig
| **Name**        | **Type**             | **Nullable** |
| --------------- | -------------------- | ------------ |
| auditLogConfigs | List<AuditLogConfig> | &check;      |
| service         | String               | &check;      |

#### AuditLogConfig
| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| exemptedMembers | List<String> | &check;      |
| logType         | String       | &check;      |

#### Binding
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| condition | Expr         | &check;      |
| members   | List<String> | &check;      |
| role      | String       | &check;      |

#### Expr
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| expression  | String   | &check;      |
| location    | String   | &check;      |
| title       | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
