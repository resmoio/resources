---
description: Google Cloud Platform Compute Project
---
gcp_compute_project
-------------------

| **Name**               | **Type**            | **Nullable** |
| ---------------------- | ------------------- | ------------ |
| commonInstanceMetadata | Metadata            | &check;      |
| creationTimestamp      | String              | &check;      |
| defaultNetworkTier     | String              | &check;      |
| defaultServiceAccount  | String              | &check;      |
| description            | String              | &check;      |
| enabledFeatures        | List<String>        | &check;      |
| id                     | String              | &cross;      |
| kind                   | String              | &check;      |
| name                   | String              | &cross;      |
| quotas                 | List<Quota>         | &check;      |
| usageExportLocation    | UsageExportLocation | &check;      |
| xpnProjectStatus       | String              | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### Metadata
| **Name** | **Type**             | **Nullable** |
| -------- | -------------------- | ------------ |
| items    | List<Metadata.Items> | &check;      |
| kind     | String               | &check;      |

#### Metadata.Items
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| key      | String   | &check;      |
| value    | String   | &check;      |

#### Quota
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| limit    | Number   | &check;      |
| metric   | String   | &check;      |
| owner    | String   | &check;      |
| usage    | Number   | &check;      |

#### UsageExportLocation
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| bucketName       | String   | &check;      |
| reportNamePrefix | String   | &check;      |
