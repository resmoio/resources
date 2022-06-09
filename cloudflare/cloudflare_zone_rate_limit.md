---
description: Cloudflare Zone Rate Limit
---
cloudflare_zone_rate_limit
--------------------------

| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| action      | Action       | &check;      |
| bypass      | List<Bypass> | &check;      |
| description | String       | &check;      |
| disabled    | Boolean      | &check;      |
| id          | String       | &cross;      |
| match       | Match        | &check;      |
| period      | Int          | &check;      |
| threshold   | Int          | &check;      |
| zone_id     | String       | &cross;      |

#### Action
| **Name** | **Type**        | **Nullable** |
| -------- | --------------- | ------------ |
| mode     | String          | &check;      |
| response | Action.Response | &check;      |
| timeout  | Int             | &check;      |

#### Action.Response
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| body         | String   | &check;      |
| content_type | String   | &check;      |

#### Bypass
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| value    | String   | &check;      |

#### Match
| **Name** | **Type**           | **Nullable** |
| -------- | ------------------ | ------------ |
| headers  | List<Match.Header> | &check;      |
| request  | Match.Request      | &check;      |
| response | Match.Response     | &check;      |

#### Match.Header
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| op       | String   | &check;      |
| value    | String   | &check;      |

#### Match.Request
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| methods  | List<String> | &check;      |
| schemes  | List<String> | &check;      |
| url      | String       | &check;      |

#### Match.Response
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| origin_traffic | Boolean  | &check;      |
