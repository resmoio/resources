---
description: Sophos Health Check
---
sophos_health_check
-------------------

| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| endpoint        | Endpoint | &check;      |
| tenantReference | Tenant   | &cross;      |

#### Endpoint
| **Name**         | **Type**         | **Nullable** |
| ---------------- | ---------------- | ------------ |
| exclusions       | Exclusions       | &check;      |
| policy           | Policy           | &check;      |
| protection       | Protection       | &check;      |
| tamperProtection | TamperProtection | &check;      |

#### ExclusionPolicyDevice
| **Name**              | **Type**                             | **Nullable** |
| --------------------- | ------------------------------------ | ------------ |
| exclusions            | List<ExclusionPolicyDeviceExclusion> | &check;      |
| numberOfSecurityRisks | Int                                  | &check;      |
| total                 | Int                                  | &check;      |

#### ExclusionPolicyDeviceExclusion
| **Name**                | **Type**                      | **Nullable** |
| ----------------------- | ----------------------------- | ------------ |
| lockedByManagingAccount | Boolean                       | &check;      |
| policyId                | String                        | &check;      |
| policyName              | String                        | &check;      |
| scanningExclusions      | List<GlobalScanningExclusion> | &check;      |

#### Exclusions
| **Name** | **Type**         | **Nullable** |
| -------- | ---------------- | ------------ |
| global   | ExclusionsGlobal | &check;      |
| policy   | ExclusionsPolicy | &check;      |

#### ExclusionsGlobal
| **Name**                | **Type**                      | **Nullable** |
| ----------------------- | ----------------------------- | ------------ |
| lockedByManagingAccount | Boolean                       | &check;      |
| numberOfSecurityRisks   | Int                           | &check;      |
| scanningExclusions      | List<GlobalScanningExclusion> | &check;      |

#### ExclusionsPolicy
| **Name** | **Type**              | **Nullable** |
| -------- | --------------------- | ------------ |
| computer | ExclusionPolicyDevice | &check;      |
| server   | ExclusionPolicyDevice | &check;      |

#### GlobalScanningExclusion
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| id         | String   | &check;      |
| reasonCode | String   | &check;      |
| scanMode   | String   | &check;      |
| type       | String   | &check;      |
| value      | String   | &check;      |

#### Policy
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| computer | PolicyDevice | &check;      |
| server   | PolicyDevice | &check;      |

#### PolicyDevice
| **Name**   | **Type**               | **Nullable** |
| ---------- | ---------------------- | ------------ |
| protection | PolicyDeviceProtection | &check;      |

#### PolicyDeviceProtection
| **Name**         | **Type**                           | **Nullable** |
| ---------------- | ---------------------------------- | ------------ |
| notOnRecommended | Int                                | &check;      |
| policies         | List<PolicyDeviceProtectionPolicy> | &check;      |
| total            | Int                                | &check;      |

#### PolicyDeviceProtectionPolicy
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| id                      | String   | &check;      |
| lockedByManagingAccount | Boolean  | &check;      |
| name                    | String   | &check;      |
| notOnRecommended        | Int      | &check;      |

#### Protection
| **Name** | **Type**         | **Nullable** |
| -------- | ---------------- | ------------ |
| computer | ProtectionDevice | &check;      |
| server   | ProtectionDevice | &check;      |

#### ProtectionDevice
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| notFullyProtected | Int      | &check;      |
| total             | Int      | &check;      |

#### TamperProtection
| **Name** | **Type**               | **Nullable** |
| -------- | ---------------------- | ------------ |
| computer | TamperProtectionDevice | &check;      |
| global   | Boolean                | &check;      |
| server   | TamperProtectionDevice | &check;      |

#### TamperProtectionDevice
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| disabled | Int      | &check;      |
| total    | Int      | &check;      |

#### Tenant
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |
