---
description: Amazon Web Services EKS Addon
---
aws_eks_addon
-------------

| **Name**              | **Type**               | **Nullable** |
| --------------------- | ---------------------- | ------------ |
| accountId             | String                 | &cross;      |
| arn                   | String                 | &cross;      |
| clusterName           | String                 | &check;      |
| createdAt             | String                 | &check;      |
| health                | AddonHealth            | &check;      |
| modifiedAt            | String                 | &check;      |
| name                  | String                 | &check;      |
| region                | String                 | &cross;      |
| serviceAccountRoleArn | String                 | &check;      |
| status                | String                 | &check;      |
| tags                  | Map<String,String>     | &check;      |
| version               | String                 | &check;      |
| versions              | List<AddonVersionInfo> | &check;      |

#### AddonHealth
| **Name** | **Type**         | **Nullable** |
| -------- | ---------------- | ------------ |
| issues   | List<AddonIssue> | &check;      |

#### AddonIssue
| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| code        | String       | &check;      |
| message     | String       | &check;      |
| resourceIds | List<String> | &check;      |

#### AddonVersionInfo
| **Name**        | **Type**            | **Nullable** |
| --------------- | ------------------- | ------------ |
| addonVersion    | String              | &check;      |
| architecture    | List<String>        | &check;      |
| compatibilities | List<Compatibility> | &check;      |

#### Compatibility
| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| clusterVersion   | String       | &check;      |
| defaultVersion   | Boolean      | &check;      |
| platformVersions | List<String> | &check;      |
