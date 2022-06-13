---
description: Gandi Domain
---
gandi_domain
------------

| **Name**               | **Type**     | **Nullable** |
| ---------------------- | ------------ | ------------ |
| autorenew              | Boolean      | &check;      |
| dates                  | Dates        | &check;      |
| domain_owner           | String       | &check;      |
| fqdn                   | String       | &cross;      |
| fqdn_unicode           | String       | &cross;      |
| href                   | String       | &check;      |
| id                     | String       | &cross;      |
| nameserver             | Nameserver   | &cross;      |
| nameserver_information | List<String> | &check;      |
| orga_owner             | String       | &check;      |
| owner                  | String       | &check;      |
| restorable             | Restorable   | &check;      |
| sharing_id             | String       | &check;      |
| status                 | List<String> | &check;      |
| tags                   | List<String> | &check;      |
| tld                    | String       | &check;      |
| zone_transfer_slave    | List<String> | &check;      |

#### Dates
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| authinfo_expires_at    | String   | &check;      |
| created_at             | String   | &check;      |
| deletes_at             | String   | &check;      |
| hold_begins_at         | String   | &check;      |
| hold_ends_at           | String   | &check;      |
| pending_delete_ends_at | String   | &check;      |
| registry_created_at    | String   | &check;      |
| registry_ends_at       | String   | &check;      |
| renew_begins_at        | String   | &check;      |
| restore_ends_at        | String   | &check;      |
| updated_at             | String   | &check;      |

#### Nameserver
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| current  | String       | &cross;      |
| hosts    | List<String> | &check;      |

#### Restorable
| **Name**   | **Type**                  | **Nullable** |
| ---------- | ------------------------- | ------------ |
| contracts  | List<Restorable.Contract> | &check;      |
| restorable | Boolean                   | &check;      |

#### Restorable.Contract
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
