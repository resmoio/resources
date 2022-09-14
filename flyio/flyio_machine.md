---
description: Flyio Machine
---
flyio_machine
-------------

| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| appId      | String   | &cross;      |
| appName    | String   | &cross;      |
| config     | Config   | &cross;      |
| hostId     | String   | &cross;      |
| id         | String   | &cross;      |
| instanceId | String   | &cross;      |
| ips        | List<IP> | &cross;      |
| name       | String   | &cross;      |
| region     | String   | &cross;      |
| state      | String   | &cross;      |
| updatedAt  | String   | &check;      |

#### Config
| **Name**  | **Type**           | **Nullable** |
| --------- | ------------------ | ------------ |
| env       | Map<String,String> | &check;      |
| image     | String             | &check;      |
| image_ref | Config.ImageRef    | &check;      |
| init      | Config.Init        | &check;      |
| mounts    | List<Config.Mount> | &cross;      |
| restart   | Config.Restart     | &cross;      |
| size      | String             | &check;      |

#### Config.ImageRef
| **Name**   | **Type**           | **Nullable** |
| ---------- | ------------------ | ------------ |
| digest     | String             | &check;      |
| labels     | Map<String,String> | &check;      |
| registry   | String             | &check;      |
| repository | String             | &check;      |
| tag        | String             | &check;      |

#### Config.Init
| **Name**   | **Type**     | **Nullable** |
| ---------- | ------------ | ------------ |
| cmd        | List<String> | &check;      |
| entrypoint | List<String> | &check;      |
| exec       | List<String> | &check;      |
| tty        | Boolean      | &check;      |

#### Config.Mount
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| encrypted | Boolean  | &check;      |
| path      | String   | &check;      |
| size_gb   | Int      | &check;      |
| volume    | String   | &check;      |

#### Config.Restart
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| max_retries | Int      | &check;      |
| policy      | String   | &check;      |

#### IP
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| family   | String   | &check;      |
| id       | String   | &check;      |
| ip       | String   | &check;      |
| kind     | String   | &check;      |
| maskSize | Int      | &check;      |
