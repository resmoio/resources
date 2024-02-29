---
description: Zendesk Custom Role
---
zendesk_custom_role
-------------------

| **Name**          | **Type**      | **Nullable** |
| ----------------- | ------------- | ------------ |
| account           | String        | &check;      |
| configuration     | Configuration | &check;      |
| created_at        | String        | &check;      |
| description       | String        | &check;      |
| id                | String        | &cross;      |
| name              | String        | &cross;      |
| role_type         | String        | &check;      |
| team_member_count | Int           | &check;      |
| updated_at        | String        | &check;      |

#### Configuration
| **Name**                         | **Type** | **Nullable** |
| -------------------------------- | -------- | ------------ |
| assign_tickets_to_any_group      | Boolean  | &check;      |
| chat_access                      | Boolean  | &check;      |
| end_user_list_access             | String   | &check;      |
| end_user_profile_access          | String   | &check;      |
| explore_access                   | String   | &check;      |
| forum_access                     | String   | &check;      |
| forum_access_restricted_content  | Boolean  | &check;      |
| group_access                     | Boolean  | &check;      |
| light_agent                      | Boolean  | &check;      |
| macro_access                     | String   | &check;      |
| manage_automations               | Boolean  | &check;      |
| manage_business_rules            | Boolean  | &check;      |
| manage_contextual_workspaces     | Boolean  | &check;      |
| manage_dynamic_content           | Boolean  | &check;      |
| manage_extensions_and_channels   | Boolean  | &check;      |
| manage_facebook                  | Boolean  | &check;      |
| manage_group_memberships         | Boolean  | &check;      |
| manage_groups                    | Boolean  | &check;      |
| manage_macro_content_suggestions | Boolean  | &check;      |
| manage_organization_fields       | Boolean  | &check;      |
| manage_organizations             | Boolean  | &check;      |
| manage_roles                     | String   | &check;      |
| manage_skills                    | Boolean  | &check;      |
| manage_slas                      | Boolean  | &check;      |
| manage_suspended_tickets         | Boolean  | &check;      |
| manage_ticket_fields             | Boolean  | &check;      |
| manage_ticket_forms              | Boolean  | &check;      |
| manage_triggers                  | Boolean  | &check;      |
| manage_user_fields               | Boolean  | &check;      |
| moderate_forums                  | Boolean  | &check;      |
| organization_editing             | Boolean  | &check;      |
| organization_notes_editing       | Boolean  | &check;      |
| read_macro_content_suggestions   | Boolean  | &check;      |
| report_access                    | String   | &check;      |
| side_conversation_create         | Boolean  | &check;      |
| ticket_access                    | String   | &check;      |
| ticket_comment_access            | String   | &check;      |
| ticket_deletion                  | Boolean  | &check;      |
| ticket_editing                   | Boolean  | &check;      |
| ticket_merge                     | Boolean  | &check;      |
| ticket_redaction                 | Boolean  | &check;      |
| ticket_tag_editing               | Boolean  | &check;      |
| twitter_search_access            | Boolean  | &check;      |
| user_view_access                 | String   | &check;      |
| view_access                      | String   | &check;      |
| view_deleted_tickets             | Boolean  | &check;      |
| view_filter_tickets              | Boolean  | &check;      |
| view_reduced_count               | Boolean  | &check;      |
| voice_access                     | Boolean  | &check;      |
| voice_dashboard_access           | Boolean  | &check;      |
