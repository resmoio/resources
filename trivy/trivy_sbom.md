---
description: Trivy SBOM
---
trivy_sbom
----------

| **Name**      | **Type**            | **Nullable** |
| ------------- | ------------------- | ------------ |
| componentName | String              | &cross;      |
| components    | List<SBOMComponent> | &check;      |
| imageId       | String              | &check;      |
| metadata      | SBOMMetadata        | &cross;      |

#### SBOMComponent
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| bomRef    | String       | &check;      |
| dependsOn | List<String> | &check;      |
| group     | String       | &check;      |
| modified  | Boolean      | &check;      |
| name      | String       | &cross;      |
| purl      | String       | &check;      |
| type      | String       | &cross;      |
| version   | String       | &check;      |

#### SBOMMetadata
| **Name**   | **Type**                       | **Nullable** |
| ---------- | ------------------------------ | ------------ |
| bomRef     | String                         | &check;      |
| group      | String                         | &check;      |
| name       | String                         | &cross;      |
| properties | List<SBOMMetadata.PropertyMap> | &check;      |
| purl       | String                         | &check;      |
| timestamp  | String                         | &check;      |
| type       | String                         | &cross;      |
| version    | String                         | &check;      |

#### SBOMMetadata.PropertyMap
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| value    | String   | &cross;      |

#### TrivyBaseResource
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |

