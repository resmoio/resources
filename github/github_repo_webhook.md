---
description: GitHub Repository Webhook
---
github_repo_webhook
-------------------

| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| active        | Boolean      | &cross;      |
| config        | Config       | &check;      |
| createdAt     | String       | &check;      |
| deliveriesUrl | String       | &check;      |
| events        | List<String> | &check;      |
| id            | String       | &cross;      |
| lastResponse  | LastResponse | &check;      |
| name          | String       | &cross;      |
| organization  | Organization | &cross;      |
| pingUrl       | String       | &check;      |
| repository    | Repository   | &cross;      |
| testUrl       | String       | &check;      |
| type          | String       | &cross;      |
| updatedAt     | String       | &check;      |
| url           | String       | &check;      |

#### Config
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| contentType | String   | &check;      |
| insecureSSL | String   | &check;      |
| secret      | String   | &check;      |
| url         | String   | &check;      |

#### LastResponse
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | Int      | &check;      |
| message  | String   | &check;      |
| status   | String   | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Repository
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
