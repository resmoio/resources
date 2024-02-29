---
description: Resmo Saas Discovery Settings
---
resmo_saas_discovery_settings
-----------------------------

| **Name**                  | **Type**       | **Nullable** |
| ------------------------- | -------------- | ------------ |
| accountId                 | String         | &cross;      |
| blockedSites              | List<String>   | &check;      |
| createdAt                 | String         | &check;      |
| createdBy                 | String         | &check;      |
| directoryOnboardingNotify | TimeWithUnit   | &check;      |
| extensionOnboardingNotify | TimeWithUnit   | &check;      |
| ignoredDomains            | List<String>   | &check;      |
| inactiveTimeout           | Int            | &check;      |
| passwordPolicy            | PasswordPolicy | &check;      |
| supportContact            | String         | &check;      |
| trackedDomains            | List<String>   | &check;      |
| updatedAt                 | String         | &check;      |
| updatedBy                 | String         | &check;      |

#### PasswordPolicy
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| hasDigit       | Boolean  | &cross;      |
| hasLowerCase   | Boolean  | &cross;      |
| hasSpecialChar | Boolean  | &cross;      |
| hasUpperCase   | Boolean  | &cross;      |
| minLength      | Int      | &cross;      |

#### TimeWithUnit
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| time     | Int      | &cross;      |
| unit     | String   | &cross;      |
