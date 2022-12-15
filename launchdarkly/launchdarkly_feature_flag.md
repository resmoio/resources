---
description: LaunchDarkly Feature Flag
---
launchdarkly_feature_flag
-------------------------

| **Name**               | **Type**                | **Nullable** |
| ---------------------- | ----------------------- | ------------ |
| _maintainer            | Maintainer              | &check;      |
| _maintainerTeam        | MaintainerTeam          | &check;      |
| _version               | Long                    | &check;      |
| archived               | Boolean                 | &check;      |
| archivedDate           | Long                    | &check;      |
| clientSideAvailability | ClientSideAvailability  | &check;      |
| creationDate           | Long                    | &check;      |
| customProperties       | CustomProperties        | &check;      |
| defaults               | Defaults                | &check;      |
| description            | String                  | &check;      |
| environments           | Map<String,Environment> | &check;      |
| experiments            | Experiments             | &check;      |
| goalIds                | List<String>            | &check;      |
| includeInSnippet       | Boolean                 | &check;      |
| key                    | String                  | &cross;      |
| kind                   | String                  | &check;      |
| maintainerId           | String                  | &check;      |
| maintainerTeamKey      | String                  | &check;      |
| name                   | String                  | &check;      |
| projectKey             | String                  | &check;      |
| tags                   | List<String>            | &check;      |
| temporary              | Boolean                 | &check;      |
| variations             | List<Variation>         | &check;      |

#### ClientSideAvailability
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| usingEnvironmentId | Boolean  | &check;      |
| usingMobileKey     | Boolean  | &check;      |

#### CustomProperties
| **Name**  | **Type**                   | **Nullable** |
| --------- | -------------------------- | ------------ |
| property1 | CustomProperties.Property1 | &check;      |
| property2 | CustomProperties.Property2 | &check;      |

#### CustomProperties.Property1
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| name     | String       | &check;      |
| value    | List<String> | &check;      |

#### CustomProperties.Property2
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| name     | String       | &check;      |
| value    | List<String> | &check;      |

#### Defaults
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| offVariation | Long     | &check;      |
| onVariation  | Long     | &check;      |

#### Environment
| **Name**               | **Type**                       | **Nullable** |
| ---------------------- | ------------------------------ | ------------ |
| _environmentName       | String                         | &check;      |
| archived               | Boolean                        | &check;      |
| fallthrough            | Environment.Fallthrough        | &check;      |
| lastModified           | Long                           | &check;      |
| offVariation           | Long                           | &check;      |
| on                     | Boolean                        | &check;      |
| prerequisites          | List<Environment.Prerequisite> | &check;      |
| rules                  | List<Environment.Rule>         | &check;      |
| salt                   | String                         | &check;      |
| sel                    | String                         | &check;      |
| targets                | List<Environment.Target>       | &check;      |
| trackEvents            | Boolean                        | &check;      |
| trackEventsFallthrough | Boolean                        | &check;      |
| version                | Long                           | &check;      |

#### Environment.Fallthrough
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| variation | Long     | &check;      |

#### Environment.Prerequisite
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| key       | String   | &check;      |
| variation | Long     | &check;      |

#### Environment.Rule
| **Name**    | **Type**                      | **Nullable** |
| ----------- | ----------------------------- | ------------ |
| _id         | String                        | &check;      |
| clauses     | List<Environment.Rule.Clause> | &check;      |
| description | String                        | &check;      |
| ref         | String                        | &check;      |
| rollout     | Environment.Rule.Rollout      | &check;      |
| trackEvents | Boolean                       | &check;      |
| variation   | Long                          | &check;      |

#### Environment.Rule.Clause
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| _id       | String   | &check;      |
| attribute | String   | &check;      |
| negate    | Boolean  | &check;      |
| op        | String   | &check;      |

#### Environment.Rule.Rollout
| **Name**             | **Type**                                      | **Nullable** |
| -------------------- | --------------------------------------------- | ------------ |
| bucketBy             | String                                        | &check;      |
| experimentAllocation | Environment.Rule.Rollout.ExperimentAllocation | &check;      |
| seed                 | Long                                          | &check;      |
| variations           | List<Variation>                               | &check;      |

