---
description: MongoDB Atlas Alert Configuration
---
mongodb_alert_configuration
---------------------------

| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| created         | String             | &check;      |
| enabled         | Boolean            | &check;      |
| eventTypeName   | String             | &check;      |
| groupId         | String             | &check;      |
| id              | String             | &cross;      |
| links           | List<Link>         | &cross;      |
| matchers        | List<Matcher>      | &cross;      |
| metricThreshold | MetricThreshold    | &check;      |
| notifications   | List<Notification> | &cross;      |
| project         | Project            | &cross;      |
| threshold       | MetricThreshold    | &check;      |
| typeName        | String             | &check;      |
| updated         | String             | &check;      |

#### Link
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| rel      | String   | &check;      |

#### Matcher
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| fieldName | String   | &check;      |
| operator  | String   | &check;      |
| value     | String   | &check;      |

#### MetricThreshold
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| metricName | String   | &check;      |
| mode       | String   | &check;      |
| operator   | String   | &check;      |
| threshold  | Int      | &check;      |
| units      | String   | &check;      |

#### Notification
| **Name**                 | **Type**     | **Nullable** |
| ------------------------ | ------------ | ------------ |
| apiToken                 | String       | &check;      |
| channelName              | String       | &check;      |
| datadogApiKey            | String       | &check;      |
| datadogRegion            | String       | &check;      |
| delayMin                 | Int          | &check;      |
| emailAddress             | String       | &check;      |
| emailEnabled             | Boolean      | &check;      |
| flowName                 | String       | &check;      |
| flowdockApiToken         | String       | &check;      |
| intervalMin              | Int          | &check;      |
| microsoftTeamsWebhookUrl | String       | &check;      |
| mobileNumber             | String       | &check;      |
| opsGenieApiKey           | String       | &check;      |
| opsGenieRegion           | String       | &check;      |
| orgName                  | String       | &check;      |
| roles                    | List<String> | &check;      |
| serviceKey               | String       | &check;      |
| smsEnabled               | Boolean      | &check;      |
| teamId                   | String       | &check;      |
| typeName                 | String       | &check;      |
| username                 | String       | &check;      |
| victorOpsApiKey          | String       | &check;      |
| victorOpsRoutingKey      | String       | &check;      |

#### Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
