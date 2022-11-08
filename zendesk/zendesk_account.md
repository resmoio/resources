---
description: Zendesk Account
---
zendesk_account
---------------

| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| multiproduct | Boolean  | &check;      |
| name         | String   | &check;      |
| owner_id     | String   | &check;      |
| sandbox      | Boolean  | &check;      |
| settings     | Settings | &check;      |
| subdomain    | String   | &cross;      |
| time_format  | Int      | &check;      |
| time_zone    | String   | &check;      |
| url          | String   | &check;      |

#### ActiveFeatures
| **Name**                           | **Type** | **Nullable** |
| ---------------------------------- | -------- | ------------ |
| advanced_analytics                 | Boolean  | &check;      |
| agent_forwarding                   | Boolean  | &check;      |
| allow_ccs                          | Boolean  | &check;      |
| allow_email_template_customization | Boolean  | &check;      |
| automatic_answers                  | Boolean  | &check;      |
| bcc_archiving                      | Boolean  | &check;      |
| benchmark_opt_out                  | Boolean  | &check;      |
| business_hours                     | Boolean  | &check;      |
| chat                               | Boolean  | &check;      |
| chat_about_my_ticket               | Boolean  | &check;      |
| csat_reason_code                   | Boolean  | &check;      |
| custom_dkim_domain                 | Boolean  | &check;      |
| customer_context_as_default        | Boolean  | &check;      |
| customer_satisfaction              | Boolean  | &check;      |
| dynamic_contents                   | Boolean  | &check;      |
| explore                            | Boolean  | &check;      |
| explore_on_support_ent_plan        | Boolean  | &check;      |
| explore_on_support_pro_plan        | Boolean  | &check;      |
| facebook                           | Boolean  | &check;      |
| facebook_login                     | Boolean  | &check;      |
| fallback_composer                  | Boolean  | &check;      |
| forum_analytics                    | Boolean  | &check;      |
| good_data_and_explore              | Boolean  | &check;      |
| google_login                       | Boolean  | &check;      |
| insights                           | Boolean  | &check;      |
| is_abusive                         | Boolean  | &check;      |
| light_agents                       | Boolean  | &check;      |
| markdown                           | Boolean  | &check;      |
| on_hold_status                     | Boolean  | &check;      |
| rich_content_in_emails             | Boolean  | &check;      |
| sandbox                            | Boolean  | &check;      |
| satisfaction_prediction            | Boolean  | &check;      |
| suspended_ticket_notification      | Boolean  | &check;      |
| ticket_forms                       | Boolean  | &check;      |
| ticket_tagging                     | Boolean  | &check;      |
| topic_suggestion                   | Boolean  | &check;      |
| twitter                            | Boolean  | &check;      |
| twitter_login                      | Boolean  | &check;      |
| user_org_fields                    | Boolean  | &check;      |
| user_tagging                       | Boolean  | &check;      |
| voice                              | Boolean  | &check;      |

#### Agents
| **Name**                        | **Type** | **Nullable** |
| ------------------------------- | -------- | ------------ |
| agent_workspace                 | Boolean  | &check;      |
| aw_self_serve_migration_enabled | Boolean  | &check;      |
| focus_mode                      | Boolean  | &check;      |
| idle_timeout_enabled            | Boolean  | &check;      |
| unified_agent_statuses          | Boolean  | &check;      |

#### Api
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| accepted_api_agreement | Boolean  | &check;      |
| api_password_access    | String   | &check;      |
| api_token_access       | String   | &check;      |

#### Apps
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| create_private | Boolean  | &check;      |
| create_public  | Boolean  | &check;      |
| use            | Boolean  | &check;      |

#### Billing
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| backend  | String   | &check;      |

#### Branding
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| favicon_url           | String   | &check;      |
| header_color          | String   | &check;      |
| header_logo_url       | String   | &check;      |
| page_background_color | String   | &check;      |
| tab_background_color  | String   | &check;      |
| text_color            | String   | &check;      |