#### Environment.Rule.Rollout.ExperimentAllocation
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| canReshuffle     | Boolean  | &check;      |
| defaultVariation | Long     | &check;      |

#### Environment.Target
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| values    | List<String> | &check;      |
| variation | Long         | &check;      |

#### Experiments
| **Name**    | **Type**               | **Nullable** |
| ----------- | ---------------------- | ------------ |
| baselineIdx | Long                   | &check;      |
| items       | List<Experiments.Item> | &check;      |

#### Experiments.Item
| **Name**             | **Type**                                         | **Nullable** |
| -------------------- | ------------------------------------------------ | ------------ |
| _environmentSettings | Map<String,Experiments.Item.EnvironmentSettings> | &check;      |
| _metric              | Experiments.Metric                               | &check;      |
| environments         | List<String>                                     | &check;      |
| metricKey            | String                                           | &check;      |

#### Experiments.Item.EnvironmentSettings
| **Name**       | **Type**  | **Nullable** |
| -------------- | --------- | ------------ |
| enabledPeriods | List<Map> | &check;      |
| startDate      | Long      | &check;      |
| stopDate       | Long      | &check;      |

#### Experiments.Metric
| **Name**           | **Type**                        | **Nullable** |
| ------------------ | ------------------------------- | ------------ |
| _attachedFlagCount | Long                            | &check;      |
| _creationDate      | Long                            | &check;      |
| _id                | String                          | &check;      |
| _maintainer        | Experiments.Metric.Maintainer   | &check;      |
| description        | String                          | &check;      |
| eventKey           | String                          | &check;      |
| experimentCount    | Long                            | &check;      |
| isNumeric          | Boolean                         | &check;      |
| key                | String                          | &check;      |
| kind               | String                          | &check;      |
| lastModified       | Experiments.Metric.LastModified | &check;      |
| maintainerId       | String                          | &check;      |
| name               | String                          | &check;      |
| successCriteria    | String                          | &check;      |
| tags               | List<String>                    | &check;      |
| unit               | String                          | &check;      |

#### Experiments.Metric.LastModified
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| date     | String   | &check;      |

#### Experiments.Metric.Maintainer
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| _id       | String   | &check;      |
| email     | String   | &check;      |
| firstName | String   | &check;      |
| lastName  | String   | &check;      |
| role      | String   | &check;      |

#### Maintainer
| **Name**  | **Type**         | **Nullable** |
| --------- | ---------------- | ------------ |
| _id       | String           | &check;      |
| _links    | Maintainer.Links | &check;      |
| email     | String           | &check;      |
| firstName | String           | &check;      |
| lastName  | String           | &check;      |
| role      | String           | &check;      |

#### Maintainer.Links
| **Name** | **Type**              | **Nullable** |
| -------- | --------------------- | ------------ |
| self     | Maintainer.Links.Self | &check;      |

#### Maintainer.Links.Self
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| type     | String   | &check;      |

#### MaintainerTeam
| **Name** | **Type**             | **Nullable** |
| -------- | -------------------- | ------------ |
| _links   | MaintainerTeam.Links | &check;      |
| key      | String               | &check;      |
| name     | String               | &check;      |

#### MaintainerTeam.Links
| **Name** | **Type**                    | **Nullable** |
| -------- | --------------------------- | ------------ |
| parent   | MaintainerTeam.Links.Parent | &check;      |
| roles    | MaintainerTeam.Links.Roles  | &check;      |
| self     | MaintainerTeam.Links.Self   | &check;      |

#### MaintainerTeam.Links.Parent
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| type     | String   | &check;      |

#### MaintainerTeam.Links.Roles
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| type     | String   | &check;      |

#### MaintainerTeam.Links.Self
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| type     | String   | &check;      |

#### Variation
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| _id      | String   | &check;      |
| value    | Boolean  | &check;      |
