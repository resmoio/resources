---
description: Tailscale Key
---
tailscale_key
-------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| capabilities | Capabilities | &check;      |
| created      | String       | &check;      |
| expires      | String       | &check;      |
| id           | String       | &cross;      |

#### Capabilities
| **Name** | **Type**             | **Nullable** |
| -------- | -------------------- | ------------ |
| devices  | Capabilities.Devices | &check;      |

#### Capabilities.Devices
| **Name** | **Type**                    | **Nullable** |
| -------- | --------------------------- | ------------ |
| create   | Capabilities.Devices.Create | &check;      |

#### Capabilities.Devices.Create
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| ephemeral     | Boolean      | &check;      |
| preauthorized | Boolean      | &check;      |
| reusable      | Boolean      | &check;      |
| tags          | List<String> | &check;      |
