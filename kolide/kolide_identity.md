---
description: Kolide Identity
---
kolide_identity
---------------

| **Name**                      | **Type** | **Nullable** |
| ----------------------------- | -------- | ------------ |
| archived                      | Boolean  | &check;      |
| email                         | String   | &check;      |
| external_id                   | String   | &check;      |
| id                            | Int      | &cross;      |
| imported_at                   | String   | &check;      |
| mfa_enabled                   | Boolean  | &check;      |
| missing                       | Boolean  | &check;      |
| onboarding_message_count      | Int      | &check;      |
| onboarding_message_first_sent | String   | &check;      |
| onboarding_message_last_sent  | String   | &check;      |
| person                        | Person   | &check;      |
| source                        | String   | &check;      |
| username                      | String   | &check;      |

#### Person
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| created_at   | String   | &check;      |
| device_count | Int      | &check;      |
| email        | String   | &check;      |
| id           | Int      | &check;      |
| name         | String   | &check;      |
| status       | String   | &check;      |
