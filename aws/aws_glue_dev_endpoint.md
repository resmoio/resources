---
description: Amazon Web Services Glue Dev Endpoint
---
aws_glue_dev_endpoint
---------------------

| **Name**                           | **Type**           | **Nullable** |
| ---------------------------------- | ------------------ | ------------ |
| accountId                          | String             | &cross;      |
| accountName                        | String             | &check;      |
| arguments                          | Map<String,String> | &check;      |
| availabilityZone                   | String             | &check;      |
| createdTimestamp                   | String             | &check;      |
| extraJarsS3Path                    | String             | &check;      |
| extraPythonLibsS3Path              | String             | &check;      |
| failureReason                      | String             | &check;      |
| glueVersion                        | String             | &check;      |
| lastModifiedTimestamp              | String             | &check;      |
| lastUpdateStatus                   | String             | &check;      |
| name                               | String             | &cross;      |
| numberOfNodes                      | Int                | &check;      |
| numberOfWorkers                    | Int                | &check;      |
| privateAddress                     | String             | &check;      |
| publicAddress                      | String             | &check;      |
| publicKey                          | String             | &check;      |
| publicKeys                         | List<String>       | &check;      |
| region                             | String             | &cross;      |
| roleArn                            | String             | &check;      |
| securityConfiguration              | String             | &check;      |
| securityGroupIds                   | List<String>       | &check;      |
| status                             | String             | &check;      |
| subnetId                           | String             | &check;      |
| vpcId                              | String             | &check;      |
| workerType                         | String             | &check;      |
| yarnEndpointAddress                | String             | &check;      |
| zeppelinRemoteSparkInterpreterPort | Int                | &check;      |
