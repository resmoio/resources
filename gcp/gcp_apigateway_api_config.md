---
description: Google Cloud Platform API Gateway API Config
---
gcp_apigateway_api_config
-------------------------

| **Name**              | **Type**                    | **Nullable** |
| --------------------- | --------------------------- | ------------ |
| createTime            | String                      | &check;      |
| displayName           | String                      | &check;      |
| gatewayServiceAccount | String                      | &check;      |
| grpcServices          | List<GrpcServiceDefinition> | &check;      |
| labels                | Map<String,String>          | &check;      |
| managedServiceConfigs | List<File>                  | &check;      |
| name                  | String                      | &cross;      |
| openapiDocuments      | List<OpenApiDocument>       | &check;      |
| project               | String                      | &cross;      |
| serviceConfigId       | String                      | &check;      |
| state                 | String                      | &check;      |
| updateTime            | String                      | &check;      |

#### File
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| path     | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### GrpcServiceDefinition
| **Name**          | **Type**   | **Nullable** |
| ----------------- | ---------- | ------------ |
| fileDescriptorSet | File       | &check;      |
| source            | List<File> | &check;      |

#### OpenApiDocument
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| document | File     | &check;      |
