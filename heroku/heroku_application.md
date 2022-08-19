---
description: Heroku Application
---
heroku_application
------------------

| **Name**                     | **Type**     | **Nullable** |
| ---------------------------- | ------------ | ------------ |
| acm                          | Boolean      | &check;      |
| archivedAt                   | String       | &check;      |
| buildStack                   | BuildStack   | &check;      |
| buildpackProvidedDescription | String       | &check;      |
| createdAt                    | String       | &check;      |
| gitUrl                       | String       | &check;      |
| id                           | String       | &cross;      |
| internalRouting              | Boolean      | &check;      |
| maintenance                  | Boolean      | &check;      |
| name                         | String       | &check;      |
| organization                 | Organization | &check;      |
| owner                        | Owner        | &check;      |
| region                       | Region       | &check;      |
| releasedAt                   | String       | &check;      |
| repoSize                     | Int          | &check;      |
| slugSize                     | Int          | &check;      |
| space                        | Space        | &check;      |
| stack                        | Stack        | &check;      |
| team                         | Team         | &check;      |
| updatedAt                    | String       | &check;      |
| webUrl                       | String       | &check;      |

#### BuildStack
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Owner
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| id       | String   | &check;      |

#### Region
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Space
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| shield   | Boolean  | &check;      |

#### Stack
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
