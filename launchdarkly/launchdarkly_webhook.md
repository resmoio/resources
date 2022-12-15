---
description: LaunchDarkly Webhook
---
launchdarkly_webhook
--------------------

| **Name**   | **Type**        | **Nullable** |
| ---------- | --------------- | ------------ |
| _access    | Access          | &check;      |
| _id        | String          | &cross;      |
| name       | String          | &check;      |
| on         | Boolean         | &check;      |
| secret     | String          | &check;      |
| statements | List<Statement> | &check;      |
| tags       | List<String>    | &check;      |
| url        | String          | &check;      |

#### Access
| **Name** | **Type**             | **Nullable** |
| -------- | -------------------- | ------------ |
| allowed  | List<Access.Allowed> | &check;      |
| denied   | List<Access.Denied>  | &check;      |

#### Access.Allowed
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| action   | String   | &check;      |
| reason   | Reason   | &check;      |

#### Access.Denied
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| action   | String   | &check;      |
| reason   | Reason   | &check;      |

#### Reason
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| actions      | List<String> | &check;      |
| effect       | String       | &check;      |
| notActions   | List<String> | &check;      |
| notResources | List<String> | &check;      |
| resources    | List<String> | &check;      |
| role_name    | String       | &check;      |

#### Statement
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| actions      | List<String> | &check;      |
| effect       | String       | &check;      |
| notActions   | List<String> | &check;      |
| notResources | List<String> | &check;      |
| resources    | List<String> | &check;      |
