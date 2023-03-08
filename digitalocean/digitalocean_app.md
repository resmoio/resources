---
description: DigitalOcean App
---
digitalocean_app
----------------

| **Name**                   | **Type**     | **Nullable** |
| -------------------------- | ------------ | ------------ |
| active_deployment          | Deployment   | &check;      |
| created_at                 | String       | &check;      |
| default_ingress            | String       | &check;      |
| domains                    | List<Domain> | &check;      |
| id                         | String       | &cross;      |
| in_progress_deployment     | Deployment   | &check;      |
| last_deployment_created_at | String       | &check;      |
| live_domain                | String       | &check;      |
| live_url                   | String       | &check;      |
| live_url_base              | String       | &check;      |
| owner_uuid                 | String       | &check;      |
| pending_deployment         | Deployment   | &check;      |
| pinned_deployment          | Deployment   | &check;      |
| project_id                 | String       | &check;      |
| region                     | Region       | &check;      |
| spec                       | Spec         | &check;      |
| tier_slug                  | String       | &check;      |
| updated_at                 | String       | &check;      |

#### Deployment
| **Name**              | **Type**                     | **Nullable** |
| --------------------- | ---------------------------- | ------------ |
| cause                 | String                       | &check;      |
| cloned_from           | String                       | &check;      |
| created_at            | String                       | &check;      |
| functions             | List<Deployment.Function>    | &check;      |
| id                    | String                       | &check;      |
| jobs                  | List<Deployment.Job>         | &check;      |
| phase                 | String                       | &check;      |
| phase_last_updated_at | String                       | &check;      |
| progress              | Deployment.Progress          | &check;      |
| services              | List<Deployment.Service>     | &check;      |
| spec                  | Spec                         | &check;      |
| static_sites          | List<Deployment.StaticSites> | &check;      |
| tier_slug             | String                       | &check;      |
| updated_at            | String                       | &check;      |
| workers               | List<Deployment.Worker>      | &check;      |

#### Deployment.Function
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| name               | String   | &check;      |
| namespace          | String   | &check;      |
| source_commit_hash | String   | &check;      |

#### Deployment.Job
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| name               | String   | &check;      |
| source_commit_hash | String   | &check;      |

#### Deployment.Progress
| **Name**      | **Type**                       | **Nullable** |
| ------------- | ------------------------------ | ------------ |
| error_steps   | Long                           | &check;      |
| pending_steps | Long                           | &check;      |
| running_steps | Long                           | &check;      |
| steps         | List<Deployment.Progress.Step> | &check;      |
| success_steps | Long                           | &check;      |
| summary_steps | List<Deployment.Progress.Step> | &check;      |
| total_steps   | Long                           | &check;      |

#### Deployment.Progress.Step
| **Name**       | **Type**                        | **Nullable** |
| -------------- | ------------------------------- | ------------ |
| component_name | String                          | &check;      |
| ended_at       | String                          | &check;      |
| message_base   | String                          | &check;      |
| name           | String                          | &check;      |
| reason         | Deployment.Progress.Step.Reason | &check;      |
| started_at     | String                          | &check;      |
| status         | String                          | &check;      |
| steps          | JSON                            | &check;      |

#### Deployment.Progress.Step.Reason
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | String   | &check;      |
| message  | String   | &check;      |

#### Deployment.Service
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| name               | String   | &check;      |
| source_commit_hash | String   | &check;      |

#### Deployment.StaticSites
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| name               | String   | &check;      |
| source_commit_hash | String   | &check;      |

#### Deployment.Worker
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| name               | String   | &check;      |
| source_commit_hash | String   | &check;      |

#### Domain
| **Name**                  | **Type**                | **Nullable** |
| ------------------------- | ----------------------- | ------------ |
| certificate_expires_at    | String                  | &check;      |
| id                        | String                  | &check;      |
| phase                     | String                  | &check;      |
| progress                  | JSON                    | &check;      |
| rotate_validation_records | Boolean                 | &check;      |
| spec                      | Domain.Spec             | &check;      |
| validations               | List<Domain.Validation> | &check;      |

#### Domain.Spec
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| domain              | String   | &check;      |
| minimum_tls_version | String   | &check;      |
| type                | String   | &check;      |
| wildcard            | Boolean  | &check;      |
| zone                | String   | &check;      |

#### Domain.Validation
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| txt_name  | String   | &check;      |
| txt_value | String   | &check;      |

#### Region
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| continent    | String       | &check;      |
| data_centers | List<String> | &check;      |
| default      | Boolean      | &check;      |
| disabled     | Boolean      | &check;      |
| flag         | String       | &check;      |
| label        | String       | &check;      |
| reason       | String       | &check;      |
| slug         | String       | &check;      |

#### Spec
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| region   | String   | &check;      |
