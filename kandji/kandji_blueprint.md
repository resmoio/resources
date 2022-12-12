---
description: Kandji Blueprint
---
kandji_blueprint
----------------

| **Name**              | **Type**                | **Nullable** |
| --------------------- | ----------------------- | ------------ |
| color                 | String                  | &check;      |
| computersCount        | Int                     | &check;      |
| description           | String                  | &check;      |
| enrollmentCode        | EnrollmentCode          | &check;      |
| icon                  | String                  | &check;      |
| id                    | String                  | &cross;      |
| missingComputersCount | Int                     | &check;      |
| name                  | String                  | &check;      |
| params                | Map<String,ParamDetail> | &check;      |

#### EnrollmentCode
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | String   | &check;      |
| isActive | Boolean  | &check;      |

#### ParamDetail
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| daily    | Boolean  | &check;      |
| mute     | Boolean  | &check;      |
