Terraform Cloud
===============
Integrating your Terraform Cloud account with Resmo offers valuable insights into your organization's infrastructure management, policy enforcement, and collaboration. Terraform Cloud is a popular infrastructure-as-code platform that enables you to manage, collaborate, and automate your infrastructure provisioning. Resmo can collect and analyze data from Terraform Cloud, which can be useful for understanding your infrastructure configurations, ensuring adherence to best practices, and optimizing your workflows.

Using Resmo's SQL query capabilities, users can ask complex questions about their Terraform Cloud data, such as:

* What are the details of organizations, including their policies, features, and permissions?
* How many policy sets are defined, and what are their associated policies and workspaces?
* What are the details of teams within the organization, including their access levels, permissions, and membership counts?
* How many workspaces exist within the organization, and what are their configurations, statuses, and associated version control repositories?
* Which user tokens are created, and how are they used within the organization?

Setting up change alerts can be helpful for monitoring critical changes in your Terraform Cloud data. For example:

* Get notified when a new organization is created, updated, or has changes in its settings or policies.
* Receive an alert when a policy set or policy is created, modified, or deleted.
* Get notified when a team is created, updated, or has changes in its access levels or permissions.
* Receive an alert when a new workspace is created, updated, or has changes in its configuration or status.
* Get notified when a user token is created, updated, or used within the organization.

In conclusion, integrating your Terraform Cloud account with Resmo provides valuable insights into your organization's infrastructure management, policy enforcement, and collaboration. By leveraging Resmo's SQL query capabilities and change alerting, you can stay on top of important changes and ensure that your Terraform Cloud configurations are optimized for maximum efficiency and effectiveness.

| **Resources** | **Key**                                                           | **Supports Events** |
| ------------- | ----------------------------------------------------------------- | ------------------- |
| Organization  | [terraformcloud\_organization](terraformcloud\_organization.md)   |                     |
| Policy        | [terraformcloud\_policy](terraformcloud\_policy.md)               |                     |
| Policy Check  | [terraformcloud\_policy\_check](terraformcloud\_policy\_check.md) |                     |
| Policy Set    | [terraformcloud\_policy\_set](terraformcloud\_policy\_set.md)     |                     |
| Team          | [terraformcloud\_team](terraformcloud\_team.md)                   |                     |
| Team Access   | [terraformcloud\_team\_access](terraformcloud\_team\_access.md)   |                     |
| User          | [terraformcloud\_user](terraformcloud\_user.md)                   |                     |
| User Token    | [terraformcloud\_user\_token](terraformcloud\_user\_token.md)     |                     |
| Workspace     | [terraformcloud\_workspace](terraformcloud\_workspace.md)         |                     |
