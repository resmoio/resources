---
description: Google Cloud Platform VPC Firewall
---
gcp_vpc_firewall
----------------

| **Name**              | **Type**          | **Nullable** |
| --------------------- | ----------------- | ------------ |
| allowed               | List<Allowed>     | &check;      |
| creationTimestamp     | String            | &check;      |
| denied                | List<Denied>      | &check;      |
| description           | String            | &check;      |
| destinationRanges     | List<String>      | &check;      |
| direction             | String            | &check;      |
| disabled              | Boolean           | &check;      |
| id                    | String            | &cross;      |
| kind                  | String            | &check;      |
| logConfig             | FirewallLogConfig | &check;      |
| name                  | String            | &check;      |
| network               | String            | &check;      |
| priority              | String            | &check;      |
| project               | String            | &cross;      |
| sourceRanges          | List<String>      | &check;      |
| sourceServiceAccounts | List<String>      | &check;      |
| sourceTags            | List<String>      | &check;      |
| targetServiceAccounts | List<String>      | &check;      |
| targetTags            | List<String>      | &check;      |

#### Allowed
| **Name**   | **Type**     | **Nullable** |
| ---------- | ------------ | ------------ |
| IPProtocol | String       | &check;      |
| ports      | List<String> | &check;      |

#### Denied
| **Name**   | **Type**     | **Nullable** |
| ---------- | ------------ | ------------ |
| IPProtocol | String       | &check;      |
| ports      | List<String> | &check;      |

#### FirewallLogConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enable   | Boolean  | &check;      |
| metadata | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
