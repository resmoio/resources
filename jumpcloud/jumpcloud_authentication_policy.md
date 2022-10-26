---
description: JumpCloud Authentication Policy
---
jumpcloud_authentication_policy
-------------------------------

| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| description      | String   | &check;      |
| disabled         | Boolean  | &check;      |
| effect           | Effect   | &check;      |
| id               | String   | &cross;      |
| name             | String   | &check;      |
| organizationId   | String   | &cross;      |
| organizationName | String   | &cross;      |
| targets          | Targets  | &check;      |
| type             | String   | &check;      |

#### Effect
| **Name**    | **Type**    | **Nullable** |
| ----------- | ----------- | ------------ |
| action      | String      | &check;      |
| obligations | Obligations | &check;      |

#### Exclusion
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| field    | String   | &check;      |
| operator | String   | &check;      |
| value    | String   | &check;      |

#### Inclusion
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| field    | String   | &check;      |
| operator | String   | &check;      |
| value    | String   | &check;      |

#### Mfa
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| required | Boolean  | &check;      |

#### Obligations
| **Name**         | **Type**         | **Nullable** |
| ---------------- | ---------------- | ------------ |
| mfa              | Mfa              | &check;      |
| userVerification | UserVerification | &check;      |

#### Resource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| type     | String   | &check;      |

#### Targets
| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| resources      | List<Resource> | &check;      |
| userAttributes | UserAttributes | &check;      |
| userGroups     | UserGroups     | &check;      |
| users          | Users          | &check;      |

#### UserAttributes
| **Name**   | **Type**        | **Nullable** |
| ---------- | --------------- | ------------ |
| exclusions | List<Exclusion> | &check;      |
| inclusions | List<Inclusion> | &check;      |

#### UserGroups
| **Name**   | **Type**     | **Nullable** |
| ---------- | ------------ | ------------ |
| exclusions | List<String> | &check;      |
| inclusions | List<String> | &check;      |

#### UserVerification
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| requirement | String   | &check;      |

#### Users
| **Name**   | **Type**     | **Nullable** |
| ---------- | ------------ | ------------ |
| inclusions | List<String> | &check;      |
