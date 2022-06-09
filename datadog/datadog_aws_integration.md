---
description: Datadog AWS Integration
---
datadog_aws_integration
-----------------------

| **Name**                      | **Type**            | **Nullable** |
| ----------------------------- | ------------------- | ------------ |
| accessKeyId                   | String              | &check;      |
| accountId                     | String              | &cross;      |
| accountSpecificNamespaceRules | Map<String,Boolean> | &check;      |
| cspmResourceCollectionEnabled | Boolean             | &check;      |
| excludedRegions               | List<String>        | &check;      |
| filterTags                    | List<String>        | &check;      |
| hostTags                      | List<String>        | &check;      |
| metricsCollectionEnabled      | Boolean             | &check;      |
| resourceCollectionEnabled     | Boolean             | &check;      |
| roleName                      | String              | &check;      |
| secretAccessKey               | String              | &check;      |
