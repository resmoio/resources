---
description: Google Cloud Platform IAM Service Account Key
---
gcp_iam_service_account_key
---------------------------

| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| disabled           | Boolean  | &check;      |
| keyAlgorithm       | String   | &check;      |
| keyOrigin          | String   | &check;      |
| keyType            | String   | &check;      |
| name               | String   | &cross;      |
| privateKeyType     | String   | &check;      |
| project            | String   | &cross;      |
| serviceAccountName | String   | &check;      |
| validAfterTime     | String   | &check;      |
| validBeforeTime    | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
