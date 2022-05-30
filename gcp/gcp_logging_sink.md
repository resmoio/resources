---
description: Google Cloud Platform Logging Sink
---
gcp_logging_sink
----------------

| **Name**            | **Type**           | **Nullable** |
| ------------------- | ------------------ | ------------ |
| bigqueryOptions     | BigQueryOptions    | &check;      |
| createTime          | String             | &check;      |
| description         | String             | &check;      |
| destination         | String             | &check;      |
| disabled            | Boolean            | &check;      |
| exclusions          | List<LogExclusion> | &check;      |
| filter              | String             | &check;      |
| includeChildren     | Boolean            | &check;      |
| name                | String             | &cross;      |
| outputVersionFormat | Int                | &check;      |
| project             | String             | &cross;      |
| updateTime          | String             | &check;      |
| writerIdentity      | String             | &check;      |

#### BigQueryOptions
| **Name**                        | **Type** | **Nullable** |
| ------------------------------- | -------- | ------------ |
| usePartitionedTables            | Boolean  | &check;      |
| usesTimestampColumnPartitioning | Boolean  | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### LogExclusion
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| createTime  | String   | &check;      |
| description | String   | &check;      |
| disabled    | Boolean  | &check;      |
| filter      | String   | &check;      |
| name        | String   | &check;      |
| updateTime  | String   | &check;      |
