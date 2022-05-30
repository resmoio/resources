---
description: Opsgenie User
---
opsgenie_user
-------------

| **Name**           | **Type**             | **Nullable** |
| ------------------ | -------------------- | ------------ |
| accountName        | String               | &check;      |
| blocked            | Boolean              | &cross;      |
| contact            | List<Contact>        | &check;      |
| createdAt          | String               | &cross;      |
| details            | Map<String,List>     | &check;      |
| escalations        | List<Escalation>     | &check;      |
| fullName           | String               | &cross;      |
| id                 | String               | &cross;      |
| locale             | String               | &cross;      |
| role               | Role                 | &cross;      |
| schedule           | List<Schedule>       | &check;      |
| tags               | List<String>         | &check;      |
| team               | List<Team>           | &check;      |
| timeZone           | String               | &cross;      |
| userAddress        | UserAddress          | &cross;      |
| userForwardingRule | List<ForwardingRule> | &check;      |
| username           | String               | &cross;      |
| verified           | Boolean              | &cross;      |

#### Contact
| **Name**   | **Type**       | **Nullable** |
| ---------- | -------------- | ------------ |
| applyOrder | Int            | &check;      |
| id         | String         | &check;      |
| method     | String         | &check;      |
| status     | Contact.Status | &check;      |
| to         | String         | &check;      |

#### Contact.Status
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### Escalation
| **Name**  | **Type**              | **Nullable** |
| --------- | --------------------- | ------------ |
| id        | String                | &check;      |
| name      | String                | &check;      |
| ownerTeam | Escalation.OwnerTeam  | &check;      |
| rules     | List<Escalation.Rule> | &check;      |

#### Escalation.OwnerTeam
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Escalation.Rule
| **Name**   | **Type**                  | **Nullable** |
| ---------- | ------------------------- | ------------ |
| condition  | String                    | &check;      |
| delay      | Escalation.Rule.Delay     | &check;      |
| notifyType | String                    | &check;      |
| recipient  | Escalation.Rule.Recipient | &check;      |

#### Escalation.Rule.Delay
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| timeAmount | Int      | &check;      |
| timeUnit   | String   | &check;      |

#### Escalation.Rule.Recipient
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### ForwardingRule
| **Name**  | **Type**                          | **Nullable** |
| --------- | --------------------------------- | ------------ |
| alias     | String                            | &check;      |
| endDate   | String                            | &check;      |
| fromUser  | ForwardingRule.ForwardingRuleUser | &check;      |
| id        | String                            | &check;      |
| startDate | String                            | &check;      |
| toUser    | ForwardingRule.ForwardingRuleUser | &check;      |

#### ForwardingRule.ForwardingRuleUser
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| username | String   | &check;      |

#### Role
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Schedule
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### UserAddress
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| city     | String   | &check;      |
| country  | String   | &check;      |
| line     | String   | &check;      |
| state    | String   | &check;      |
| zipCode  | String   | &check;      |
