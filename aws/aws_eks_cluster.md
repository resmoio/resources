---
description: Amazon Web Services EKS Cluster
---
aws_eks_cluster
---------------

| **Name**                | **Type**                        | **Nullable** |
| ----------------------- | ------------------------------- | ------------ |
| accountId               | String                          | &cross;      |
| arn                     | String                          | &cross;      |
| certificateAuthority    | Certificate                     | &check;      |
| clientRequestToken      | String                          | &check;      |
| connectorConfig         | ConnectorConfigResponse         | &check;      |
| createdAt               | String                          | &check;      |
| encryptionConfig        | List<EncryptionConfig>          | &check;      |
| endpoint                | String                          | &check;      |
| identity                | Identity                        | &check;      |
| kubernetesNetworkConfig | KubernetesNetworkConfigResponse | &check;      |
| logging                 | Logging                         | &check;      |
| name                    | String                          | &check;      |
| platformVersion         | String                          | &check;      |
| region                  | String                          | &cross;      |
| resourcesVpcConfig      | VpcConfigResponse               | &check;      |
| roleArn                 | String                          | &check;      |
| status                  | String                          | &check;      |
| tags                    | Map<String,String>              | &check;      |
| version                 | String                          | &check;      |

#### Certificate
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| data     | String   | &check;      |

#### ConnectorConfigResponse
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| activationCode   | String   | &check;      |
| activationExpiry | String   | &check;      |
| activationId     | String   | &check;      |
| provider         | String   | &check;      |
| roleArn          | String   | &check;      |

#### EncryptionConfig
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| provider  | Provider     | &check;      |
| resources | List<String> | &check;      |

#### Identity
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| oidc     | OIDC     | &check;      |

#### KubernetesNetworkConfigResponse
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| ipFamily        | String   | &check;      |
| serviceIpv4Cidr | String   | &check;      |
| serviceIpv6Cidr | String   | &check;      |

#### LogSetup
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| enabled  | Boolean      | &check;      |
| types    | List<String> | &check;      |

#### Logging
| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| clusterLogging | List<LogSetup> | &check;      |

#### OIDC
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| issuer   | String   | &check;      |

#### Provider
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| keyArn   | String   | &check;      |

#### VpcConfigResponse
| **Name**               | **Type**     | **Nullable** |
| ---------------------- | ------------ | ------------ |
| clusterSecurityGroupId | String       | &check;      |
| endpointPrivateAccess  | Boolean      | &check;      |
| endpointPublicAccess   | Boolean      | &check;      |
| publicAccessCidrs      | List<String> | &check;      |
| securityGroupIds       | List<String> | &check;      |
| subnetIds              | List<String> | &check;      |
| vpcId                  | String       | &check;      |
