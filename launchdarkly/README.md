LaunchDarkly
============
Integrating your LaunchDarkly account with Resmo offers valuable insights into your organization's feature flag management, projects, environments, and team information. LaunchDarkly is a feature management platform that allows you to deploy, manage, and control feature flags across your applications. Resmo can collect and analyze data from LaunchDarkly, which can be useful for understanding your feature flag configurations, project settings, environments, and team assignments.

Using Resmo's SQL query capabilities, users can ask complex questions about their LaunchDarkly data, such as:

* Which feature flags are active, archived, or temporary, and what are their variations?
* How are environments configured, and what are their API keys and settings?
* What are the details of each project, including environments, default client-side availability, and tags?
* How are account members and teams organized, and what are their roles and permissions?
* Which webhooks are active and what are their configurations, including URLs, secrets, and associated events?

Setting up change alerts can be helpful for monitoring critical changes in your LaunchDarkly data. For example:

* Get notified when a new feature flag is created, updated, or archived.
* Receive an alert when a project is created, updated, or deleted.
* Get notified when an environment's configuration changes, such as API keys or settings.
* Receive an alert when a team member's role or permissions are updated, or when a new member is added to a team.
* Get notified when a webhook is created, updated, or deleted.

In conclusion, integrating your LaunchDarkly account with Resmo provides valuable insights into your organization's feature flag management, projects, environments, and team information. By leveraging Resmo's SQL query capabilities and change alerting, you can stay on top of important changes and ensure that your LaunchDarkly configurations are optimized for maximum efficiency and effectiveness.

| **Resources**  | **Key**                                                           | **Supports Events** |
| -------------- | ----------------------------------------------------------------- | ------------------- |
| Access Token   | [launchdarkly\_access\_token](launchdarkly\_access\_token.md)     |                     |
| Account Member | [launchdarkly\_account\_member](launchdarkly\_account\_member.md) |                     |
| Custom Role    | [launchdarkly\_custom\_role](launchdarkly\_custom\_role.md)       |                     |
| Environment    | [launchdarkly\_environment](launchdarkly\_environment.md)         |                     |
| Feature Flag   | [launchdarkly\_feature\_flag](launchdarkly\_feature\_flag.md)     |                     |
| Project        | [launchdarkly\_project](launchdarkly\_project.md)                 |                     |
| Team           | [launchdarkly\_team](launchdarkly\_team.md)                       |                     |
| Webhook        | [launchdarkly\_webhook](launchdarkly\_webhook.md)                 |                     |
