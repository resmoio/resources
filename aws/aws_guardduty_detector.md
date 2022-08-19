---
description: Amazon Web Services GuardDuty Detector
---
aws_guardduty_detector
----------------------

| **Name**                   | **Type**                       | **Nullable** |
| -------------------------- | ------------------------------ | ------------ |
| accountId                  | String                         | &cross;      |
| accountName                | String                         | &check;      |
| administratorAccount       | AdministratorAccount           | &check;      |
| createdAt                  | String                         | &check;      |
| dataSources                | DataSourceConfigurationsResult | &check;      |
| findingPublishingFrequency | String                         | &check;      |
| id                         | String                         | &cross;      |
| serviceRole                | String                         | &check;      |
| status                     | String                         | &check;      |
| tags                       | Map<String,String>             | &check;      |
| updatedAt                  | String                         | &check;      |

#### AdministratorAccount
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| accountId          | String   | &check;      |
| invitationId       | String   | &check;      |
| invitedAt          | String   | &check;      |
| relationshipStatus | String   | &check;      |

#### ConfigurationResult
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| status   | String   | &check;      |

#### DataSourceConfigurationsResult
| **Name**   | **Type**                      | **Nullable** |
| ---------- | ----------------------------- | ------------ |
| cloudTrail | ConfigurationResult           | &check;      |
| dnsLogs    | ConfigurationResult           | &check;      |
| flowLogs   | ConfigurationResult           | &check;      |
| kubernetes | KubernetesConfigurationResult | &check;      |
| s3Logs     | ConfigurationResult           | &check;      |

#### KubernetesConfigurationResult
| **Name**  | **Type**            | **Nullable** |
| --------- | ------------------- | ------------ |
| auditLogs | ConfigurationResult | &check;      |
