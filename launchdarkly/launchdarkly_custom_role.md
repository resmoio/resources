---
description: LaunchDarkly Custom Role
---
launchdarkly_custom_role
------------------------

| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| _access         | Access       | &check;      |
| _id             | String       | &cross;      |
| basePermissions | String       | &check;      |
| description     | String       | &check;      |
| key             | String       | &check;      |
| name            | String       | &check;      |
| policy          | List<Policy> | &check;      |

#### Access
| **Name** | **Type**             | **Nullable** |
| -------- | -------------------- | ------------ |
| allowed  | List<Access.Allowed> | &check;      |
| denied   | List<Access.Denied>  | &check;      |

#### Access.Allowed
| **Name** | **Type**      | **Nullable** |
| -------- | ------------- | ------------ |
| action   | String        | &check;      |
| reason   | Access.Reason | &check;      |

#### Access.Denied
| **Name** | **Type**      | **Nullable** |
| -------- | ------------- | ------------ |
| action   | String        | &check;      |
| reason   | Access.Reason | &check;      |

#### Access.Reason
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| actions      | List<String> | &check;      |
| effect       | String       | &check;      |
| notActions   | List<String> | &check;      |
| notResources | List<String> | &check;      |
| resources    | List<String> | &check;      |
| role_name    | String       | &check;      |

#### Policy
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| actions      | List<String> | &check;      |
| effect       | String       | &check;      |
| notActions   | List<String> | &check;      |
| notResources | List<String> | &check;      |
| resources    | List<String> | &check;      |
