---
description: Amazon Web Services EC2 Snapshot
---
aws_ec2_snapshot
----------------

| **Name**    | **Type**           | **Nullable** |
| ----------- | ------------------ | ------------ |
| accountId   | String             | &cross;      |
| accountName | String             | &check;      |
| description | String             | &cross;      |
| encrypted   | Boolean            | &cross;      |
| id          | String             | &cross;      |
| kmsKeyID    | String             | &check;      |
| name        | String             | &cross;      |
| region      | String             | &cross;      |
| state       | String             | &cross;      |
| tags        | Map<String,String> | &cross;      |
| volumeSize  | Int                | &cross;      |
