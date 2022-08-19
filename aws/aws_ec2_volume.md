---
description: Amazon Web Services EC2 Volume
---
aws_ec2_volume
--------------

| **Name**    | **Type**           | **Nullable** |
| ----------- | ------------------ | ------------ |
| accountId   | String             | &cross;      |
| accountName | String             | &check;      |
| createTime  | String             | &check;      |
| encrypted   | Boolean            | &check;      |
| id          | String             | &cross;      |
| iops        | Int                | &check;      |
| kmsKeyID    | String             | &check;      |
| name        | String             | &check;      |
| region      | String             | &cross;      |
| size        | Int                | &check;      |
| state       | String             | &check;      |
| tags        | Map<String,String> | &check;      |
| volumeId    | String             | &check;      |
| volumeType  | String             | &check;      |
| zone        | String             | &check;      |
