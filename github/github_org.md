---
description: GitHub Organization
---
github_org
----------

| **Name**                             | **Type** | **Nullable** |
| ------------------------------------ | -------- | ------------ |
| billingEmail                         | String   | &check;      |
| blog                                 | String   | &check;      |
| collaborators                        | Long     | &check;      |
| company                              | String   | &check;      |
| createdAt                            | Date     | &check;      |
| defaultRepositoryPermission          | String   | &check;      |
| description                          | String   | &check;      |
| email                                | String   | &check;      |
| followers                            | Long     | &check;      |
| following                            | Long     | &check;      |
| hasOrganizationProjects              | Boolean  | &check;      |
| hasRepositoryProjects                | Boolean  | &check;      |
| id                                   | Long     | &cross;      |
| isVerified                           | Boolean  | &check;      |
| location                             | String   | &check;      |
| login                                | String   | &cross;      |
| membersAllowedRepositoryCreationType | String   | &check;      |
| membersCanCreateInternalRepositories | Boolean  | &check;      |
| membersCanCreatePages                | Boolean  | &check;      |
| membersCanCreatePrivateRepositories  | Boolean  | &check;      |
| membersCanCreatePublicRepositories   | Boolean  | &check;      |
| membersCanCreateRepositories         | Boolean  | &check;      |
| membersCanForkPrivateRepositories    | Boolean  | &check;      |
| name                                 | String   | &check;      |
| nodeId                               | String   | &check;      |
| organizationId                       | String   | &cross;      |
| ownedPrivateRepos                    | Long     | &check;      |
| plan                                 | Plan     | &check;      |
| privateGists                         | Long     | &check;      |
| publicGists                          | Long     | &check;      |
| publicRepos                          | Long     | &check;      |
| totalPrivateRepos                    | Long     | &check;      |
| twitterUsername                      | String   | &check;      |
| twoFactorRequirementEnabled          | Boolean  | &check;      |
| type                                 | String   | &check;      |
| updatedAt                            | Date     | &check;      |

#### Plan
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| filledSeats  | Int      | &check;      |
| name         | String   | &check;      |
| privateRepos | Int      | &check;      |
| seats        | Int      | &check;      |
| space        | Int      | &check;      |
