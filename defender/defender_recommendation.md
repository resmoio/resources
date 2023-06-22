---
description: Defender Recommendation
---
defender_recommendation
-----------------------

| **Name**                      | **Type**     | **Nullable** |
| ----------------------------- | ------------ | ------------ |
| activeAlert                   | Boolean      | &check;      |
| associatedThreats             | List<String> | &check;      |
| configScoreImpact             | Double       | &check;      |
| exposedMachinesCount          | Int          | &check;      |
| exposureImpact                | Double       | &check;      |
| hasUnpatchableCve             | Boolean      | &check;      |
| id                            | String       | &cross;      |
| nonProductivityImpactedAssets | Int          | &check;      |
| productName                   | String       | &check;      |
| publicExploit                 | Boolean      | &check;      |
| recommendationCategory        | String       | &check;      |
| recommendationName            | String       | &check;      |
| recommendedProgram            | String       | &check;      |
| recommendedVendor             | String       | &check;      |
| recommendedVersion            | String       | &check;      |
| relatedComponent              | String       | &check;      |
| remediationType               | String       | &check;      |
| severityScore                 | Double       | &check;      |
| status                        | String       | &check;      |
| subCategory                   | String       | &check;      |
| tags                          | List<String> | &check;      |
| totalMachineCount             | Int          | &check;      |
| vendor                        | String       | &check;      |
| weaknesses                    | Int          | &check;      |
