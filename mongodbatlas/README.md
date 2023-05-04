MongoDB Atlas
=============

Connecting your MongoDB Atlas account to Resmo can be advantageous in various ways. MongoDB Atlas is a fully managed, global cloud database service for modern applications. Resmo can collect and analyze configuration data from MongoDB Atlas, which can be useful for identifying security risks, detecting best practices, and optimizing configurations.

Using Resmo's SQL query capabilities, users can ask complex questions about their MongoDB Atlas configuration data. For example:

* What are the settings of each cluster in your MongoDB Atlas project?
* How many clusters have backup enabled?
* What is the average disk size of clusters across your projects?
* Which clusters have the highest number of shards?
* How many network peering connections are established in your MongoDB Atlas projects?

Setting up change alerts can also be helpful for monitoring critical changes in your MongoDB Atlas configuration. For example:

* Get notified when a new cluster is created in your MongoDB Atlas project.
* Receive an alert when a cluster's configuration is updated.
* Get notified when a new network peering connection is established.
* Receive an alert when a private endpoint service's status changes.
* Get notified when an API key's roles are modified or added.

In conclusion, connecting your MongoDB Atlas account to Resmo can provide valuable insights into your organization's database management. By leveraging Resmo's SQL query capabilities and change alerting, you can stay on top of important changes and optimize your MongoDB Atlas configuration for maximum efficiency.

| **Resources**              | **Key**                                                                           | **Supports Events** |
| -------------------------- | --------------------------------------------------------------------------------- | ------------------- |
| Alert Configuration        | [mongodb\_alert\_configuration](mongodb\_alert\_configuration.md)                 |                     |
| Cloud Backup Schedule      | [mongodb\_cloud\_backup\_schedule](mongodb\_cloud\_backup\_schedule.md)           |                     |
| Cluster                    | [mongodb\_cluster](mongodb\_cluster.md)                                           |                     |
| Network Peering Connection | [mongodb\_network\_peering\_connection](mongodb\_network\_peering\_connection.md) |                     |
| Network Peering Container  | [mongodb\_network\_peering\_container](mongodb\_network\_peering\_container.md)   |                     |
| Organization               | [mongodb\_organization](mongodb\_organization.md)                                 |                     |
| Organization User          | [mongodb\_organization\_user](mongodb\_organization\_user.md)                     |                     |
| Private Endpoint Service   | [mongodb\_private\_endpoint\_service](mongodb\_private\_endpoint\_service.md)     |                     |
| API Key                    | [mongodb\_programmatic\_api\_key](mongodb\_programmatic\_api\_key.md)             |                     |
| Project                    | [mongodb\_project](mongodb\_project.md)                                           |                     |
| Root                       | [mongodb\_root](mongodb\_root.md)                                                 |                     |
| Serverless Instance        | [mongodb\_serverless\_instance](mongodb\_serverless\_instance.md)                 |                     |
| Organization Team          | [mongodb\_team](mongodb\_team.md)                                                 |                     |
