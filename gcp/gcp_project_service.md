---
description: Google Cloud Platform GCP Project Service
---
gcp_project_service
-------------------

| **Name** | **Type**      | **Nullable** |
| -------- | ------------- | ------------ |
| config   | ServiceConfig | &check;      |
| name     | String        | &cross;      |
| parent   | String        | &check;      |
| project  | String        | &cross;      |
| state    | String        | &check;      |

#### Api
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| version  | String   | &cross;      |

#### AuthProvider
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| audiences        | String   | &check;      |
| authorizationUrl | String   | &check;      |
| id               | String   | &check;      |
| issuer           | String   | &check;      |
| jwksUri          | String   | &check;      |

#### AuthRequirement
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| audiences  | String   | &check;      |
| providerId | String   | &check;      |

#### Authentication
| **Name**  | **Type**                 | **Nullable** |
| --------- | ------------------------ | ------------ |
| providers | List<AuthProvider>       | &check;      |
| rules     | List<AuthenticationRule> | &check;      |

#### AuthenticationRule
| **Name**               | **Type**              | **Nullable** |
| ---------------------- | --------------------- | ------------ |
| allowWithoutCredential | Boolean               | &check;      |
| oauth                  | OAuthRequirements     | &check;      |
| requirements           | List<AuthRequirement> | &check;      |
| selector               | String                | &check;      |

#### Documentation
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| documentationRootUrl | String   | &check;      |
| overview             | String   | &check;      |
| serviceRootUrl       | String   | &check;      |
| summary              | String   | &check;      |

#### Endpoint
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| aliases   | List<String> | &check;      |
| allowCors | Boolean      | &check;      |
| name      | String       | &check;      |
| target    | String       | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### OAuthRequirements
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| canonicalScopes | String   | &check;      |

#### ServiceConfig
| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| apis           | List<Api>      | &check;      |
| authentication | Authentication | &check;      |
| documentation  | Documentation  | &check;      |
| endpoints      | List<Endpoint> | &check;      |
| name           | String         | &check;      |
| title          | String         | &check;      |
