---
description: WordPress Site
---
wordpress_site
--------------

| **Name**                    | **Type**        | **Nullable** |
| --------------------------- | --------------- | ------------ |
| ID                          | Int             | &cross;      |
| URL                         | String          | &check;      |
| capabilities                | Capabilities    | &check;      |
| description                 | String          | &check;      |
| is_coming_soon              | Boolean         | &check;      |
| is_core_site_editor_enabled | Boolean         | &check;      |
| is_following                | Boolean         | &check;      |
| is_fse_active               | Boolean         | &check;      |
| is_fse_eligible             | Boolean         | &check;      |
| is_multisite                | Boolean         | &check;      |
| is_private                  | Boolean         | &check;      |
| is_vip                      | Boolean         | &check;      |
| is_wpcom_atomic             | Boolean         | &check;      |
| is_wpcom_staging_site       | Boolean         | &check;      |
| jetpack                     | Boolean         | &check;      |
| jetpack_connection          | Boolean         | &check;      |
| lang                        | String          | &check;      |
| launch_status               | String          | &check;      |
| logo                        | Logo            | &check;      |
| meta                        | Meta            | &check;      |
| name                        | String          | &check;      |
| options                     | Options         | &check;      |
| organization_id             | Int             | &check;      |
| plan                        | Plan            | &check;      |
| post_count                  | Int             | &check;      |
| quota                       | Quota           | &check;      |
| single_user_site            | Boolean         | &check;      |
| site_owner                  | Int             | &check;      |
| subscribers_count           | Int             | &check;      |
| user_can_manage             | Boolean         | &check;      |
| user_interactions           | List<String>    | &check;      |
| visible                     | Boolean         | &check;      |
| was_ecommerce_trial         | Boolean         | &check;      |
| was_hosting_trial           | Boolean         | &check;      |
| was_migration_trial         | Boolean         | &check;      |
| was_upgraded_from_trial     | Boolean         | &check;      |
| zendesk_site_meta           | ZendeskSiteMeta | &check;      |

#### Capabilities
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| activate_plugins    | Boolean  | &check;      |
| activate_wordads    | Boolean  | &check;      |
| delete_others_posts | Boolean  | &check;      |
| delete_posts        | Boolean  | &check;      |
| delete_users        | Boolean  | &check;      |
| edit_others_pages   | Boolean  | &check;      |
| edit_others_posts   | Boolean  | &check;      |
| edit_pages          | Boolean  | &check;      |
| edit_posts          | Boolean  | &check;      |
| edit_theme_options  | Boolean  | &check;      |
| edit_users          | Boolean  | &check;      |
| list_users          | Boolean  | &check;      |
| manage_categories   | Boolean  | &check;      |
| manage_options      | Boolean  | &check;      |
| moderate_comments   | Boolean  | &check;      |
| own_site            | Boolean  | &check;      |
| promote_users       | Boolean  | &check;      |
| publish_posts       | Boolean  | &check;      |
| remove_users        | Boolean  | &check;      |
| upload_files        | Boolean  | &check;      |
| view_hosting        | Boolean  | &check;      |
| view_stats          | Boolean  | &check;      |

#### Logo
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| url      | String   | &check;      |

#### Meta
| **Name** | **Type**   | **Nullable** |
| -------- | ---------- | ------------ |
| links    | Meta.Links | &check;      |

#### Meta.Links
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| comments | String   | &check;      |
| help     | String   | &check;      |
| posts    | String   | &check;      |
| self     | String   | &check;      |
| xmlrpc   | String   | &check;      |