#### Brands
| **Name**                     | **Type** | **Nullable** |
| ---------------------------- | -------- | ------------ |
| default_brand_id             | String   | &check;      |
| require_brand_on_new_tickets | Boolean  | &check;      |

#### Cdn
| **Name**              | **Type**   | **Nullable** |
| --------------------- | ---------- | ------------ |
| cdn_provider          | String     | &check;      |
| fallback_cdn_provider | String     | &check;      |
| hosts                 | List<Host> | &check;      |

#### Chat
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| available             | Boolean  | &check;      |
| enabled               | Boolean  | &check;      |
| integrated            | Boolean  | &check;      |
| maximum_request_count | Int      | &check;      |
| welcome_message       | String   | &check;      |

#### CrossSell
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| show_chat_tooltip | Boolean  | &check;      |
| xsell_source      | String   | &check;      |

#### GooddataAdvancedAnalytics
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### GoogleApps
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| has_google_apps       | Boolean  | &check;      |
| has_google_apps_admin | Boolean  | &check;      |

#### Groups
| **Name**                    | **Type** | **Nullable** |
| --------------------------- | -------- | ------------ |
| check_group_name_uniqueness | Boolean  | &check;      |

#### Host
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| url      | String   | &check;      |

#### Limits
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| attachment_size | Int      | &check;      |

#### Localization
| **Name**   | **Type**     | **Nullable** |
| ---------- | ------------ | ------------ |
| locale_ids | List<String> | &check;      |

#### Lotus
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| pod_id       | String   | &check;      |
| prefer_lotus | Boolean  | &check;      |
| reporting    | Boolean  | &check;      |

#### Metrics
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| account_size | String   | &check;      |

#### Onboarding
| **Name**                     | **Type** | **Nullable** |
| ---------------------------- | -------- | ------------ |
| checklist_onboarding_version | Int      | &check;      |
| onboarding_segments          | String   | &check;      |
| product_sign_up              | String   | &check;      |

#### Routing
| **Name**                       | **Type** | **Nullable** |
| ------------------------------ | -------- | ------------ |
| autorouting_tag                | String   | &check;      |
| enabled                        | Boolean  | &check;      |
| max_email_capacity             | Int      | &check;      |
| max_messaging_capacity         | Int      | &check;      |
| reassignment_messaging_enabled | Boolean  | &check;      |
| reassignment_messaging_timeout | Int      | &check;      |
| reassignment_talk_timeout      | Int      | &check;      |

#### Rule
| **Name**                   | **Type**     | **Nullable** |
| -------------------------- | ------------ | ------------ |
| macro_most_used            | Boolean      | &check;      |
| macro_order                | String       | &check;      |
| skill_based_filtered_views | List<String> | &check;      |
| using_skill_based_routing  | Boolean      | &check;      |

#### Settings
| **Name**                    | **Type**                  | **Nullable** |
| --------------------------- | ------------------------- | ------------ |
| active_features             | ActiveFeatures            | &check;      |
| agents                      | Agents                    | &check;      |
| api                         | Api                       | &check;      |
| apps                        | Apps                      | &check;      |
| billing                     | Billing                   | &check;      |
| branding                    | Branding                  | &check;      |
| brands                      | Brands                    | &check;      |
| cdn                         | Cdn                       | &check;      |
| chat                        | Chat                      | &check;      |
| cross_sell                  | CrossSell                 | &check;      |
| gooddata_advanced_analytics | GooddataAdvancedAnalytics | &check;      |
| google_apps                 | GoogleApps                | &check;      |
| groups                      | Groups                    | &check;      |
| limits                      | Limits                    | &check;      |
| localization                | Localization              | &check;      |
| lotus                       | Lotus                     | &check;      |
| metrics                     | Metrics                   | &check;      |
| onboarding                  | Onboarding                | &check;      |
| routing                     | Routing                   | &check;      |
| rule                        | Rule                      | &check;      |
| side_conversations          | SideConversations         | &check;      |
| statistics                  | Statistics                | &check;      |
| ticket_form                 | TicketForm                | &check;      |
| ticket_sharing_partners     | TicketSharingPartners     | &check;      |
| tickets                     | Tickets                   | &check;      |
| twitter                     | Twitter                   | &check;      |
| user                        | User                      | &check;      |
| voice                       | Voice                     | &check;      |

