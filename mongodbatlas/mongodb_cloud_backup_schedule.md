---
description: MongoDB Atlas Cloud Backup Schedule
---
mongodb_cloud_backup_schedule
-----------------------------

| **Name**                          | **Type**     | **Nullable** |
| --------------------------------- | ------------ | ------------ |
| autoExportEnabled                 | Boolean      | &check;      |
| clusterId                         | String       | &cross;      |
| clusterName                       | String       | &cross;      |
| export                            | Export       | &check;      |
| links                             | List<Link>   | &cross;      |
| nextSnapshot                      | String       | &check;      |
| policies                          | List<Policy> | &cross;      |
| project                           | Project      | &cross;      |
| referenceHourOfDay                | Int          | &check;      |
| referenceMinuteOfHour             | Int          | &check;      |
| restoreWindowDays                 | Int          | &check;      |
| useOrgAndGroupNamesInExportPrefix | Boolean      | &check;      |

#### Export
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| exportBucketId | String   | &check;      |
| frequencyType  | String   | &check;      |

#### Link
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| rel      | String   | &check;      |

#### Policy
| **Name**    | **Type**         | **Nullable** |
| ----------- | ---------------- | ------------ |
| id          | String           | &check;      |
| policyItems | List<PolicyItem> | &cross;      |

#### PolicyItem
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| frequencyInterval | Int      | &check;      |
| frequencyType     | String   | &check;      |
| id                | String   | &check;      |
| retentionUnit     | String   | &check;      |
| retentionValue    | Int      | &check;      |

#### Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
