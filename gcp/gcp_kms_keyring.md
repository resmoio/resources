---
description: Google Cloud Platform KMS Keyring
---
gcp_kms_keyring
---------------

| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| createTime | String   | &check;      |
| location   | String   | &check;      |
| name       | String   | &cross;      |
| policy     | Policy   | &check;      |
| project    | String   | &cross;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### Policy
| **Name** | **Type**             | **Nullable** |
| -------- | -------------------- | ------------ |
| bindings | List<Policy.Binding> | &check;      |

#### Policy.Binding
| **Name**  | **Type**            | **Nullable** |
| --------- | ------------------- | ------------ |
| condition | Policy.Binding.Expr | &check;      |
| members   | List<String>        | &check;      |
| role      | String              | &check;      |

#### Policy.Binding.Expr
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| expression  | String   | &check;      |
| location    | String   | &check;      |
| title       | String   | &check;      |
