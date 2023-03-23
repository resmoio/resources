---
description: CrowdStrike Host
---
crowdstrike_host
----------------

| **Name**                     | **Type**     | **Nullable** |
| ---------------------------- | ------------ | ------------ |
| agent_load_flag              | String       | &check;      |
| agent_local_time             | String       | &check;      |
| agent_version                | String       | &check;      |
| bios_manufacturer            | String       | &check;      |
| bios_version                 | String       | &check;      |
| build_number                 | String       | &check;      |
| chassis_type                 | String       | &check;      |
| chassis_type_desc            | String       | &check;      |
| cid                          | String       | &check;      |
| config_id_base               | String       | &check;      |
| config_id_build              | String       | &check;      |
| config_id_platform           | String       | &check;      |
| cpu_signature                | String       | &check;      |
| detection_suppression_status | String       | &check;      |
| device_id                    | String       | &cross;      |
| device_policies              | DevicePolicy | &check;      |
| email                        | String       | &check;      |
| external_ip                  | String       | &check;      |
| first_login_timestamp        | String       | &check;      |
| first_seen                   | String       | &check;      |
| group_hash                   | String       | &check;      |
| groups                       | List<String> | &check;      |
| host_hidden_status           | String       | &check;      |
| hostname                     | String       | &check;      |
| instance_id                  | String       | &check;      |
| internet_exposure            | String       | &check;      |
| kernel_version               | String       | &check;      |
| last_login_timestamp         | String       | &check;      |
| last_seen                    | String       | &check;      |
| local_ip                     | String       | &check;      |
| mac_address                  | String       | &check;      |
| machine_domain               | String       | &check;      |
| major_version                | String       | &check;      |
| managed_apps                 | ManagedApps  | &check;      |
| meta                         | Meta         | &check;      |
| minor_version                | String       | &check;      |
| modified_timestamp           | String       | &check;      |
| notes                        | List<String> | &check;      |
| os_build                     | String       | &check;      |
| os_version                   | String       | &check;      |
| ou                           | List<String> | &check;      |
| platform_id                  | String       | &check;      |
| platform_name                | String       | &check;      |
| pod_annotations              | List<String> | &check;      |
| pod_host_ip4                 | String       | &check;      |
| pod_host_ip6                 | String       | &check;      |
| pod_hostname                 | String       | &check;      |
| pod_id                       | String       | &check;      |
| pod_ip4                      | String       | &check;      |
| pod_ip6                      | String       | &check;      |
| pod_labels                   | List<String> | &check;      |
| pod_name                     | String       | &check;      |
| pod_namespace                | String       | &check;      |
| pod_service_account_name     | String       | &check;      |
| pointer_size                 | String       | &check;      |
| policies                     | List<Policy> | &check;      |
| product_type                 | String       | &check;      |
| product_type_desc            | String       | &check;      |
| provision_status             | String       | &check;      |
| reduced_functionality_mode   | String       | &check;      |
| release_group                | String       | &check;      |
| serial_number                | String       | &check;      |
| service_pack_major           | String       | &check;      |
| service_pack_minor           | String       | &check;      |
| service_provider             | String       | &check;      |
| service_provider_account_id  | String       | &check;      |
| site_name                    | String       | &check;      |
| status                       | String       | &check;      |
| system_manufacturer          | String       | &check;      |
| system_product_name          | String       | &check;      |
| tags                         | List<String> | &check;      |
| zone_group                   | String       | &check;      |

#### DevicePolicy
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| airlock             | Policy   | &check;      |
| automox             | Policy   | &check;      |
| device_control      | Policy   | &check;      |
| fim                 | Policy   | &check;      |
| firewall            | Policy   | &check;      |
| global_config       | Policy   | &check;      |
| identity_protection | Policy   | &check;      |
| jumpcloud           | Policy   | &check;      |
| mobile              | Policy   | &check;      |
| netskope            | Policy   | &check;      |
| prevention          | Policy   | &check;      |
| remote_response     | Policy   | &check;      |
| sensor_update       | Policy   | &check;      |

#### ManagedApps
| **Name**            | **Type**               | **Nullable** |
| ------------------- | ---------------------- | ------------ |
| airlock             | ManagedApps.ManagedApp | &check;      |
| automox             | ManagedApps.ManagedApp | &check;      |
| identity_protection | ManagedApps.ManagedApp | &check;      |
| jumpcloud           | ManagedApps.ManagedApp | &check;      |
| netskope            | ManagedApps.ManagedApp | &check;      |

#### ManagedApps.ManagedApp
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| version  | String   | &check;      |

#### Meta
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| version        | String   | &check;      |
| version_string | String   | &check;      |

#### Policy
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| applied       | Boolean  | &check;      |
| applied_date  | String   | &check;      |
| assigned_date | String   | &check;      |
| policy_id     | String   | &check;      |
| policy_type   | String   | &check;      |
| rule_groups   | JSON     | &check;      |
| settings_hash | String   | &check;      |
