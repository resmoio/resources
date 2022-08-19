---
description: Amazon Web Services ELB Load Balancer
---
aws_elb_load_balancer
---------------------

| **Name**              | **Type**               | **Nullable** |
| --------------------- | ---------------------- | ------------ |
| accountId             | String                 | &cross;      |
| accountName           | String                 | &check;      |
| attributes            | Map<String,String>     | &check;      |
| availabilityZones     | List<AvailabilityZone> | &cross;      |
| canonicalHostedZoneId | String                 | &check;      |
| createdTime           | String                 | &check;      |
| customerOwnedIpv4Pool | String                 | &check;      |
| dnsName               | String                 | &check;      |
| ipAddressType         | String                 | &check;      |
| listeners             | List<Listener>         | &check;      |
| loadBalancerArn       | String                 | &cross;      |
| loadBalancerName      | String                 | &cross;      |
| region                | String                 | &cross;      |
| scheme                | String                 | &check;      |
| securityGroups        | List<String>           | &cross;      |
| type                  | String                 | &check;      |
| vpcId                 | String                 | &cross;      |

#### AvailabilityZone
| **Name**              | **Type**                  | **Nullable** |
| --------------------- | ------------------------- | ------------ |
| loadBalancerAddresses | List<LoadBalancerAddress> | &check;      |
| outpostId             | String                    | &check;      |
| subnetId              | String                    | &check;      |
| zoneName              | String                    | &check;      |

#### Listener
| **Name**       | **Type**                   | **Nullable** |
| -------------- | -------------------------- | ------------ |
| alpnPolicy     | List<String>               | &check;      |
| certificates   | List<Listener.Certificate> | &check;      |
| defaultActions | List<Listener.Action>      | &cross;      |
| listenerArn    | String                     | &cross;      |
| port           | Int                        | &check;      |
| protocol       | String                     | &check;      |
| rules          | List<Listener.Rule>        | &check;      |
| sslPolicy      | String                     | &check;      |

#### Listener.Action
| **Name**                  | **Type**                                        | **Nullable** |
| ------------------------- | ----------------------------------------------- | ------------ |
| authenticateCognitoConfig | Listener.Action.AuthenticateCognitoActionConfig | &check;      |
| authenticateOidcConfig    | Listener.Action.AuthenticateOidcActionConfig    | &check;      |
| fixedResponseConfig       | Listener.Action.FixedResponseActionConfig       | &check;      |
| forwardConfig             | Listener.Action.ForwardActionConfig             | &check;      |
| order                     | Int                                             | &check;      |
| redirectConfig            | Listener.Action.RedirectActionConfig            | &check;      |
| targetGroupArn            | String                                          | &check;      |
| type                      | String                                          | &cross;      |

#### Listener.Action.AuthenticateCognitoActionConfig
| **Name**                         | **Type**           | **Nullable** |
| -------------------------------- | ------------------ | ------------ |
| authenticationRequestExtraParams | Map<String,String> | &check;      |
| onUnauthenticatedRequest         | String             | &check;      |
| scope                            | String             | &check;      |
| sessionCookieName                | String             | &check;      |
| sessionTimeout                   | Long               | &check;      |
| userPoolArn                      | String             | &check;      |
| userPoolClientId                 | String             | &check;      |
| userPoolDomain                   | String             | &check;      |

#### Listener.Action.AuthenticateOidcActionConfig
| **Name**                         | **Type**           | **Nullable** |
| -------------------------------- | ------------------ | ------------ |
| authenticationRequestExtraParams | Map<String,String> | &check;      |
| authorizationEndpoint            | String             | &check;      |
| clientId                         | String             | &check;      |
| clientSecret                     | String             | &check;      |
| issuer                           | String             | &check;      |
| onUnauthenticatedRequest         | String             | &check;      |
| scope                            | String             | &check;      |
| sessionCookieName                | String             | &check;      |
| sessionTimeout                   | Long               | &check;      |
| tokenEndpoint                    | String             | &check;      |
| useExistingClientSecret          | Boolean            | &check;      |
| userInfoEndpoint                 | String             | &check;      |

#### Listener.Action.FixedResponseActionConfig
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| contentType | String   | &check;      |
| messageBody | String   | &check;      |
| statusCode  | String   | &check;      |

#### Listener.Action.ForwardActionConfig
| **Name**                    | **Type**                                                        | **Nullable** |
| --------------------------- | --------------------------------------------------------------- | ------------ |
| targetGroupStickinessConfig | Listener.Action.ForwardActionConfig.TargetGroupStickinessConfig | &check;      |
| targetGroups                | List<Listener.Action.ForwardActionConfig.TargetGroupTuple>      | &check;      |

#### Listener.Action.ForwardActionConfig.TargetGroupStickinessConfig
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| durationSeconds | Int      | &check;      |
| enabled         | Boolean  | &check;      |

#### Listener.Action.ForwardActionConfig.TargetGroupTuple
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| targetGroupArn | String   | &check;      |
| weight         | Int      | &check;      |

#### Listener.Action.RedirectActionConfig
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| host       | String   | &check;      |
| path       | String   | &check;      |
| port       | String   | &check;      |
| protocol   | String   | &check;      |
| query      | String   | &check;      |
| statusCode | String   | &check;      |

#### Listener.Certificate
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| certificateArn | String   | &check;      |
| isDefault      | Boolean  | &check;      |

#### Listener.Rule
| **Name**   | **Type**                          | **Nullable** |
| ---------- | --------------------------------- | ------------ |
| actions    | List<Listener.Action>             | &cross;      |
| conditions | List<Listener.Rule.RuleCondition> | &check;      |
| isDefault  | Boolean                           | &check;      |
| priority   | String                            | &check;      |
| ruleArn    | String                            | &cross;      |

#### Listener.Rule.RuleCondition
| **Name**                | **Type**                                              | **Nullable** |
| ----------------------- | ----------------------------------------------------- | ------------ |
| field                   | String                                                | &check;      |
| hostHeaderConfig        | List<String>                                          | &check;      |
| httpHeaderConfig        | Listener.Rule.RuleCondition.HttpHeaderConditionConfig | &check;      |
| httpRequestMethodConfig | List<String>                                          | &check;      |
| pathPatternConfig       | List<String>                                          | &check;      |
| queryStringConfig       | Map<String,String>                                    | &check;      |
| sourceIpConfig          | List<String>                                          | &check;      |
| values                  | List<String>                                          | &check;      |

#### Listener.Rule.RuleCondition.HttpHeaderConditionConfig
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| httpHeaderName | String       | &cross;      |
| values         | List<String> | &cross;      |

#### LoadBalancerAddress
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| allocationId       | String   | &check;      |
| iPv6Address        | String   | &check;      |
| ipAddress          | String   | &check;      |
| privateIPv4Address | String   | &check;      |
