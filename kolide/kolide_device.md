---
description: Kolide Device
---
kolide_device
-------------

| **Name**                 | **Type**               | **Nullable** |
| ------------------------ | ---------------------- | ------------ |
| assigned_owner           | AssignedOwner          | &check;      |
| enrolled_at              | String                 | &check;      |
| failure_count            | Int                    | &check;      |
| hardware_model           | String                 | &check;      |
| hardware_vendor          | String                 | &check;      |
| id                       | Int                    | &cross;      |
| issue_count              | Int                    | &check;      |
| issues                   | List<Issue>            | &cross;      |
| last_seen_at             | String                 | &check;      |
| launcher_version         | String                 | &check;      |
| name                     | String                 | &check;      |
| note                     | String                 | &check;      |
| operating_system         | String                 | &check;      |
| operating_system_details | OperatingSystemDetails | &check;      |
| osquery_version          | String                 | &check;      |
| owned_by                 | String                 | &check;      |
| platform                 | String                 | &check;      |
| privacy                  | String                 | &check;      |
| remote_ip                | String                 | &check;      |
| resolved_failure_count   | Int                    | &check;      |
| resolved_issue_count     | Int                    | &check;      |
| serial                   | String                 | &check;      |

#### AssignedOwner
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| email      | String   | &check;      |
| id         | Int      | &cross;      |
| name       | String   | &check;      |
| owner_type | String   | &check;      |

#### Check
| **Name**                  | **Type**     | **Nullable** |
| ------------------------- | ------------ | ------------ |
| check_tags                | List<String> | &check;      |
| compatibility             | List<String> | &check;      |
| description               | String       | &check;      |
| display_name              | String       | &cross;      |
| failing_device_count      | Int          | &check;      |
| id                        | Int          | &cross;      |
| name                      | String       | &cross;      |
| notification_grace_period | Int          | &check;      |
| notification_strategy     | String       | &check;      |
| tags                      | List<String> | &check;      |
| topics                    | List<String> | &check;      |

#### Issue
| **Name**                | **Type**           | **Nullable** |
| ----------------------- | ------------------ | ------------ |
| check                   | Check              | &cross;      |
| check_id                | Int                | &cross;      |
| escalation_status       | String             | &check;      |
| first_notified_owner_at | String             | &check;      |
| grace_period_expiration | String             | &check;      |
| id                      | Int                | &check;      |
| ignored                 | Boolean            | &check;      |
| issue_key               | String             | &check;      |
| issue_value             | String             | &check;      |
| resolved_at             | String             | &check;      |
| timestamp               | String             | &check;      |
| title                   | String             | &check;      |
| value                   | Map<String,String> | &check;      |

#### OperatingSystemDetails
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| build         | String   | &check;      |
| codename      | String   | &check;      |
| device_id     | Int      | &check;      |
| major_version | Int      | &check;      |
| minor_version | Int      | &check;      |
| name          | String   | &check;      |
| patch_version | Int      | &check;      |
| platform      | String   | &check;      |
| version       | String   | &check;      |
