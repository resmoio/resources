---
description: Amazon Web Services SSO Instance
---
aws_sso_instance
----------------

| **Name**                | **Type**                     | **Nullable** |
| ----------------------- | ---------------------------- | ------------ |
| accessControlAttributes | List<AccessControlAttribute> | &check;      |
| accountId               | String                       | &cross;      |
| arn                     | String                       | &cross;      |
| id                      | String                       | &cross;      |
| permissionSets          | List<PermissionSet>          | &check;      |
| region                  | String                       | &cross;      |

#### AccessControlAttribute
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| key      | String       | &cross;      |
| value    | List<String> | &check;      |

#### PermissionSet
| **Name**        | **Type**                          | **Nullable** |
| --------------- | --------------------------------- | ------------ |
| accounts        | List<PermissionSet.Account>       | &cross;      |
| arn             | String                            | &cross;      |
| createdDate     | String                            | &check;      |
| description     | String                            | &check;      |
| inlinePolicy    | JSON                              | &check;      |
| managedPolicies | List<PermissionSet.ManagedPolicy> | &check;      |
| name            | String                            | &cross;      |
| relayState      | String                            | &check;      |
| sessionDuration | String                            | &cross;      |
| tags            | Map<String,String>                | &check;      |

#### PermissionSet.Account
| **Name**    | **Type**                                      | **Nullable** |
| ----------- | --------------------------------------------- | ------------ |
| assignments | List<PermissionSet.Account.AccountAssignment> | &cross;      |
| id          | String                                        | &cross;      |

#### PermissionSet.Account.AccountAssignment
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| principalId   | String   | &cross;      |
| principalType | String   | &cross;      |

#### PermissionSet.ManagedPolicy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| arn      | String   | &cross;      |
| name     | String   | &cross;      |

#### ResourceCustomComparable
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |

