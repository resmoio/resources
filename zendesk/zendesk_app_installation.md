---
description: Zendesk App Installation
---
zendesk_app_installation
------------------------

| **Name**                    | **Type**             | **Nullable** |
| --------------------------- | -------------------- | ------------ |
| account                     | String               | &check;      |
| app                         | App                  | &check;      |
| app_id                      | String               | &check;      |
| collapsible                 | Boolean              | &check;      |
| created_at                  | String               | &check;      |
| enabled                     | Boolean              | &check;      |
| group_restrictions          | List<Long>           | &check;      |
| has_incomplete_subscription | Boolean              | &check;      |
| has_unpaid_subscription     | Boolean              | &check;      |
| id                          | String               | &cross;      |
| paid                        | Boolean              | &check;      |
| plan_information            | PlanInformation      | &check;      |
| product                     | String               | &check;      |
| recurring_payment           | Boolean              | &check;      |
| role_restrictions           | List<Long>           | &check;      |
| settings                    | Settings             | &check;      |
| settings_objects            | List<SettingsObject> | &check;      |
| stripe_account              | String               | &check;      |
| stripe_subscription_id      | String               | &check;      |
| updated                     | String               | &check;      |
| updated_at                  | String               | &check;      |

#### App
| **Name**                      | **Type**        | **Nullable** |
| ----------------------------- | --------------- | ------------ |
| author_email                  | String          | &check;      |
| author_name                   | String          | &check;      |
| author_url                    | String          | &check;      |
| categories                    | List<Category>  | &check;      |
| closed_preview                | Boolean         | &check;      |
| created_at                    | String          | &check;      |
| default_locale                | String          | &check;      |
| deprecated                    | Boolean         | &check;      |
| feature_color                 | String          | &check;      |
| featured                      | Boolean         | &check;      |
| framework_version             | String          | &check;      |
| id                            | String          | &check;      |
| installable                   | Boolean         | &check;      |
| installation_instructions     | String          | &check;      |
| large_icon                    | String          | &check;      |
| long_description              | String          | &check;      |
| marketing_only                | Boolean         | &check;      |
| name                          | String          | &check;      |
| obsolete                      | Boolean         | &check;      |
| owner_id                      | String          | &check;      |
| paid                          | Boolean         | &check;      |
| parameters                    | List<Parameter> | &check;      |
| products                      | List<String>    | &check;      |
| promoted                      | Boolean         | &check;      |
| raw_installation_instructions | String          | &check;      |
| raw_long_description          | String          | &check;      |
| remote_installation_url       | String          | &check;      |
| screenshots                   | List<String>    | &check;      |
| short_description             | String          | &check;      |
| single_install                | Boolean         | &check;      |
| small_icon                    | String          | &check;      |
| state                         | String          | &check;      |
| terms_conditions_url          | String          | &check;      |
| updated_at                    | String          | &check;      |
| version                       | String          | &check;      |
| visibility                    | String          | &check;      |

#### Category
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Parameter
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| app_id        | String   | &check;      |
| created_at    | String   | &check;      |
| default_value | String   | &check;      |
| id            | String   | &check;      |
| kind          | String   | &check;      |
| name          | String   | &check;      |
| position      | Int      | &check;      |
| required      | Boolean  | &check;      |
| secure        | Boolean  | &check;      |
| updated_at    | String   | &check;      |

#### PlanInformation
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |

#### Settings
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| title    | String   | &check;      |

#### SettingsObject
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| value    | String   | &check;      |
