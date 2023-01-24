---
description: Mixpanel Schema
---
mixpanel_schema
---------------

| **Name**   | **Type**   | **Nullable** |
| ---------- | ---------- | ------------ |
| entityType | String     | &cross;      |
| name       | String     | &check;      |
| projectId  | String     | &cross;      |
| schemaJson | SchemaJson | &check;      |

#### SchemaJson
| **Name**   | **Type**              | **Nullable** |
| ---------- | --------------------- | ------------ |
| metadata   | SchemaJson.Metadata   | &check;      |
| properties | SchemaJson.Properties | &check;      |

#### SchemaJson.Metadata
| **Name**    | **Type**                        | **Nullable** |
| ----------- | ------------------------------- | ------------ |
| comMixpanel | SchemaJson.Metadata.ComMixpanel | &check;      |

#### SchemaJson.Metadata.ComMixpanel
| **Name**    | **Type**                                    | **Nullable** |
| ----------- | ------------------------------------------- | ------------ |
| displayName | String                                      | &check;      |
| dropped     | Boolean                                     | &check;      |
| hidden      | Boolean                                     | &check;      |
| owners      | List<SchemaJson.Metadata.ComMixpanel.Owner> | &check;      |
| source      | String                                      | &check;      |
| tags        | List<String>                                | &check;      |

#### SchemaJson.Metadata.ComMixpanel.Owner
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| name     | String   | &check;      |

#### SchemaJson.Properties
| **Name**       | **Type**                             | **Nullable** |
| -------------- | ------------------------------------ | ------------ |
| additionalProp | SchemaJson.Properties.AdditionalProp | &check;      |

#### SchemaJson.Properties.AdditionalProp
| **Name**    | **Type**                                      | **Nullable** |
| ----------- | --------------------------------------------- | ------------ |
| description | String                                        | &check;      |
| metadata    | SchemaJson.Properties.AdditionalProp.Metadata | &check;      |

#### SchemaJson.Properties.AdditionalProp.Metadata
| **Name**    | **Type**                                                  | **Nullable** |
| ----------- | --------------------------------------------------------- | ------------ |
| comMixpanel | SchemaJson.Properties.AdditionalProp.Metadata.ComMixpanel | &check;      |

#### SchemaJson.Properties.AdditionalProp.Metadata.ComMixpanel
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| dropped     | Boolean  | &check;      |
| hidden      | Boolean  | &check;      |
