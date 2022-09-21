---
description: Azure DevOps User Entitlement
---
azure_devops_user_entitlement
-----------------------------

| **Name**            | **Type**                 | **Nullable** |
| ------------------- | ------------------------ | ------------ |
| accessLevel         | AccessLevel              | &check;      |
| accountId           | String                   | &cross;      |
| accountName         | String                   | &cross;      |
| dateCreated         | String                   | &check;      |
| groupAssignments    | List<GroupEntitlement>   | &check;      |
| id                  | String                   | &cross;      |
| lastAccessedDate    | String                   | &check;      |
| projectEntitlements | List<ProjectEntitlement> | &check;      |
| user                | User                     | &check;      |

#### AccessLevel
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| accountLicenseType | String   | &check;      |
| assignmentSource   | String   | &check;      |
| licenseDisplayName | String   | &check;      |
| licensingSource    | String   | &check;      |
| msdnLicenseType    | String   | &check;      |
| status             | String   | &check;      |
| statusMessage      | String   | &check;      |

#### Group
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| description   | String   | &check;      |
| descriptor    | String   | &check;      |
| displayName   | String   | &check;      |
| domain        | String   | &check;      |
| mailAddress   | String   | &check;      |
| origin        | String   | &check;      |
| originId      | String   | &check;      |
| principalName | String   | &check;      |
| subjectKind   | String   | &check;      |
| url           | String   | &check;      |

#### GroupEntitlement
| **Name**            | **Type**                 | **Nullable** |
| ------------------- | ------------------------ | ------------ |
| group               | Group                    | &check;      |
| id                  | String                   | &check;      |
| lastExecuted        | String                   | &check;      |
| licenceRule         | AccessLevel              | &check;      |
| projectEntitlements | List<ProjectEntitlement> | &check;      |
| status              | String                   | &check;      |

#### ProjectEntitlement
| **Name**                   | **Type**                      | **Nullable** |
| -------------------------- | ----------------------------- | ------------ |
| assignmentSource           | String                        | &check;      |
| group                      | ProjectEntitlement.Group      | &check;      |
| projectPermissionInherited | String                        | &check;      |
| projectRef                 | ProjectEntitlement.Project    | &check;      |
| teamRefs                   | List<ProjectEntitlement.Team> | &check;      |

#### ProjectEntitlement.Group
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| groupType   | String   | &check;      |

#### ProjectEntitlement.Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### ProjectEntitlement.Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### User
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| descriptor        | String   | &check;      |
| directoryAlias    | String   | &check;      |
| displayName       | String   | &check;      |
| domain            | String   | &check;      |
| isDeletedInOrigin | Boolean  | &check;      |
| mailAddress       | String   | &check;      |
| metaType          | String   | &check;      |
| origin            | String   | &check;      |
| originId          | String   | &check;      |
| principalName     | String   | &check;      |
| subjectKind       | String   | &check;      |
| url               | String   | &check;      |
