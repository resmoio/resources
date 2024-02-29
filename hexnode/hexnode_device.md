---
description: Hexnode Device
---
hexnode_device
--------------

| **Name**                   | **Type**          | **Nullable** |
| -------------------------- | ----------------- | ------------ |
| agent_active               | Boolean           | &check;      |
| applications               | List<Application> | &check;      |
| compliant                  | Boolean           | &check;      |
| device                     | Device            | &check;      |
| device_name                | String            | &check;      |
| disenrolled_time           | String            | &check;      |
| enrolled_time              | String            | &check;      |
| enrollment_status          | String            | &check;      |
| id                         | Int               | &cross;      |
| last_location              | String            | &check;      |
| last_location_time         | String            | &check;      |
| lastnotified               | String            | &check;      |
| lastreported               | String            | &check;      |
| lastscanned                | String            | &check;      |
| latitude                   | String            | &check;      |
| location_tracking_disabled | Boolean           | &check;      |
| location_tracking_interval | Int               | &check;      |
| longitude                  | String            | &check;      |
| lostmode                   | Boolean           | &check;      |
| model_name                 | String            | &check;      |
| os_name                    | String            | &check;      |
| os_version                 | String            | &check;      |
| platform                   | String            | &check;      |
| policies                   | List<Policy>      | &check;      |
| remarks                    | String            | &check;      |
| serial_number              | String            | &check;      |
| udid                       | String            | &check;      |
| user                       | User              | &check;      |

#### Application
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| black_listed | Boolean  | &check;      |
| bundle_size  | Long     | &check;      |
| id           | Int      | &cross;      |
| managed      | Boolean  | &check;      |
| name         | String   | &check;      |
| status       | String   | &check;      |
| version      | String   | &check;      |

#### Device
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| available_device_capacity | Double   | &check;      |
| battery_level             | Double   | &check;      |
| build_version             | String   | &check;      |
| description               | String   | &check;      |
| device_capacity           | Double   | &check;      |
| device_name               | String   | &check;      |
| device_type               | String   | &check;      |
| imei_1                    | String   | &check;      |
| imei_2                    | String   | &check;      |
| is_kiosk                  | Boolean  | &check;      |
| is_supervised             | Boolean  | &check;      |
| manufacture               | String   | &check;      |
| model                     | String   | &check;      |
| model_name                | String   | &check;      |
| modem_firmware_version    | String   | &check;      |
| os_name                   | String   | &check;      |
| os_version                | String   | &check;      |
| phoeno_1                  | String   | &check;      |
| phoeno_2                  | String   | &check;      |
| product_name              | String   | &check;      |
| serial_number             | String   | &check;      |
| used_device_capacity      | Double   | &check;      |

#### Policy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &cross;      |
| name     | String   | &check;      |
| version  | Int      | &check;      |

#### User
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| alternate_email | String   | &check;      |
| email           | String   | &check;      |
| id              | String   | &cross;      |
| name            | String   | &check;      |
| phoneno         | String   | &check;      |
