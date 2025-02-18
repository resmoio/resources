Google Cloud Platform
=====================
GCP (Google Cloud Platform) is a cloud computing platform provided by Google. Resmo can connect to a GCP account to collect configuration data from various GCP resources, including Compute Engine instances, Cloud Storage buckets, VPC firewall rules, and IAM users. Resmo can help users monitor the configuration of their GCP resources, detect security issues, and ensure best practices are followed.

With Resmo's SQL queries, users can ask complex questions about their GCP configuration data. For example:

* Which Compute Engine instances are exposed to the internet?
* Which Cloud Storage buckets are publicly accessible?
* Which VPC firewall rules allow traffic from all IP addresses?
* Which IAM users have not logged in within the last 90 days?
* Which databases are not encrypted?

Users can also set alarms to receive notifications when critical changes occur in their GCP resources. For example:

* Receive an alert when a new Compute Engine instance is created.
* Receive an alert when a VPC firewall rule's configuration is changed.
* Receive an alert when a Cloud Storage bucket's permissions are changed.
* Receive an alert when a new IAM user is created.
* Receive an alert when a database's encryption status changes.

| **Resources**                | **Key**                                                                       | **Supports Events** |
| ---------------------------- | ----------------------------------------------------------------------------- | ------------------- |
| API Gateway API              | [gcp\_apigateway\_api](gcp\_apigateway\_api.md)                               |                     |
| API Gateway API Config       | [gcp\_apigateway\_api\_config](gcp\_apigateway\_api\_config.md)               |                     |
| API Gateway Gateway          | [gcp\_apigateway\_gateway](gcp\_apigateway\_gateway.md)                       |                     |
| AppEngine Application        | [gcp\_appengine\_application](gcp\_appengine\_application.md)                 |                     |
| AppEngine Instance           | [gcp\_appengine\_instance](gcp\_appengine\_instance.md)                       |                     |
| AppEngine Service            | [gcp\_appengine\_service](gcp\_appengine\_service.md)                         |                     |
| AppEngine Version            | [gcp\_appengine\_version](gcp\_appengine\_version.md)                         |                     |
| BigQuery Dataset             | [gcp\_bigquery\_dataset](gcp\_bigquery\_dataset.md)                           |                     |
| BigQuery Model               | [gcp\_bigquery\_model](gcp\_bigquery\_model.md)                               |                     |
| BigQuery Table               | [gcp\_bigquery\_table](gcp\_bigquery\_table.md)                               |                     |
| BigTable Application Profile | [gcp\_bigtable\_application\_profile](gcp\_bigtable\_application\_profile.md) |                     |
| BigTable Backup              | [gcp\_bigtable\_backup](gcp\_bigtable\_backup.md)                             |                     |
| BigTable Cluster             | [gcp\_bigtable\_cluster](gcp\_bigtable\_cluster.md)                           |                     |
| BigTable Instance            | [gcp\_bigtable\_instance](gcp\_bigtable\_instance.md)                         |                     |
| BigTable Table               | [gcp\_bigtable\_table](gcp\_bigtable\_table.md)                               |                     |
| Function                     | [gcp\_cloud\_function](gcp\_cloud\_function.md)                               |                     |
| Cloud Storage Bucket         | [gcp\_cloudstorage\_bucket](gcp\_cloudstorage\_bucket.md)                     | &check;             |
| Compute Backend Bucket       | [gcp\_compute\_backend\_bucket](gcp\_compute\_backend\_bucket.md)             |                     |
| Compute Backend Service      | [gcp\_compute\_backend\_service](gcp\_compute\_backend\_service.md)           |                     |
| Compute Disk                 | [gcp\_compute\_disk](gcp\_compute\_disk.md)                                   |                     |
| Compute Health Check         | [gcp\_compute\_health\_check](gcp\_compute\_health\_check.md)                 |                     |
| Compute Instance             | [gcp\_compute\_instance](gcp\_compute\_instance.md)                           | &check;             |
| Compute Instance Group       | [gcp\_compute\_instance\_group](gcp\_compute\_instance\_group.md)             |                     |
| Compute LoadBalancer         | [gcp\_compute\_loadbalancer](gcp\_compute\_loadbalancer.md)                   |                     |
| Compute Project              | [gcp\_compute\_project](gcp\_compute\_project.md)                             |                     |
| Compute Snapshot             | [gcp\_compute\_snapshot](gcp\_compute\_snapshot.md)                           |                     |
| Compute SSL Policy           | [gcp\_compute\_ssl\_policy](gcp\_compute\_ssl\_policy.md)                     |                     |
| Compute Target HttpProxy     | [gcp\_compute\_target\_http\_proxy](gcp\_compute\_target\_http\_proxy.md)     |                     |
| Compute Target HttpsProxy    | [gcp\_compute\_target\_https\_proxy](gcp\_compute\_target\_https\_proxy.md)   |                     |
| Compute Target SSLProxy      | [gcp\_compute\_target\_ssl\_proxy](gcp\_compute\_target\_ssl\_proxy.md)       |                     |
| DNS Managed Zone             | [gcp\_dns\_managed\_zone](gcp\_dns\_managed\_zone.md)                         |                     |
| DNS Policy                   | [gcp\_dns\_policy](gcp\_dns\_policy.md)                                       |                     |
| DNS Record Set               | [gcp\_dns\_record\_set](gcp\_dns\_record\_set.md)                             |                     |
| GKE Cluster                  | [gcp\_gke\_cluster](gcp\_gke\_cluster.md)                                     | &check;             |
| IAM Policy                   | [gcp\_iam\_policy](gcp\_iam\_policy.md)                                       |                     |
| IAM Role                     | [gcp\_iam\_role](gcp\_iam\_role.md)                                           |                     |
| IAM Service Account          | [gcp\_iam\_service\_account](gcp\_iam\_service\_account.md)                   |                     |
| IAM Service Account Key      | [gcp\_iam\_service\_account\_key](gcp\_iam\_service\_account\_key.md)         |                     |
| KMS Crypto Key               | [gcp\_kms\_crypto\_key](gcp\_kms\_crypto\_key.md)                             |                     |
| KMS Keyring                  | [gcp\_kms\_keyring](gcp\_kms\_keyring.md)                                     |                     |
| Logging Metric               | [gcp\_logging\_metric](gcp\_logging\_metric.md)                               |                     |
| Logging Sink                 | [gcp\_logging\_sink](gcp\_logging\_sink.md)                                   |                     |
| Memcache Instance            | [gcp\_memcache\_instance](gcp\_memcache\_instance.md)                         |                     |
| Monitoring Alert Policy      | [gcp\_monitoring\_alert\_policy](gcp\_monitoring\_alert\_policy.md)           |                     |
| GCP Organization             | [gcp\_organization](gcp\_organization.md)                                     |                     |
| GCP Project                  | [gcp\_project](gcp\_project.md)                                               |                     |
| GCP Project Service          | [gcp\_project\_service](gcp\_project\_service.md)                             |                     |
| PUB/SUB Subscription         | [gcp\_pubsub\_subscription](gcp\_pubsub\_subscription.md)                     | &check;             |
| PUB/SUB Topic                | [gcp\_pubsub\_topic](gcp\_pubsub\_topic.md)                                   | &check;             |
| Redis Instance               | [gcp\_redis\_instance](gcp\_redis\_instance.md)                               |                     |
| GCP Region                   | [gcp\_region](gcp\_region.md)                                                 |                     |
| Spanner Database             | [gcp\_spanner\_database](gcp\_spanner\_database.md)                           |                     |
| Spanner Instance             | [gcp\_spanner\_instance](gcp\_spanner\_instance.md)                           |                     |
| Spanner Instance Config      | [gcp\_spanner\_instance\_config](gcp\_spanner\_instance\_config.md)           |                     |
| SQL Backup                   | [gcp\_sql\_backup](gcp\_sql\_backup.md)                                       |                     |
| SQL Database                 | [gcp\_sql\_database](gcp\_sql\_database.md)                                   |                     |
| SQL Instance                 | [gcp\_sql\_instance](gcp\_sql\_instance.md)                                   |                     |
| VPC Address                  | [gcp\_vpc\_address](gcp\_vpc\_address.md)                                     |                     |
| VPC Firewall                 | [gcp\_vpc\_firewall](gcp\_vpc\_firewall.md)                                   | &check;             |
| VPC Forwarding Rule          | [gcp\_vpc\_forwarding\_rule](gcp\_vpc\_forwarding\_rule.md)                   |                     |
| VPC Network                  | [gcp\_vpc\_network](gcp\_vpc\_network.md)                                     | &check;             |
| VPC Subnet                   | [gcp\_vpc\_subnet](gcp\_vpc\_subnet.md)                                       | &check;             |
