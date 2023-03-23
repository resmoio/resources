---
description: CrowdStrike Detection
---
crowdstrike_detection
---------------------

| **Name**                 | **Type**       | **Nullable** |
| ------------------------ | -------------- | ------------ |
| adversary_ids            | List<Long>     | &check;      |
| assigned_to_name         | String         | &check;      |
| assigned_to_uid          | String         | &check;      |
| behaviors                | List<Behavior> | &check;      |
| behaviors_processed      | List<String>   | &check;      |
| cid                      | String         | &check;      |
| created_timestamp        | Date           | &check;      |
| detection_id             | String         | &cross;      |
| device                   | Device         | &check;      |
| email_sent               | Boolean        | &check;      |
| first_behavior           | String         | &check;      |
| hostinfo                 | HostInfo       | &check;      |
| last_behavior            | String         | &check;      |
| max_confidence           | Long           | &check;      |
| max_severity             | Long           | &check;      |
| max_severity_displayname | String         | &check;      |
| overwatch_notes          | String         | &check;      |
| quarantined_files        | List<Files>    | &check;      |
| seconds_to_resolve       | Long           | &check;      |
| seconds_to_triaged       | Long           | &check;      |
| show_in_ui               | Boolean        | &check;      |
| status                   | String         | &check;      |

#### Behavior
| **Name**                    | **Type**             | **Nullable** |
| --------------------------- | -------------------- | ------------ |
| alleged_filetype            | String               | &check;      |
| behavior_id                 | String               | &check;      |
| cmdline                     | String               | &check;      |
| confidence                  | Long                 | &check;      |
| container_id                | String               | &check;      |
| control_graph_id            | String               | &check;      |
| description                 | String               | &check;      |
| device_id                   | String               | &check;      |
| display_name                | String               | &check;      |
| filename                    | String               | &check;      |
| filepath                    | String               | &check;      |
| ioc_description             | String               | &check;      |
| ioc_source                  | String               | &check;      |
| ioc_type                    | String               | &check;      |
| ioc_value                   | String               | &check;      |
| md5                         | String               | &check;      |
| objective                   | String               | &check;      |
| parent_details              | Behavior.Parent      | &check;      |
| pattern_disposition         | Long                 | &check;      |
| pattern_disposition_details | Behavior.Disposition | &check;      |
| rule_instance_id            | String               | &check;      |
| rule_instance_version       | Long                 | &check;      |
| scenario                    | String               | &check;      |
| severity                    | Long                 | &check;      |
| sha256                      | String               | &check;      |
| tactic                      | String               | &check;      |
| tactic_id                   | String               | &check;      |
| technique                   | String               | &check;      |
| technique_id                | String               | &check;      |
| template_instance_id        | String               | &check;      |
| timestamp                   | String               | &check;      |
| triggering_process_graph_id | String               | &check;      |
| user_id                     | String               | &check;      |
| user_name                   | String               | &check;      |

#### Behavior.Disposition
| **Name**                         | **Type** | **Nullable** |
| -------------------------------- | -------- | ------------ |
| blocking_unsupported_or_disabled | Boolean  | &check;      |
| bootup_safeguard_enabled         | Boolean  | &check;      |
| critical_process_disabled        | Boolean  | &check;      |
| detect                           | Boolean  | &check;      |
| fs_operation_blocked             | Boolean  | &check;      |
| handle_operation_downgraded      | Boolean  | &check;      |
| inddet_mask                      | Boolean  | &check;      |
| indicator                        | Boolean  | &check;      |
| kill_action_failed               | Boolean  | &check;      |
| kill_parent                      | Boolean  | &check;      |
| kill_process                     | Boolean  | &check;      |
| kill_subprocess                  | Boolean  | &check;      |
| operation_blocked                | Boolean  | &check;      |
| policy_disabled                  | Boolean  | &check;      |
| process_blocked                  | Boolean  | &check;      |
| quarantine_file                  | Boolean  | &check;      |
| quarantine_machine               | Boolean  | &check;      |
| registry_operation_blocked       | Boolean  | &check;      |
| rooting                          | Boolean  | &check;      |
| sensor_only                      | Boolean  | &check;      |
| suspend_parent                   | Boolean  | &check;      |
| suspend_process                  | Boolean  | &check;      |

#### Behavior.Parent
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| parent_cmdline          | String   | &check;      |
| parent_md5              | String   | &check;      |
| parent_process_graph_id | String   | &check;      |
| parent_sha256           | String   | &check;      |

#### Device
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| device_id | String   | &check;      |
| hostname  | String   | &check;      |

#### Files
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| paths    | String   | &check;      |
| sha256   | String   | &check;      |
| state    | String   | &check;      |

#### HostInfo
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| domain   | String   | &check;      |