#### SideConversations
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| show_in_context_panel | Boolean  | &check;      |

#### Statistics
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| forum      | Boolean  | &check;      |
| rule_usage | Boolean  | &check;      |
| search     | Boolean  | &check;      |

#### TicketForm
| **Name**                      | **Type** | **Nullable** |
| ----------------------------- | -------- | ------------ |
| raw_ticket_forms_instructions | String   | &check;      |
| ticket_forms_instructions     | String   | &check;      |

#### TicketSharingPartners
| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| support_addresses | List<String> | &check;      |

#### Tickets
| **Name**                             | **Type** | **Nullable** |
| ------------------------------------ | -------- | ------------ |
| accepted_new_collaboration_tos       | Boolean  | &check;      |
| agent_collision                      | Boolean  | &check;      |
| agent_ticket_deletion                | Boolean  | &check;      |
| allow_group_reset                    | Boolean  | &check;      |
| assign_default_organization          | Boolean  | &check;      |
| assign_tickets_upon_solve            | Boolean  | &check;      |
| auto_updated_ccs_followers_rules     | Boolean  | &check;      |
| collaboration                        | Boolean  | &check;      |
| comments_public_by_default           | Boolean  | &check;      |
| email_attachments                    | Boolean  | &check;      |
| emoji_autocompletion                 | Boolean  | &check;      |
| follower_and_email_cc_collaborations | Boolean  | &check;      |
| has_color_text                       | Boolean  | &check;      |
| is_first_comment_private_enabled     | Boolean  | &check;      |
| light_agent_email_ccs_allowed        | Boolean  | &check;      |
| list_empty_views                     | Boolean  | &check;      |
| list_newest_comments_first           | Boolean  | &check;      |
| markdown_ticket_comments             | Boolean  | &check;      |
| maximum_personal_views_to_list       | Int      | &check;      |
| private_attachments                  | Boolean  | &check;      |
| rich_text_comments                   | Boolean  | &check;      |
| status_hold                          | Boolean  | &check;      |
| tagging                              | Boolean  | &check;      |
| using_skill_based_routing            | Boolean  | &check;      |

#### Twitter
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| shorten_url | String   | &check;      |

#### User
| **Name**                         | **Type** | **Nullable** |
| -------------------------------- | -------- | ------------ |
| agent_created_welcome_emails     | Boolean  | &check;      |
| end_user_phone_number_validation | Boolean  | &check;      |
| have_gravatars_enabled           | Boolean  | &check;      |
| language_selection               | Boolean  | &check;      |
| multiple_organizations           | Boolean  | &check;      |
| tagging                          | Boolean  | &check;      |
| time_zone_selection              | Boolean  | &check;      |

#### Voice
| **Name**                           | **Type** | **Nullable** |
| ---------------------------------- | -------- | ------------ |
| agent_confirmation_when_forwarding | Boolean  | &check;      |
| agent_wrap_up_after_calls          | Boolean  | &check;      |
| enabled                            | Boolean  | &check;      |
| logging                            | Boolean  | &check;      |
| maximum_queue_size                 | Int      | &check;      |
| maximum_queue_wait_time            | Int      | &check;      |
| only_during_business_hours         | Boolean  | &check;      |
| outbound_enabled                   | Boolean  | &check;      |
| recordings_public                  | Boolean  | &check;      |
| uk_mobile_forwarding               | Boolean  | &check;      |
