SonarCloud
==========
Resmo's SonarCloud integration enables you to analyze and monitor your code quality and security data in a comprehensive manner. SonarCloud is a popular cloud-based code quality and security analysis platform that helps developers identify and fix issues in their code. By connecting Resmo with SonarCloud, you can access and query data from SonarCloud to gain insights into your organization's code quality, security vulnerabilities, and development practices.

Utilizing Resmo's SQL query capabilities, you can explore complex questions about your SonarCloud data, such as:

* What are the key metrics and trends for each project, including code quality, security vulnerabilities, and code coverage?
* How many pull requests have been analyzed, and what are their statuses?
* What are the users, user groups, and their respective permissions within the organization?
* Which webhooks are configured for each project, and when were they last delivered?

By setting up change alerts in Resmo, you can stay informed about important updates and events in your SonarCloud data. For example:

* Get notified when a new project is added or when an existing project's metrics change significantly.
* Receive an alert when a pull request analysis is completed or when its status changes.
* Get notified when a user or user group is added, modified, or removed.
* Receive an alert when a webhook is created, updated, or deleted.

Integrating your SonarCloud account with Resmo allows you to efficiently monitor and analyze your organization's code quality and security data, ensuring that your codebase remains reliable and secure. With Resmo's SQL query capabilities and change alerting, you can stay informed about crucial changes and events in your SonarCloud data, allowing you to make better decisions regarding your code quality, security, and development practices.

| **Resources** | **Key**                                                   | **Supports Events** |
| ------------- | --------------------------------------------------------- | ------------------- |
| Project       | [sonarcloud\_project](sonarcloud\_project.md)             |                     |
| Pull Request  | [sonarcloud\_pull\_request](sonarcloud\_pull\_request.md) |                     |
| User          | [sonarcloud\_user](sonarcloud\_user.md)                   |                     |
| User Group    | [sonarcloud\_user\_group](sonarcloud\_user\_group.md)     |                     |
| Webhook       | [sonarcloud\_webhook](sonarcloud\_webhook.md)             |                     |
