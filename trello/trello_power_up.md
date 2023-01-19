---
description: Trello Power Up
---
trello_power_up
---------------

| **Name**                        | **Type**      | **Nullable** |
| ------------------------------- | ------------- | ------------ |
| author                          | String        | &check;      |
| capabilities                    | List<String>  | &check;      |
| capabilitiesOptions             | List<String>  | &check;      |
| categories                      | List<String>  | &check;      |
| claimedDomains                  | List<String>  | &check;      |
| icon                            | Icon          | &check;      |
| id                              | String        | &cross;      |
| idOrganizationOwner             | String        | &check;      |
| iframeConnectorUrl              | String        | &check;      |
| isCompliantWithPrivacyStandards | Boolean       | &check;      |
| listing                         | Listing       | &check;      |
| moderatedState                  | String        | &check;      |
| name                            | String        | &check;      |
| privacyUrl                      | String        | &check;      |
| public                          | Boolean       | &check;      |
| supportEmail                    | String        | &check;      |
| tags                            | List<String>  | &check;      |
| url                             | String        | &check;      |
| usageBrackets                   | UsageBrackets | &check;      |

#### Icon
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| url      | String   | &check;      |

#### Listing
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| locale   | String   | &check;      |
| name     | String   | &check;      |
| overview | String   | &check;      |

#### UsageBrackets
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| boards   | Long     | &check;      |
