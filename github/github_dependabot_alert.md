---
description: GitHub Dependabot Alert
---
github_dependabot_alert
-----------------------

| **Name**              | **Type**         | **Nullable** |
| --------------------- | ---------------- | ------------ |
| createdAt             | Date             | &check;      |
| dependency            | Dependency       | &check;      |
| dismissedAt           | Date             | &check;      |
| dismissedBy           | DismissedBy      | &check;      |
| dismissedComment      | String           | &check;      |
| dismissedReason       | String           | &check;      |
| fixedAt               | String           | &check;      |
| number                | Long             | &cross;      |
| organization          | Organization     | &cross;      |
| repository            | Repository       | &cross;      |
| securityAdvisory      | SecurityAdvisory | &check;      |
| securityVulnerability | Vulnerability    | &check;      |
| state                 | String           | &check;      |
| updatedAt             | Date             | &check;      |

#### Cvss
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| score        | Double   | &check;      |
| vectorString | String   | &check;      |

#### Cwe
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| cweId    | String   | &check;      |
| name     | String   | &check;      |

#### Dependency
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| manifestPath | String   | &check;      |
| package      | Package  | &check;      |
| scope        | String   | &check;      |

#### DismissedBy
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &check;      |
| login     | String   | &check;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |

#### FirstPatchedVersion
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| identifier | String   | &check;      |

#### Identifier
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |
| value    | String   | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |

#### Package
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| ecosystem | String   | &check;      |
| name      | String   | &check;      |

#### Reference
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| url      | String   | &check;      |

#### Repository
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &cross;      |
| name     | String   | &cross;      |

#### SecurityAdvisory
| **Name**        | **Type**            | **Nullable** |
| --------------- | ------------------- | ------------ |
| cveId           | String              | &check;      |
| cvss            | Cvss                | &check;      |
| cwes            | List<Cwe>           | &check;      |
| description     | String              | &check;      |
| ghsaId          | String              | &check;      |
| identifiers     | List<Identifier>    | &check;      |
| publishedAt     | String              | &check;      |
| references      | List<Reference>     | &check;      |
| severity        | String              | &check;      |
| summary         | String              | &check;      |
| updatedAt       | String              | &check;      |
| vulnerabilities | List<Vulnerability> | &check;      |
| withdrawnAt     | String              | &check;      |

#### Vulnerability
| **Name**               | **Type**            | **Nullable** |
| ---------------------- | ------------------- | ------------ |
| firstPatchedVersion    | FirstPatchedVersion | &check;      |
| package                | Package             | &check;      |
| severity               | String              | &check;      |
| vulnerableVersionRange | String              | &check;      |