#### Options
| **Name**                             | **Type**                                | **Nullable** |
| ------------------------------------ | --------------------------------------- | ------------ |
| admin_url                            | String                                  | &check;      |
| advanced_seo_front_page_description  | String                                  | &check;      |
| allowed_file_types                   | List<String>                            | &check;      |
| anchor_podcast                       | Boolean                                 | &check;      |
| background_color                     | Boolean                                 | &check;      |
| blog_public                          | Int                                     | &check;      |
| blogging_prompts_settings            | Options.BloggingPromptsSettings         | &check;      |
| can_blaze                            | Boolean                                 | &check;      |
| created_at                           | String                                  | &check;      |
| default_category                     | Int                                     | &check;      |
| default_comment_status               | Boolean                                 | &check;      |
| default_likes_enabled                | Boolean                                 | &check;      |
| default_ping_status                  | Boolean                                 | &check;      |
| default_post_format                  | String                                  | &check;      |
| default_sharing_status               | Boolean                                 | &check;      |
| difm_lite_site_options               | Options.DifmLiteSiteOptions             | &check;      |
| editing_toolkit_is_active            | Boolean                                 | &check;      |
| featured_images_enabled              | Boolean                                 | &check;      |
| frame_nonce                          | String                                  | &check;      |
| gmt_offset                           | Int                                     | &check;      |
| header_image                         | Boolean                                 | &check;      |
| headstart                            | Boolean                                 | &check;      |
| headstart_is_fresh                   | Boolean                                 | &check;      |
| image_default_link_type              | String                                  | &check;      |
| image_large_height                   | Int                                     | &check;      |
| image_large_width                    | Int                                     | &check;      |
| image_medium_height                  | Int                                     | &check;      |
| image_medium_width                   | Int                                     | &check;      |
| image_thumbnail_crop                 | Int                                     | &check;      |
| image_thumbnail_height               | Int                                     | &check;      |
| image_thumbnail_width                | Int                                     | &check;      |
| is_automated_transfer                | Boolean                                 | &check;      |
| is_cloud_eligible                    | Boolean                                 | &check;      |
| is_commercial                        | Boolean                                 | &check;      |
| is_difm_lite_in_progress             | Boolean                                 | &check;      |
| is_domain_only                       | Boolean                                 | &check;      |
| is_mapped_domain                     | Boolean                                 | &check;      |
| is_pending_plan                      | Boolean                                 | &check;      |
| is_redirect                          | Boolean                                 | &check;      |
| is_wpcom_atomic                      | Boolean                                 | &check;      |
| is_wpcom_store                       | Boolean                                 | &check;      |
| is_wpforteams_site                   | Boolean                                 | &check;      |
| jetpack_frame_nonce                  | String                                  | &check;      |
| launchpad_checklist_tasks_statuses   | Options.LaunchpadChecklistTasksStatuses | &check;      |
| launchpad_screen                     | String                                  | &check;      |
| login_url                            | String                                  | &check;      |
| permalink_structure                  | String                                  | &check;      |
| publicize_permanently_disabled       | Boolean                                 | &check;      |
| show_on_front                        | String                                  | &check;      |
| site_intent                          | String                                  | &check;      |
| software_version                     | String                                  | &check;      |
| theme_slug                           | String                                  | &check;      |
| timezone                             | String                                  | &check;      |
| unmapped_url                         | String                                  | &check;      |
| updated_at                           | String                                  | &check;      |
| upgraded_filetypes_enabled           | Boolean                                 | &check;      |
| videopress_enabled                   | Boolean                                 | &check;      |
| videopress_storage_used              | Int                                     | &check;      |
| was_created_with_blank_canvas_design | Boolean                                 | &check;      |
| woocommerce_is_active                | Boolean                                 | &check;      |
| wordads                              | Boolean                                 | &check;      |
| wpcom_admin_interface                | String                                  | &check;      |
| wpcom_production_blog_id             | Int                                     | &check;      |
| wpcom_site_setup                     | Boolean                                 | &check;      |

#### Options.BloggingPromptsSettings
| **Name**                   | **Type**                                      | **Nullable** |
| -------------------------- | --------------------------------------------- | ------------ |
| is_potential_blogging_site | Boolean                                       | &check;      |
| prompts_card_opted_in      | Boolean                                       | &check;      |
| prompts_reminders_opted_in | Boolean                                       | &check;      |
| reminders_days             | Options.BloggingPromptsSettings.RemindersDays | &check;      |
| reminders_time             | String                                        | &check;      |

#### Options.BloggingPromptsSettings.RemindersDays
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| friday    | Boolean  | &check;      |
| monday    | Boolean  | &check;      |
| saturday  | Boolean  | &check;      |
| sunday    | Boolean  | &check;      |
| thursday  | Boolean  | &check;      |
| tuesday   | Boolean  | &check;      |
| wednesday | Boolean  | &check;      |

#### Options.DifmLiteSiteOptions
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |


#### Options.LaunchpadChecklistTasksStatuses
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| design_completed    | Boolean  | &check;      |
| site_launched       | Boolean  | &check;      |
| site_theme_selected | Boolean  | &check;      |

#### Plan
| **Name**           | **Type**      | **Nullable** |
| ------------------ | ------------- | ------------ |
| billing_period     | String        | &check;      |
| expired            | Boolean       | &check;      |
| features           | Plan.Features | &check;      |
| is_free            | Boolean       | &check;      |
| license_key        | String        | &check;      |
| product_id         | Int           | &check;      |
| product_name       | String        | &check;      |
| product_name_short | String        | &check;      |
| product_slug       | String        | &check;      |
| user_is_owner      | Boolean       | &check;      |

#### Plan.Features
| **Name**  | **Type**         | **Nullable** |
| --------- | ---------------- | ------------ |
| active    | List<String>     | &check;      |
| available | Map<String,List> | &check;      |

#### Quota
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| percent_used    | Double   | &check;      |
| space_allowed   | Long     | &check;      |
| space_available | Long     | &check;      |
| space_used      | Int      | &check;      |

#### ZendeskSiteMeta
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| plan     | String   | &check;      |
