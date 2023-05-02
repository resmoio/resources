Azure
=====
Azure is a cloud computing platform provided by Microsoft. Resmo can connect to an Azure account to collect configuration data from various Azure resources, including virtual machines, storage accounts, network security groups, and Cosmos DB accounts. Resmo can help users monitor the configuration of their Azure resources, detect security issues, and ensure best practices are followed.

With Resmo's SQL queries, users can ask complex questions about their Azure configuration data. For example:

* Which virtual machines have open ports to the internet?
* Which storage accounts are publicly accessible?
* Which network security groups allow traffic from all IP addresses?
* Which Cosmos DB accounts are not encrypted?
* Which Azure Kubernetes Service (AKS) clusters have outdated node versions?

Users can also set alarms to receive notifications when critical changes occur in their Azure resources. For example:

* Receive an alert when a new virtual machine is created.
* Receive an alert when a network security group's rules are modified.
* Receive an alert when a storage account's permissions are changed.
* Receive an alert when a Cosmos DB account's encryption status changes.
* Receive an alert when an AKS cluster's node version is outdated.

| **Resources**                             | **Key**                                                                                                         | **Supports Events** |
| ----------------------------------------- | --------------------------------------------------------------------------------------------------------------- | ------------------- |
| Activity Log Alert Rule                   | [azure\_activity\_log\_alert\_rule](azure\_activity\_log\_alert\_rule.md)                                       |                     |
| App Service App                           | [azure\_app\_service\_app](azure\_app\_service\_app.md)                                                         |                     |
| Compute Disk                              | [azure\_compute\_disk](azure\_compute\_disk.md)                                                                 |                     |
| Container Group                           | [azure\_container\_group](azure\_container\_group.md)                                                           |                     |
| Container Registry                        | [azure\_container\_registry](azure\_container\_registry.md)                                                     |                     |
| Cosmos Account                            | [azure\_cosmos\_account](azure\_cosmos\_account.md)                                                             |                     |
| Dns Zone                                  | [azure\_dns\_zone](azure\_dns\_zone.md)                                                                         |                     |
| Key Vault                                 | [azure\_key\_vault](azure\_key\_vault.md)                                                                       |                     |
| Kubernetes Cluster                        | [azure\_kubernetes\_cluster](azure\_kubernetes\_cluster.md)                                                     |                     |
| MySql Server                              | [azure\_mysql\_server](azure\_mysql\_server.md)                                                                 |                     |
| Network Interface                         | [azure\_network\_interface](azure\_network\_interface.md)                                                       |                     |
| Network Security Group                    | [azure\_network\_security\_group](azure\_network\_security\_group.md)                                           |                     |
| Network Watcher                           | [azure\_network\_watcher](azure\_network\_watcher.md)                                                           |                     |
| Policy Assignment                         | [azure\_policy\_assignment](azure\_policy\_assignment.md)                                                       |                     |
| Policy State                              | [azure\_policy\_state](azure\_policy\_state.md)                                                                 |                     |
| PostgreSql Server                         | [azure\_postgresql\_server](azure\_postgresql\_server.md)                                                       |                     |
| Public IP Address                         | [azure\_public\_ip\_address](azure\_public\_ip\_address.md)                                                     |                     |
| Resource Group                            | [azure\_resource\_group](azure\_resource\_group.md)                                                             |                     |
| Security Assessment                       | [azure\_security\_assessment](azure\_security\_assessment.md)                                                   |                     |
| Security Center Auto Provisioning Setting | [azure\_security\_center\_auto\_provisioning\_setting](azure\_security\_center\_auto\_provisioning\_setting.md) |                     |
| Security Center Setting                   | [azure\_security\_center\_setting](azure\_security\_center\_setting.md)                                         |                     |
| Security Center Subscription Pricing      | [azure\_security\_center\_subscription\_pricing](azure\_security\_center\_subscription\_pricing.md)             |                     |
| Security Contact                          | [azure\_security\_contact](azure\_security\_contact.md)                                                         |                     |
| Sql Database                              | [azure\_sql\_database](azure\_sql\_database.md)                                                                 |                     |
| Sql Server                                | [azure\_sql\_server](azure\_sql\_server.md)                                                                     |                     |
| Storage Account                           | [azure\_storage\_account](azure\_storage\_account.md)                                                           |                     |
| Storage Blob Container                    | [azure\_storage\_blob\_container](azure\_storage\_blob\_container.md)                                           |                     |
| Storage Queue                             | [azure\_storage\_queue](azure\_storage\_queue.md)                                                               |                     |
| Storage Table                             | [azure\_storage\_table](azure\_storage\_table.md)                                                               |                     |
| Subscription                              | [azure\_subscription](azure\_subscription.md)                                                                   |                     |
| Virtual Machine                           | [azure\_virtual\_machine](azure\_virtual\_machine.md)                                                           |                     |
| Virtual Network                           | [azure\_virtual\_network](azure\_virtual\_network.md)                                                           |                     |
