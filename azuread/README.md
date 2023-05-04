Azure Active Directory
======================
Connecting your Azure Active Directory (Azure AD) account to Resmo can be beneficial in various ways. Azure AD is Microsoft's cloud-based identity and access management service that helps organizations manage users, groups, and access to applications and resources. Resmo can collect and analyze configuration data from Azure AD, which can be useful for identifying security risks, detecting best practices, and optimizing configurations.

Using Resmo's SQL query capabilities, users can ask complex questions about their Azure AD configuration data. For example:

* Which users have access to a specific application?
* How many users are assigned to a particular group?
* What is the average number of assigned licenses per user?
* Which service principals have the highest number of app role assignments?
* How many conditional access policies are applied to specific resources?

Setting up change alerts can also be helpful for monitoring critical changes in your Azure AD configuration. For example:

* Get notified when a new user is added to your Azure AD tenant.
* Receive an alert when a user's assigned licenses change.
* Get notified when a new group is created in your Azure AD tenant.
* Receive an alert when a service principal's configuration is updated.
* Get notified when a conditional access policy is modified or added.

In conclusion, connecting your Azure AD account to Resmo can provide valuable insights into your organization's identity and access management. By leveraging Resmo's SQL query capabilities and change alerting, you can stay on top of important changes and optimize your Azure AD configuration for maximum efficiency.

| **Resources**             | **Key**                                                                             | **Supports Events** |
| ------------------------- | ----------------------------------------------------------------------------------- | ------------------- |
| Authorization Policy      | [azure\_ad\_authorization\_policy](azure\_ad\_authorization\_policy.md)             |                     |
| Conditional Access Policy | [azure\_ad\_conditional\_access\_policy](azure\_ad\_conditional\_access\_policy.md) |                     |
| OAuth2 Permission Grant   | [azure\_ad\_oauth2\_permission\_grant](azure\_ad\_oauth2\_permission\_grant.md)     |                     |
| Organization              | [azure\_ad\_organization](azure\_ad\_organization.md)                               |                     |
| Service Principal         | [azure\_ad\_service\_principal](azure\_ad\_service\_principal.md)                   |                     |
| User                      | [azure\_ad\_user](azure\_ad\_user.md)                                               |                     |
| User Group                | [azure\_ad\_user\_group](azure\_ad\_user\_group.md)                                 |                     |
