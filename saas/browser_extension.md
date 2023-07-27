---
description: SaaS Browser Extension
---
browser_extension
-----------------

| **Name**           | **Type**   | **Nullable** |
| ------------------ | ---------- | ------------ |
| browser            | Browser    | &cross;      |
| email              | String     | &cross;      |
| extensionVersion   | String     | &cross;      |
| id                 | String     | &cross;      |
| installedAt        | String     | &check;      |
| lastSync           | String     | &cross;      |
| passwordSharedApps | List<List> | &check;      |
| platform           | Platform   | &cross;      |
| profileEmail       | String     | &check;      |
| uninstalledAt      | String     | &check;      |

#### Browser
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |
| version  | String   | &check;      |

#### Platform
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| architecture | String   | &check;      |
| name         | String   | &check;      |
| version      | String   | &check;      |

#### SharedApp
| **Name**            | **Type**  | **Nullable** |
| ------------------- | --------- | ------------ |
| app                 | String    | &check;      |
| eventTime           | Timestamp | &cross;      |
| hasCorrectLoginInfo | Boolean   | &check;      |
| identifier          | String    | &cross;      |
| initiator           | String    | &cross;      |
| relatedURLPart      | String    | &check;      |
