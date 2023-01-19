---
description: Trello Member
---
trello_member
-------------

| **Name**                          | **Type**       | **Nullable** |
| --------------------------------- | -------------- | ------------ |
| aaBlockSyncUntil                  | String         | &check;      |
| aaEmail                           | String         | &check;      |
| aaEnrolledDate                    | String         | &check;      |
| aaId                              | String         | &check;      |
| activityBlocked                   | Boolean        | &check;      |
| avatarHash                        | String         | &check;      |
| avatarSource                      | String         | &check;      |
| avatarUrl                         | String         | &check;      |
| bio                               | String         | &check;      |
| confirmed                         | Boolean        | &check;      |
| credentialsRemovedCount           | Long           | &check;      |
| domainClaimed                     | String         | &check;      |
| email                             | String         | &check;      |
| fullName                          | String         | &check;      |
| goldSunsetFreeTrialIdOrganization | String         | &check;      |
| gravatarHash                      | String         | &check;      |
| id                                | String         | &cross;      |
| idBoards                          | List<String>   | &check;      |
| idEnterprise                      | String         | &check;      |
| idEnterprisesAdmin                | List<String>   | &check;      |
| idEnterprisesDeactivated          | List<String>   | &check;      |
| idMemberReferrer                  | String         | &check;      |
| idPremOrgsAdmin                   | List<String>   | &check;      |
| initials                          | String         | &check;      |
| isAaMastered                      | Boolean        | &check;      |
| ixUpdate                          | String         | &check;      |
| limits                            | Limits         | &check;      |
| loginTypes                        | List<String>   | &check;      |
| marketingOptIn                    | MarketingOptIn | &check;      |
| memberType                        | String         | &check;      |
| membership                        | Membership     | &check;      |
| messagesDismissed                 | List<String>   | &check;      |
| nonPublic                         | JSON           | &check;      |
| nonPublicAvailable                | Boolean        | &check;      |
| oneTimeMessagesDismissed          | List<String>   | &check;      |
| organizationId                    | String         | &check;      |
| prefs                             | Prefs          | &check;      |
| premiumFeatures                   | List<String>   | &check;      |
| products                          | List<String>   | &check;      |
| status                            | String         | &check;      |
| trophies                          | List<String>   | &check;      |
| uploadedAvatarHash                | String         | &check;      |
| uploadedAvatarUrl                 | String         | &check;      |
| url                               | String         | &check;      |
| username                          | String         | &check;      |

#### Boards
| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| totalPerMember | TotalPerMember | &check;      |

#### Limits
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| boards   | Boards   | &check;      |
| orgs     | Orgs     | &check;      |

#### MarketingOptIn
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| date     | String   | &check;      |
| optedIn  | Boolean  | &check;      |

#### Membership
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| deactivated | Boolean  | &check;      |
| id          | String   | &cross;      |
| memberType  | String   | &check;      |
| unconfirmed | Boolean  | &check;      |

#### Orgs
| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| totalPerMember | TotalPerMember | &check;      |

#### Prefs
| **Name**                      | **Type** | **Nullable** |
| ----------------------------- | -------- | ------------ |
| colorBlind                    | Boolean  | &check;      |
| locale                        | String   | &check;      |
| minutesBeforeDeadlineToNotify | Long     | &check;      |
| minutesBetweenSummaries       | Long     | &check;      |
| privacy                       | Privacy  | &check;      |
| sendSummaries                 | Boolean  | &check;      |

#### Privacy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| avatar   | String   | &check;      |
| fullName | String   | &check;      |

#### TotalPerMember
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| disableAt | Long     | &check;      |
| status    | String   | &check;      |
| warnAt    | Long     | &check;      |
