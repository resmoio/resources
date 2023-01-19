---
description: Trello Board
---
trello_board
------------

| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| closed            | Boolean      | &check;      |
| creationMethod    | String       | &check;      |
| dateClosed        | String       | &check;      |
| dateLastActivity  | String       | &check;      |
| dateLastView      | String       | &check;      |
| datePluginDisable | String       | &check;      |
| desc              | String       | &check;      |
| descData          | String       | &check;      |
| enterpriseOwned   | Boolean      | &check;      |
| id                | String       | &cross;      |
| idBoardSource     | String       | &check;      |
| idEnterprise      | String       | &check;      |
| idMemberCreator   | String       | &check;      |
| idOrganization    | String       | &cross;      |
| idTags            | List<String> | &check;      |
| ixUpdate          | String       | &check;      |
| labelNames        | LabelNames   | &check;      |
| limits            | Limits       | &check;      |
| members           | List<Member> | &check;      |
| name              | String       | &check;      |
| nodeId            | String       | &check;      |
| pinned            | Boolean      | &check;      |
| prefs             | Prefs        | &check;      |
| premiumFeatures   | List<String> | &check;      |
| shortLink         | String       | &check;      |
| shortUrl          | String       | &check;      |
| starred           | Boolean      | &check;      |
| subscribed        | Boolean      | &check;      |
| templateGallery   | String       | &check;      |
| url               | String       | &check;      |

#### Attachments
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| perBoard | PerField | &check;      |
| perCard  | PerField | &check;      |

#### BackgroundImageScaled
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| height   | Long     | &check;      |
| url      | String   | &check;      |
| width    | Long     | &check;      |

#### Boards
| **Name**                    | **Type** | **Nullable** |
| --------------------------- | -------- | ------------ |
| totalAccessRequestsPerBoard | PerField | &check;      |
| totalMembersPerBoard        | PerField | &check;      |

#### Cards
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| openPerBoard  | PerField | &check;      |
| openPerList   | PerField | &check;      |
| totalPerBoard | PerField | &check;      |
| totalPerList  | PerField | &check;      |

#### CheckItems
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| perChecklist | PerField | &check;      |

#### Checklists
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| perBoard | PerField | &check;      |
| perCard  | PerField | &check;      |

#### CustomFieldOptions
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| perField | PerField | &check;      |

#### CustomFields
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| perBoard | PerField | &check;      |

#### LabelNames
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| black        | String   | &check;      |
| black_dark   | String   | &check;      |
| black_light  | String   | &check;      |
| blue         | String   | &check;      |
| blue_dark    | String   | &check;      |
| blue_light   | String   | &check;      |
| green        | String   | &check;      |
| green_dark   | String   | &check;      |
| green_light  | String   | &check;      |
| lime         | String   | &check;      |
| lime_dark    | String   | &check;      |
| lime_light   | String   | &check;      |
| orange       | String   | &check;      |
| orange_dark  | String   | &check;      |
| orange_light | String   | &check;      |
| pink         | String   | &check;      |
| pink_dark    | String   | &check;      |
| pink_light   | String   | &check;      |
| purple       | String   | &check;      |
| purple_dark  | String   | &check;      |
| purple_light | String   | &check;      |
| red          | String   | &check;      |
| red_dark     | String   | &check;      |
| red_light    | String   | &check;      |
| sky          | String   | &check;      |
| sky_dark     | String   | &check;      |
| sky_light    | String   | &check;      |
| yellow       | String   | &check;      |
| yellow_dark  | String   | &check;      |
| yellow_light | String   | &check;      |

#### Labels
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| perBoard | PerField | &check;      |

#### Limits
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| attachments        | Attachments        | &check;      |
| boards             | Boards             | &check;      |
| cards              | Cards              | &check;      |
| checkItems         | CheckItems         | &check;      |
| checklists         | Checklists         | &check;      |
| customFieldOptions | CustomFieldOptions | &check;      |
| customFields       | CustomFields       | &check;      |
| labels             | Labels             | &check;      |
| lists              | Lists              | &check;      |
| reactions          | Reactions          | &check;      |
| stickers           | Stickers           | &check;      |

#### Lists
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| openPerBoard  | PerField | &check;      |
| totalPerBoard | PerField | &check;      |

#### Member
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| activityBlocked    | Boolean  | &check;      |
| avatarHash         | String   | &check;      |
| avatarUrl          | String   | &check;      |
| deactivated        | Boolean  | &check;      |
| fullName           | String   | &check;      |
| id                 | String   | &cross;      |
| idMemberReferrer   | String   | &check;      |
| initials           | String   | &check;      |
| memberType         | String   | &check;      |
| membershipId       | String   | &check;      |
| nonPublicAvailable | String   | &check;      |
| unconfirmed        | Boolean  | &check;      |
| username           | String   | &check;      |

#### PerField
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| disableAt | Long     | &check;      |
| status    | String   | &check;      |
| warnAt    | Long     | &check;      |

#### Prefs
| **Name**                 | **Type**                    | **Nullable** |
| ------------------------ | --------------------------- | ------------ |
| background               | String                      | &check;      |
| backgroundBottomColor    | String                      | &check;      |
| backgroundBrightness     | String                      | &check;      |
| backgroundColor          | String                      | &check;      |
| backgroundImage          | String                      | &check;      |
| backgroundImageScaled    | List<BackgroundImageScaled> | &check;      |
| backgroundTile           | Boolean                     | &check;      |
| backgroundTopColor       | String                      | &check;      |
| calendarFeedEnabled      | Boolean                     | &check;      |
| canBeEnterprise          | Boolean                     | &check;      |
| canBeOrg                 | Boolean                     | &check;      |
| canBePrivate             | Boolean                     | &check;      |
| canBePublic              | Boolean                     | &check;      |
| canInvite                | Boolean                     | &check;      |
| cardAging                | String                      | &check;      |
| cardCovers               | Boolean                     | &check;      |
| comments                 | String                      | &check;      |
| hiddenPluginBoardButtons | List<String>                | &check;      |
| hideVotes                | Boolean                     | &check;      |
| invitations              | String                      | &check;      |
| isTemplate               | Boolean                     | &check;      |
| permissionLevel          | String                      | &check;      |
| selfJoin                 | Boolean                     | &check;      |
| switcherViews            | List<SwitcherView>          | &check;      |
| voting                   | String                      | &check;      |

#### Reactions
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| perAction       | PerField | &check;      |
| uniquePerAction | PerField | &check;      |

#### Stickers
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| perCard  | PerField | &check;      |

#### SwitcherView
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| _id      | String   | &check;      |
| enabled  | Boolean  | &check;      |
| id       | String   | &check;      |
| typeName | String   | &check;      |
| viewType | String   | &check;      |
