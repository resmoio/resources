---
description: Confluence Space
---
confluence_space
----------------

| **Name**    | **Type**         | **Nullable** |
| ----------- | ---------------- | ------------ |
| description | Description      | &check;      |
| history     | History          | &check;      |
| id          | Number           | &cross;      |
| key         | String           | &check;      |
| metadata    | List<Metadata>   | &check;      |
| name        | String           | &check;      |
| operations  | List<Operation>  | &check;      |
| permissions | List<Permission> | &check;      |
| settings    | Setting          | &check;      |
| site        | String           | &cross;      |
| status      | String           | &check;      |
| type        | String           | &check;      |

#### Description
| **Name** | **Type**                     | **Nullable** |
| -------- | ---------------------------- | ------------ |
| plain    | Description.DescriptionValue | &check;      |
| view     | Description.DescriptionValue | &check;      |

#### Description.DescriptionValue
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| representation | String   | &check;      |
| value          | String   | &check;      |

#### Group
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### History
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| createdBy   | User     | &check;      |
| createdDate | String   | &check;      |

#### Metadata
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| label    | String   | &check;      |
| name     | String   | &check;      |
| prefix   | String   | &check;      |

#### Operation
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| operation  | String   | &check;      |
| targetType | String   | &check;      |

#### Permission
| **Name**         | **Type**           | **Nullable** |
| ---------------- | ------------------ | ------------ |
| anonymousAccess  | Boolean            | &check;      |
| id               | Number             | &check;      |
| operation        | Operation          | &check;      |
| subjects         | Permission.Subject | &check;      |
| unlicensedAccess | Boolean            | &check;      |

#### Permission.Subject
| **Name** | **Type**    | **Nullable** |
| -------- | ----------- | ------------ |
| groups   | List<Group> | &check;      |
| users    | List<User>  | &check;      |

#### Setting
| **Name**             | **Type**       | **Nullable** |
| -------------------- | -------------- | ------------ |
| editor               | Setting.Editor | &check;      |
| routeOverrideEnabled | Boolean        | &check;      |

#### Setting.Editor
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| blogpost | String   | &check;      |
| default  | String   | &check;      |
| page     | String   | &check;      |

#### User
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| accountId              | String   | &check;      |
| accountType            | String   | &check;      |
| displayName            | String   | &check;      |
| email                  | String   | &check;      |
| isExternalCollaborator | Boolean  | &check;      |
| publicName             | String   | &check;      |
| timeZone               | String   | &check;      |
| type                   | String   | &check;      |
| userKey                | String   | &check;      |
| username               | String   | &check;      |
