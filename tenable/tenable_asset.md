---
description: Tenable.io Asset
---
tenable_asset
-------------

| **Name**                     | **Type**        | **Nullable** |
| ---------------------------- | --------------- | ------------ |
| agent_names                  | List<String>    | &check;      |
| agent_uuid                   | String          | &check;      |
| aws_availability_zone        | String          | &check;      |
| aws_ec2_instance_ami_id      | String          | &check;      |
| aws_ec2_instance_group_name  | String          | &check;      |
| aws_ec2_instance_id          | String          | &check;      |
| aws_ec2_instance_state_name  | String          | &check;      |
| aws_ec2_instance_type        | String          | &check;      |
| aws_ec2_name                 | String          | &check;      |
| aws_ec2_product_code         | String          | &check;      |
| aws_owner_id                 | String          | &check;      |
| aws_region                   | String          | &check;      |
| aws_subnet_id                | String          | &check;      |
| aws_vpc_id                   | String          | &check;      |
| azure_resource_id            | String          | &check;      |
| azure_vm_id                  | String          | &check;      |
| bigfix_asset_id              | String          | &check;      |
| bios_uuid                    | String          | &check;      |
| created_at                   | String          | &check;      |
| deleted_at                   | String          | &check;      |
| deleted_by                   | String          | &check;      |
| first_scan_time              | String          | &check;      |
| first_seen                   | String          | &check;      |
| fqdns                        | List<String>    | &check;      |
| gcp_instance_id              | String          | &check;      |
| gcp_project_id               | String          | &check;      |
| gcp_zone                     | String          | &check;      |
| has_agent                    | Boolean         | &check;      |
| has_plugin_results           | Boolean         | &check;      |
| hostnames                    | List<String>    | &check;      |
| id                           | String          | &cross;      |
| installed_software           | List<String>    | &check;      |
| ipv4s                        | List<String>    | &check;      |
| ipv6s                        | List<String>    | &check;      |
| last_authenticated_scan_date | String          | &check;      |
| last_licensed_scan_date      | String          | &check;      |
| last_scan_id                 | String          | &check;      |
| last_scan_time               | String          | &check;      |
| last_schedule_id             | String          | &check;      |
| last_seen                    | String          | &check;      |
| mac_addresses                | List<String>    | &check;      |
| manufacturer_tpm_ids         | List<String>    | &check;      |
| mcafee_epo_agent_guid        | String          | &check;      |
| mcafee_epo_guid              | String          | &check;      |
| netbios_names                | List<String>    | &check;      |
| network_id                   | String          | &check;      |
| network_interfaces           | List<Interface> | &check;      |
| network_name                 | String          | &check;      |
| operating_systems            | List<String>    | &check;      |
| qualys_asset_ids             | List<String>    | &check;      |
| qualys_host_ids              | List<String>    | &check;      |
| servicenow_sysid             | String          | &check;      |
| sources                      | List<Source>    | &check;      |
| ssh_fingerprints             | List<String>    | &check;      |
| symantec_ep_hardware_keys    | List<String>    | &check;      |
| system_types                 | List<String>    | &check;      |
| tags                         | List<Tag>       | &check;      |
| terminated_at                | String          | &check;      |
| terminated_by                | String          | &check;      |
| updated_at                   | String          | &check;      |

#### Interface
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| aliased       | String       | &check;      |
| fqdns         | List<String> | &check;      |
| ipv4s         | List<String> | &check;      |
| ipv6s         | List<String> | &check;      |
| mac_addresses | List<String> | &check;      |
| name          | String       | &check;      |
| virtual       | String       | &check;      |

#### Source
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| first_seen | Date     | &check;      |
| last_seen  | Date     | &check;      |
| name       | String   | &check;      |

#### Tag
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| added_at | String   | &check;      |
| added_by | String   | &check;      |
| key      | String   | &check;      |
| uuid     | String   | &check;      |
| value    | String   | &check;      |
