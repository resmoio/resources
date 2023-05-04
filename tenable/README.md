Tenable.io
==========
Integrating your Tenable account with Resmo offers valuable insights into your organization's vulnerability management and security configurations. Tenable is a leading cybersecurity solution that provides vulnerability assessment, detection, and remediation capabilities. Resmo can collect and analyze configuration data from Tenable, which can be useful for identifying potential security risks, ensuring adherence to best practices, and optimizing configurations.

Using Resmo's SQL query capabilities, users can ask complex questions about their Tenable data, such as:

* What are the details of users, their associated groups, and permissions?
* How are user groups configured, including their permissions and user counts?
* What are the properties of vulnerability scans, including schedules and progress?
* What are the details of detected vulnerabilities, including severity and affected assets?
* How are assets configured, including IP addresses, hostnames, and installed software?

Setting up change alerts can be helpful for monitoring critical changes in your Tenable data. For example:

* Get notified when a new user is added or removed, or when their permissions change.
* Receive an alert when a user group's configuration or membership is updated.
* Get notified when a vulnerability scan is created, modified, or deleted, including changes to schedules or progress.
* Receive an alert when new vulnerabilities are detected, or when existing vulnerabilities are fixed.
* Get notified when assets are added, removed, or have their properties updated.

In conclusion, integrating your Tenable account with Resmo provides valuable insights into your organization's vulnerability management and security configurations. By leveraging Resmo's SQL query capabilities and change alerting, you can stay on top of important changes and ensure that your Tenable configurations are optimized for maximum efficiency and effectiveness.

| **Resources** | **Key**                                             | **Supports Events** |
| ------------- | --------------------------------------------------- | ------------------- |
| Asset         | [tenable\_asset](tenable\_asset.md)                 |                     |
| Scan          | [tenable\_scan](tenable\_scan.md)                   |                     |
| User          | [tenable\_user](tenable\_user.md)                   |                     |
| User Group    | [tenable\_user\_group](tenable\_user\_group.md)     |                     |
| Vulnerability | [tenable\_vulnerability](tenable\_vulnerability.md) |                     |
