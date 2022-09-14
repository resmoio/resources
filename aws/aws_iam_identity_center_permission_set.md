---
description: Amazon Web Services IAM Identity Center Permission Set
---
aws_iam_identity_center_permission_set
--------------------------------------

| **Name**            | **Type**         | **Nullable** |
| ------------------- | ---------------- | ------------ |
| accounts            | List<String>     | &cross;      |
| assignments         | List<Assignment> | &cross;      |
| createdDate         | String           | &check;      |
| description         | String           | &check;      |
| duration            | String           | &check;      |
| inlinePolicy        | String           | &check;      |
| name                | String           | &cross;      |
| permissionSetArn    | String           | &cross;      |
| permissionsBoundary | Boundary         | &check;      |
| relayState          | String           | &check;      |

#### Assignment
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| accountId     | String   | &cross;      |
| principalId   | String   | &cross;      |
| principalType | String   | &cross;      |

#### Boundary
| **Name**                       | **Type**           | **Nullable** |
| ------------------------------ | ------------------ | ------------ |
| customerManagedPolicyReference | Boundary.Reference | &check;      |
| managedPolicyArn               | String             | &check;      |

#### Boundary.Reference
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| path     | String   | &cross;      |
