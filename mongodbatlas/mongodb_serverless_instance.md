---
description: MongoDB Atlas Serverless Instance
---
mongodb_serverless_instance
---------------------------

| **Name**          | **Type**          | **Nullable** |
| ----------------- | ----------------- | ------------ |
| connectionStrings | ConnectionStrings | &check;      |
| createDate        | String            | &check;      |
| groupId           | String            | &check;      |
| id                | String            | &cross;      |
| links             | List<Link>        | &cross;      |
| mongoDBVersion    | String            | &check;      |
| name              | String            | &cross;      |
| project           | Project           | &cross;      |
| providerSettings  | ProviderSettings  | &check;      |
| stateName         | String            | &check;      |

#### ConnectionStrings
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| standard    | String   | &check;      |
| standardSrv | String   | &check;      |

#### Link
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| rel      | String   | &check;      |

#### Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |

#### ProviderSettings
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| backingProviderName | String   | &check;      |
| providerName        | String   | &check;      |
| regionName          | String   | &check;      |
