---
description: Tenable.io Image Report
---
tenable_image_report
--------------------

| **Name**                      | **Type**          | **Nullable** |
| ----------------------------- | ----------------- | ------------ |
| created_at                    | String            | &check;      |
| digest                        | String            | &check;      |
| docker_image_id               | String            | &check;      |
| findings                      | List<Finding>     | &check;      |
| image_name                    | String            | &cross;      |
| installed_packages            | List<PackageInfo> | &check;      |
| malware                       | List<Malware>     | &check;      |
| os                            | String            | &check;      |
| os_architecture               | String            | &check;      |
| os_release_name               | String            | &check;      |
| os_version                    | String            | &check;      |
| platform                      | String            | &check;      |
| potentially_unwanted_programs | List<Program>     | &cross;      |
| repository                    | String            | &cross;      |
| risk_score                    | Int               | &check;      |
| sha256                        | String            | &check;      |
| tag                           | String            | &check;      |
| updated_at                    | String            | &check;      |

#### Finding
| **Name**   | **Type**           | **Nullable** |
| ---------- | ------------------ | ------------ |
| nvdFinding | Finding.NvdFinding | &check;      |
| packages   | List<String>       | &check;      |

#### Finding.NvdFinding
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| access_complexity      | String   | &check;      |
| access_vector          | String   | &check;      |
| auth                   | String   | &check;      |
| availability_impact    | String   | &check;      |
| confidentiality_impact | String   | &check;      |
| cpe                    | String   | &check;      |
| cve                    | String   | &check;      |
| cvss_score             | String   | &check;      |
| cwe                    | String   | &check;      |
| description            | String   | &check;      |
| integrity_impact       | String   | &check;      |
| modified_date          | String   | &check;      |
| published_date         | String   | &check;      |
| references             | String   | &check;      |
| remediation            | String   | &check;      |

#### Malware
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| fileTypeDescriptor | String   | &check;      |
| infectedFile       | String   | &check;      |
| md5                | String   | &check;      |
| sha256             | String   | &check;      |

#### PackageInfo
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |
| version  | String   | &check;      |

#### Program
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| fileTypeDescriptor | String   | &check;      |
| infectedFile       | String   | &check;      |
| md5                | String   | &check;      |
| sha256             | String   | &check;      |
