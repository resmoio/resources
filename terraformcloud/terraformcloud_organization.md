---
description: Terraform Cloud Organization
---
terraformcloud_organization
---------------------------

| **Name**                                          | **Type**            | **Nullable** |
| ------------------------------------------------- | ------------------- | ------------ |
| allowForceDeleteWorkspaces                        | Boolean             | &check;      |
| assessmentsEnforced                               | Boolean             | &check;      |
| collaboratorAuthPolicy                            | String              | &check;      |
| costEstimationEnabled                             | Boolean             | &check;      |
| createdAt                                         | String              | &check;      |
| email                                             | String              | &check;      |
| externalId                                        | String              | &check;      |
| fairRunQueuingEnabled                             | Boolean             | &check;      |
| id                                                | String              | &cross;      |
| name                                              | String              | &check;      |
| permissions                                       | Map<String,Boolean> | &check;      |
| planExpired                                       | Boolean             | &check;      |
| planExpiresAt                                     | String              | &check;      |
| planIdentifier                                    | String              | &check;      |
| planIsEnterprise                                  | Boolean             | &check;      |
| planIsTrial                                       | Boolean             | &check;      |
| samlEnabled                                       | Boolean             | &check;      |
| sendPassingStatusesForUntriggeredSpeculativePlans | Boolean             | &check;      |
| sessionRemember                                   | String              | &check;      |
| sessionTimeout                                    | String              | &check;      |
| twoFactorConformant                               | Boolean             | &check;      |
| type                                              | String              | &check;      |
