---
description: Segment Destination
---
segment_destination
-------------------

| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| enabled     | Boolean  | &check;      |
| id          | String   | &cross;      |
| metadata    | Metadata | &check;      |
| name        | String   | &check;      |
| settings    | Settings | &check;      |
| sourceId    | String   | &check;      |
| workspaceId | String   | &check;      |

#### Action
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| defaultTrigger | String   | &check;      |
| description    | String   | &check;      |
| fields         | Fields   | &cross;      |
| hidden         | Boolean  | &check;      |
| id             | String   | &check;      |
| name           | String   | &check;      |
| platform       | String   | &check;      |
| slug           | String   | &check;      |

#### Component
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | String   | &check;      |
| type     | String   | &check;      |

#### Fields
| **Name**    | **Type**           | **Nullable** |
| ----------- | ------------------ | ------------ |
| allowNull   | Boolean            | &check;      |
| choices     | Map<String,String> | &check;      |
| description | String             | &check;      |
| dynamic     | Boolean            | &check;      |
| fieldKey    | String             | &check;      |
| id          | String             | &check;      |
| label       | String             | &check;      |
| multiple    | Boolean            | &check;      |
| placeholder | String             | &check;      |
| required    | Boolean            | &check;      |
| sortOrder   | Long               | &check;      |
| type        | String             | &check;      |

#### Logos
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| default  | String   | &check;      |
| mark     | String   | &check;      |

#### Metadata
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| actions            | List<Action>       | &check;      |
| categories         | List<String>       | &check;      |
| components         | List<Component>    | &check;      |
| description        | String             | &check;      |
| id                 | String             | &check;      |
| logos              | Logos              | &check;      |
| name               | String             | &check;      |
| options            | List<Option>       | &check;      |
| presets            | List<Preset>       | &check;      |
| previousNames      | List<String>       | &check;      |
| slug               | String             | &check;      |
| status             | String             | &check;      |
| supportedFeatures  | SupportedFeatures  | &check;      |
| supportedMethods   | SupportedMethods   | &check;      |
| supportedPlatforms | SupportedPlatforms | &check;      |
| website            | String             | &check;      |

#### Option
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| label       | String   | &check;      |
| name        | String   | &check;      |
| required    | Boolean  | &check;      |
| type        | String   | &check;      |

#### Preset
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| actionId | String       | &check;      |
| fields   | List<String> | &check;      |
| name     | String       | &check;      |
| trigger  | String       | &check;      |

#### Settings
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| region      | String   | &check;      |
| roleAddress | String   | &check;      |
| secretId    | String   | &check;      |
| stream      | String   | &check;      |

#### SupportedFeatures
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| browserUnbundling       | Boolean  | &check;      |
| browserUnbundlingPublic | Boolean  | &check;      |
| cloudModeInstances      | String   | &check;      |
| deviceModeInstances     | String   | &check;      |
| replay                  | Boolean  | &check;      |

#### SupportedMethods
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| alias    | Boolean  | &check;      |
| group    | Boolean  | &check;      |
| identify | Boolean  | &check;      |
| pageview | Boolean  | &check;      |
| track    | Boolean  | &check;      |

#### SupportedPlatforms
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| browser  | Boolean  | &check;      |
| mobile   | Boolean  | &check;      |
| server   | Boolean  | &check;      |
