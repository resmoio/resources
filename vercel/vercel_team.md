---
description: Vercel Team
---
vercel_team
-----------

| **Name**                | **Type**            | **Nullable** |
| ----------------------- | ------------------- | ------------ |
| billing                 | Billing             | &check;      |
| created                 | String              | &check;      |
| createdAt               | Long                | &check;      |
| creatorId               | String              | &check;      |
| description             | String              | &check;      |
| enablePreviewFeedback   | Boolean             | &check;      |
| enabledInvoiceItems     | Map<String,Map>     | &check;      |
| id                      | String              | &cross;      |
| inviteCode              | String              | &check;      |
| memberUserIds           | List<String>        | &check;      |
| membership              | Membership          | &check;      |
| name                    | String              | &check;      |
| platformVersion         | String              | &check;      |
| previewDeploymentSuffix | String              | &check;      |
| profiles                | List<String>        | &check;      |
| remoteCaching           | Map<String,Boolean> | &check;      |
| resourceConfig          | ResourceConfig      | &check;      |
| slug                    | String              | &check;      |
| softBlock               | String              | &check;      |
| stagingPrefix           | String              | &check;      |
| updatedAt               | Long                | &check;      |

#### Billing
| **Name**    | **Type**         | **Nullable** |
| ----------- | ---------------- | ------------ |
| addons      | String           | &check;      |
| address     | String           | &check;      |
| cancelation | Long             | &check;      |
| currency    | String           | &check;      |
| email       | String           | &check;      |
| language    | String           | &check;      |
| name        | String           | &check;      |
| overdue     | String           | &check;      |
| period      | Map<String,Long> | &check;      |
| plan        | String           | &check;      |
| platform    | String           | &check;      |
| status      | String           | &check;      |
| tax         | String           | &check;      |
| trial       | Map<String,Long> | &check;      |

#### Membership
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| ceratedAt | Long     | &check;      |
| confirmed | Boolean  | &check;      |
| created   | Long     | &check;      |
| role      | String   | &check;      |
| teamId    | String   | &check;      |
| updatedAt | Long     | &check;      |

#### ResourceConfig
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| concurrentBuilds | Long     | &check;      |
