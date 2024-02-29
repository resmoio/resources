---
description: Asana Project
---
asana_project
-------------

| **Name**                               | **Type**                  | **Nullable** |
| -------------------------------------- | ------------------------- | ------------ |
| archived                               | Boolean                   | &cross;      |
| color                                  | String                    | &check;      |
| completed                              | Boolean                   | &cross;      |
| completed_at                           | String                    | &check;      |
| completed_by                           | User                      | &check;      |
| created_at                             | String                    | &cross;      |
| current_status_update                  | CurrentStatusUpdate       | &check;      |
| custom_field_settings                  | List<CustomFieldSettings> | &check;      |
| custom_fields                          | List<CustomField>         | &cross;      |
| default_access_level                   | String                    | &cross;      |
| default_view                           | String                    | &cross;      |
| due_date                               | String                    | &check;      |
| due_on                                 | String                    | &check;      |
| followers                              | List<User>                | &check;      |
| gid                                    | String                    | &cross;      |
| html_notes                             | String                    | &check;      |
| icon                                   | String                    | &check;      |
| members                                | List<User>                | &check;      |
| minimum_access_level_for_customization | String                    | &cross;      |
| minimum_access_level_for_sharing       | String                    | &cross;      |
| modified_at                            | String                    | &cross;      |
| name                                   | String                    | &cross;      |
| notes                                  | String                    | &cross;      |
| owner                                  | User                      | &check;      |
| permalink_url                          | String                    | &cross;      |
| public                                 | Boolean                   | &cross;      |
| resource_type                          | String                    | &cross;      |
| start_on                               | String                    | &check;      |
| team                                   | Team                      | &check;      |

#### CurrentStatusUpdate
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| gid              | String   | &cross;      |
| resource_subtype | String   | &cross;      |
| resource_type    | String   | &cross;      |
| title            | String   | &cross;      |

#### CustomField
| **Name**          | **Type**                      | **Nullable** |
| ----------------- | ----------------------------- | ------------ |
| date_value        | CustomField.DateValue         | &check;      |
| display_value     | String                        | &check;      |
| enabled           | Boolean                       | &cross;      |
| enum_options      | List<CustomField.EnumOptions> | &check;      |
| enum_value        | CustomField.EnumValue         | &check;      |
| gid               | String                        | &cross;      |
| is_formula_field  | Boolean                       | &cross;      |
| multi_enum_values | List<CustomField.EnumValue>   | &check;      |
| name              | String                        | &cross;      |
| number_value      | Int                           | &check;      |
| resource_type     | String                        | &cross;      |
| text_value        | String                        | &check;      |
| type              | String                        | &cross;      |

#### CustomField.DateValue
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| date      | String   | &cross;      |
| date_time | String   | &cross;      |

#### CustomField.EnumOptions
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| color         | String   | &cross;      |
| enabled       | Boolean  | &cross;      |
| gid           | String   | &cross;      |
| name          | String   | &cross;      |
| resource_type | String   | &cross;      |

#### CustomField.EnumValue
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| color         | String   | &cross;      |
| enabled       | Boolean  | &cross;      |
| gid           | String   | &cross;      |
| name          | String   | &cross;      |
| resource_type | String   | &cross;      |

#### CustomFieldSettings
| **Name**      | **Type**                   | **Nullable** |
| ------------- | -------------------------- | ------------ |
| gid           | String                     | &cross;      |
| is_important  | Boolean                    | &cross;      |
| parent        | CustomFieldSettings.Parent | &cross;      |
| resource_type | String                     | &cross;      |

#### CustomFieldSettings.Parent
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| gid           | String   | &cross;      |
| name          | String   | &cross;      |
| resource_type | String   | &cross;      |

#### Team
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| gid           | String   | &cross;      |
| name          | String   | &cross;      |
| resource_type | String   | &cross;      |

#### User
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| gid           | String   | &cross;      |
| name          | String   | &cross;      |
| resource_type | String   | &cross;      |
