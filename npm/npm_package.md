---
description: NPM Package
---
npm_package
-----------

| **Name**       | **Type**            | **Nullable** |
| -------------- | ------------------- | ------------ |
| author         | String              | &check;      |
| description    | String              | &check;      |
| distTags       | Map<String,String>  | &check;      |
| id             | String              | &cross;      |
| maintainers    | List<User>          | &check;      |
| name           | String              | &check;      |
| npmUser        | User                | &check;      |
| readmeFilename | String              | &check;      |
| rev            | String              | &check;      |
| time           | Map<String,String>  | &check;      |
| versions       | Map<String,Version> | &check;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| name     | String   | &check;      |

#### Version
| **Name**    | **Type**   | **Nullable** |
| ----------- | ---------- | ------------ |
| author      | String     | &check;      |
| description | String     | &check;      |
| from        | String     | &check;      |
| id          | String     | &check;      |
| license     | String     | &check;      |
| main        | String     | &check;      |
| maintainers | List<User> | &check;      |
| name        | String     | &check;      |
| nodeVersion | String     | &check;      |
| npmUser     | User       | &check;      |
| npmVersion  | String     | &check;      |
| version     | String     | &check;      |
