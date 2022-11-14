---
description: Amazon Web Services Elastic Beanstalk Application
---
aws_elasticbeanstalk_application
--------------------------------

| **Name**                | **Type**                           | **Nullable** |
| ----------------------- | ---------------------------------- | ------------ |
| accountId               | String                             | &cross;      |
| accountName             | String                             | &check;      |
| applicationArn          | String                             | &cross;      |
| applicationName         | String                             | &check;      |
| configurationTemplates  | List<String>                       | &check;      |
| dateCreated             | String                             | &check;      |
| dateUpdated             | String                             | &check;      |
| description             | String                             | &check;      |
| region                  | String                             | &cross;      |
| resourceLifecycleConfig | ApplicationResourceLifecycleConfig | &check;      |
| versions                | List<String>                       | &check;      |

#### ApplicationResourceLifecycleConfig
| **Name**               | **Type**                          | **Nullable** |
| ---------------------- | --------------------------------- | ------------ |
| serviceRole            | String                            | &check;      |
| versionLifecycleConfig | ApplicationVersionLifecycleConfig | &check;      |

#### ApplicationVersionLifecycleConfig
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| maxAgeRule   | MaxAgeRule   | &check;      |
| maxCountRule | MaxCountRule | &check;      |

#### MaxAgeRule
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| deleteSourceFromS3 | Boolean  | &check;      |
| enabled            | Boolean  | &check;      |
| maxAgeInDays       | Int      | &check;      |

#### MaxCountRule
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| deleteSourceFromS3 | Boolean  | &check;      |
| enabled            | Boolean  | &check;      |
| maxCount           | Int      | &check;      |
