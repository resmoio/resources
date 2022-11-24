---
description: Tailscale DNS
---
tailscale_dns
-------------

| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| dnsPreferences | DNSPreferences | &check;      |
| nameservers    | List<String>   | &check;      |
| searchpaths    | List<String>   | &check;      |

#### DNSPreferences
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| magicDNS | Boolean  | &check;      |
