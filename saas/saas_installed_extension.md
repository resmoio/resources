---
description: SaaS Browser Extension
---
saas_installed_extension
------------------------

| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| browser          | Browser  | &cross;      |
| extensionVersion | String   | &cross;      |
| id               | String   | &cross;      |
| lastSync         | String   | &cross;      |
| platform         | Platform | &cross;      |
| profileEmail     | String   | &check;      |
| userId           | String   | &cross;      |

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
