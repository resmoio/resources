---
description: Drata Personnel
---
drata_personnel
---------------

| **Name**                      | **Type**              | **Nullable** |
| ----------------------------- | --------------------- | ------------ |
| agentEnabled                  | Boolean               | &check;      |
| appsCount                     | Int                   | &check;      |
| appsCountLastCheckedAt        | String                | &check;      |
| backgroundCheckExcluded       | Boolean               | &check;      |
| backgroundCheckExcludedReason | String                | &check;      |
| complianceChecks              | List<ComplianceCheck> | &check;      |
| complianceTests               | List<ComplianceTest>  | &check;      |
| createdAt                     | String                | &check;      |
| data                          | PersonnelData         | &check;      |
| devices                       | List<Device>          | &check;      |
| devicesCount                  | Int                   | &check;      |
| devicesFailingComplianceCount | Int                   | &check;      |
| employmentStatus              | String                | &check;      |
| id                            | Int                   | &cross;      |
| manualUploadEnabled           | Boolean               | &check;      |
| notHumanReason                | String                | &check;      |
| reasonProvider                | User                  | &check;      |
| separationDate                | String                | &check;      |
| startDate                     | String                | &check;      |
| statusUpdatedAt               | String                | &check;      |
| updatedAt                     | String                | &check;      |
| user                          | User                  | &check;      |

#### ComplianceCheck
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| checkFrequency | String   | &check;      |
| compliant      | Boolean  | &check;      |
| createdAt      | String   | &check;      |
| expiresAt      | String   | &check;      |
| id             | Int      | &check;      |
| lastCheckedAt  | String   | &check;      |
| type           | String   | &check;      |
| updatedAt      | String   | &check;      |

#### ComplianceTest
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| autopilotTaskType     | String   | &check;      |
| checkResultStatus     | String   | &check;      |
| checkStatus           | String   | &check;      |
| controlTestInstanceId | Int      | &check;      |
| lastCheck             | String   | &check;      |
| monitorId             | Int      | &check;      |
| name                  | String   | &check;      |
| testId                | Int      | &check;      |

#### Connection
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| accountId          | String             | &check;      |
| aliasUpdatedAt     | String             | &check;      |
| authorized         | Boolean            | &check;      |
| clientAlias        | String             | &check;      |
| clientId           | String             | &check;      |
| clientType         | String             | &check;      |
| code               | String             | &check;      |
| connected          | Boolean            | &check;      |
| connectedAt        | String             | &check;      |
| deletedAt          | String             | &check;      |
| failedAt           | String             | &check;      |
| id                 | Int                | &check;      |
| key                | String             | &check;      |
| manuallyUpdatedAt  | String             | &check;      |
| providerTypes      | List<ProviderType> | &check;      |
| state              | String             | &check;      |
| writeAccessEnabled | Boolean            | &check;      |

#### Data
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| agentVersion   | String   | &check;      |
| macAddress     | String   | &check;      |
| osVersion      | String   | &check;      |
| processor      | String   | &check;      |
| screenLockTime | Int      | &check;      |
| serialNumber   | String   | &check;      |

#### Device
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| agentVersion      | String   | &check;      |
| appsCount         | Int      | &check;      |
| createdAt         | String   | &check;      |
| deletedAt         | String   | &check;      |
| encryptionEnabled | Boolean  | &check;      |
| firewallEnabled   | Boolean  | &check;      |
| gateKeeperEnabled | Boolean  | &check;      |
| graphics          | String   | &check;      |
| hddSize           | String   | &check;      |
| id                | Int      | &check;      |
| lastCheckedAt     | String   | &check;      |
| macAddress        | String   | &check;      |
| memory            | String   | &check;      |
| model             | String   | &check;      |
| osVersion         | String   | &check;      |
| processor         | String   | &check;      |
| screenLockTime    | Int      | &check;      |
| serialNumber      | String   | &check;      |
| sourceType        | String   | &check;      |
| updatedAt         | String   | &check;      |

#### Identity
| **Name**       | **Type**   | **Nullable** |
| -------------- | ---------- | ------------ |
| connectedAt    | String     | &check;      |
| connection     | Connection | &check;      |
| disconnectedAt | String     | &check;      |
| hasMfa         | Boolean    | &check;      |
| id             | Int        | &check;      |
| identityId     | String     | &check;      |
| user           | Int        | &check;      |
| username       | String     | &check;      |

#### PersonnelData
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| agentVersion   | String   | &check;      |
| createdAt      | String   | &check;      |
| graphics       | String   | &check;      |
| hddSize        | String   | &check;      |
| lastCheckedAt  | String   | &check;      |
| macAddress     | String   | &check;      |
| memory         | String   | &check;      |
| osVersion      | String   | &check;      |
| processor      | String   | &check;      |
| screenLockTime | Int      | &check;      |
| serialNumber   | String   | &check;      |
| updatedAt      | String   | &check;      |

#### ProviderType
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| isEnabled | Boolean  | &check;      |
| value     | String   | &check;      |

#### User
| **Name**           | **Type**       | **Nullable** |
| ------------------ | -------------- | ------------ |
| createdAt          | String         | &check;      |
| drataTermsAgreedAt | String         | &check;      |
| email              | String         | &check;      |
| firstName          | String         | &check;      |
| id                 | Int            | &check;      |
| identities         | List<Identity> | &check;      |
| jobTitle           | String         | &check;      |
| lastName           | String         | &check;      |
| required           | Boolean        | &check;      |
| roles              | List<String>   | &check;      |
| updatedAt          | String         | &check;      |
