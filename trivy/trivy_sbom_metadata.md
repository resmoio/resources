---
description: Trivy SBOM Metadata
---
trivy_sbom_metadata
-------------------

| **Name**   | **Type**          | **Nullable** |
| ---------- | ----------------- | ------------ |
| bomRef     | String            | &cross;      |
| group      | String            | &check;      |
| name       | String            | &cross;      |
| properties | List<PropertyMap> | &check;      |
| purl       | String            | &check;      |
| timestamp  | String            | &cross;      |
| type       | String            | &cross;      |
| version    | String            | &check;      |

#### PropertyMap
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| value    | String   | &cross;      |

#### TrivyBaseResource
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |

