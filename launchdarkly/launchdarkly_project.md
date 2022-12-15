---
description: LaunchDarkly Project
---
launchdarkly_project
--------------------

| **Name**                      | **Type**                      | **Nullable** |
| ----------------------------- | ----------------------------- | ------------ |
| _id                           | String                        | &check;      |
| defaultClientSideAvailability | DefaultClientSideAvailability | &check;      |
| environments                  | Environments                  | &check;      |
| includeInSnippetByDefault     | Boolean                       | &check;      |
| key                           | String                        | &cross;      |
| name                          | String                        | &check;      |
| tags                          | List<String>                  | &check;      |

#### DefaultClientSideAvailability
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| usingEnvironmentId | Boolean  | &check;      |
| usingMobileKey     | Boolean  | &check;      |

#### Environments
| **Name**   | **Type**                | **Nullable** |
| ---------- | ----------------------- | ------------ |
| _links     | Environments.Links      | &check;      |
| items      | List<Environments.Item> | &check;      |
| totalCount | Int                     | &check;      |

#### Environments.Item
| **Name**           | **Type**                           | **Nullable** |
| ------------------ | ---------------------------------- | ------------ |
| _id                | String                             | &check;      |
| _links             | Environments.Item.Links            | &check;      |
| apiKey             | String                             | &check;      |
| approvalSettings   | Environments.Item.ApprovalSettings | &check;      |
| color              | String                             | &check;      |
| confirmChanges     | Boolean                            | &check;      |
| defaultTrackEvents | Boolean                            | &check;      |
| defaultTtl         | Int                                | &check;      |
| key                | String                             | &check;      |
| mobileKey          | String                             | &check;      |
| name               | String                             | &check;      |
| requireComments    | Boolean                            | &check;      |
| secureMode         | Boolean                            | &check;      |
| tags               | List<String>                       | &check;      |

#### Environments.Item.ApprovalSettings
| **Name**                         | **Type**     | **Nullable** |
| -------------------------------- | ------------ | ------------ |
| bypassApprovalsForPendingChanges | Boolean      | &check;      |
| canApplyDeclinedChanges          | Boolean      | &check;      |
| canReviewOwnRequest              | Boolean      | &check;      |
| minNumApprovals                  | Int          | &check;      |
| required                         | Boolean      | &check;      |
| requiredApprovalTags             | List<String> | &check;      |
| serviceKind                      | String       | &check;      |

#### Environments.Item.Links
| **Name** | **Type**                     | **Nullable** |
| -------- | ---------------------------- | ------------ |
| self     | Environments.Item.Links.Self | &check;      |

#### Environments.Item.Links.Self
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| type     | String   | &check;      |

#### Environments.Links
| **Name**  | **Type**                     | **Nullable** |
| --------- | ---------------------------- | ------------ |
| property1 | Environments.Links.Property1 | &check;      |
| property2 | Environments.Links.Property2 | &check;      |

#### Environments.Links.Property1
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| type     | String   | &check;      |

#### Environments.Links.Property2
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| type     | String   | &check;      |
