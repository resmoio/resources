---
description: LaunchDarkly Team
---
launchdarkly_team
-----------------

| **Name**      | **Type**    | **Nullable** |
| ------------- | ----------- | ------------ |
| _access       | Access      | &check;      |
| _creationDate | Long        | &check;      |
| _idpSynced    | Boolean     | &check;      |
| _lastModified | Long        | &check;      |
| _version      | Int         | &check;      |
| description   | String      | &check;      |
| key           | String      | &cross;      |
| maintainers   | Maintainers | &check;      |
| members       | Members     | &check;      |
| name          | String      | &check;      |
| projects      | Projects    | &check;      |
| roles         | Roles       | &check;      |

#### Access
| **Name** | **Type**             | **Nullable** |
| -------- | -------------------- | ------------ |
| allowed  | List<Access.Allowed> | &check;      |
| denied   | List<Access.Denied>  | &check;      |

#### Access.Allowed
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| action   | String   | &check;      |
| reason   | Reason   | &check;      |

#### Access.Denied
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| action   | String   | &check;      |
| reason   | Reason   | &check;      |

#### Item
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| _id       | String   | &check;      |
| email     | String   | &check;      |
| firstName | String   | &check;      |
| lastName  | String   | &check;      |
| role      | String   | &check;      |

#### Maintainers
| **Name**   | **Type**   | **Nullable** |
| ---------- | ---------- | ------------ |
| items      | List<Item> | &check;      |
| totalCount | Int        | &check;      |

#### Members
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| totalCount | Int      | &check;      |

#### Projects
| **Name**   | **Type**            | **Nullable** |
| ---------- | ------------------- | ------------ |
| items      | List<Projects.Item> | &check;      |
| totalCount | Int                 | &check;      |

#### Projects.Item
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| key      | String   | &cross;      |
| name     | String   | &check;      |

#### Reason
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| actions      | List<String> | &check;      |
| effect       | String       | &check;      |
| notActions   | List<String> | &check;      |
| notResources | List<String> | &check;      |
| resources    | List<String> | &check;      |
| role_name    | String       | &check;      |

#### Roles
| **Name**   | **Type**         | **Nullable** |
| ---------- | ---------------- | ------------ |
| items      | List<Roles.Item> | &check;      |
| totalCount | Int              | &check;      |

#### Roles.Item
| **Name**  | **Type**            | **Nullable** |
| --------- | ------------------- | ------------ |
| appliedOn | Long                | &check;      |
| key       | String              | &check;      |
| name      | String              | &check;      |
| projects  | Roles.Item.Projects | &check;      |

#### Roles.Item.Projects
| **Name**   | **Type**                       | **Nullable** |
| ---------- | ------------------------------ | ------------ |
| items      | List<Roles.Item.Projects.Item> | &check;      |
| totalCount | Int                            | &check;      |

#### Roles.Item.Projects.Item
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| key      | String   | &check;      |
| name     | String   | &check;      |
