---
description: Entity Device
---
device
------

| **Name**               | **Type**     | **Nullable** |
| ---------------------- | ------------ | ------------ |
| encrypted              | Boolean      | &check;      |
| firewallEnabled        | Boolean      | &check;      |
| id                     | String       | &cross;      |
| model                  | String       | &check;      |
| operatingSystem        | String       | &check;      |
| operatingSystemVersion | String       | &check;      |
| platform               | String       | &check;      |
| referencedType         | String       | &cross;      |
| screenLockEnabled      | Boolean      | &check;      |
| status                 | String       | &check;      |
| type                   | DeviceType   | &check;      |
| userEmails             | List<String> | &check;      |
| userNames              | List<String> | &check;      |
| vendor                 | String       | &check;      |

#### BasicResource
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| referencedType | String   | &cross;      |

#### DeviceType
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |
