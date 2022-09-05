---
description: Fastly Service Backend
---
fastly_service_backend
----------------------

| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| address               | String   | &check;      |
| auto_loadbalance      | Boolean  | &check;      |
| between_bytes_timeout | Int      | &check;      |
| client_cert           | String   | &check;      |
| comment               | String   | &check;      |
| connect_timeout       | Int      | &check;      |
| created_at            | String   | &check;      |
| deleted_at            | String   | &check;      |
| first_byte_timeout    | Int      | &check;      |
| healthcheck           | String   | &check;      |
| hostname              | String   | &check;      |
| ipv4                  | String   | &check;      |
| ipv6                  | String   | &check;      |
| locked                | Boolean  | &check;      |
| max_conn              | Int      | &check;      |
| max_tls_version       | String   | &check;      |
| min_tls_version       | String   | &check;      |
| name                  | String   | &cross;      |
| override_host         | String   | &check;      |
| port                  | Int      | &check;      |
| request_condition     | String   | &check;      |
| service_id            | String   | &cross;      |
| shield                | String   | &check;      |
| ssl_ca_cert           | String   | &check;      |
| ssl_cert_hostname     | String   | &check;      |
| ssl_check_cert        | Boolean  | &check;      |
| ssl_ciphers           | String   | &check;      |
| ssl_client_cert       | String   | &check;      |
| ssl_client_key        | String   | &check;      |
| ssl_sni_hostname      | String   | &check;      |
| updated_at            | String   | &check;      |
| use_ssl               | Boolean  | &check;      |
| version               | Int      | &cross;      |
| weight                | Int      | &check;      |
