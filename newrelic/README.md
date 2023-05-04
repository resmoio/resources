New Relic
=========
Integrating Resmo with New Relic can offer numerous advantages for monitoring and optimizing your application configuration settings. New Relic is a comprehensive application performance management (APM) platform that provides real-time visibility into your applications' performance, reliability, and scalability. Resmo can collect and analyze various resources from New Relic's API, such as Account, User, API Key, Device Configuration, Alert Policy, Notification Channel, Muting Rule and more.

With Resmo's SQL query capabilities, users can ask intricate questions about their New Relic configuration data. For instance:

* Which users are associated with specific API keys?
* What are the device configurations for a particular Mobile Application?
* Which Alert Policies have the most conditions attached?
* What are the notification channels assigned to a specific Alert Policy?
* Which Infrastructure Hosts have specific tags assigned?

Setting up configuration alerts in Resmo can also be beneficial for proactively monitoring critical changes in your New Relic settings. For example:

* Get notified when a new API key is created or deleted.
* Receive an alert when a change is made to a Device Configuration.
* Get notified when a new Alert Policy is created, updated, or deleted.
* Receive an alert when a Notification Channel is added or removed from an Alert Policy.
* Get notified when a Muting Rule is enabled, disabled, or updated.

In conclusion, connecting your New Relic account to Resmo can provide valuable insights into your application's configuration settings, helping you optimize your applications for maximum efficiency. By leveraging Resmo's SQL query capabilities and configuration alerting, you can stay on top of important changes and enhance your New Relic settings for optimal performance.

| **Resources**        | **Key**                                                               | **Supports Events** |
| -------------------- | --------------------------------------------------------------------- | ------------------- |
| Account              | [newrelic\_account](newrelic\_account.md)                             |                     |
| Alert Policy         | [newrelic\_alert\_policy](newrelic\_alert\_policy.md)                 |                     |
| API Key              | [newrelic\_api\_key](newrelic\_api\_key.md)                           |                     |
| Browser Application  | [newrelic\_browser\_application](newrelic\_browser\_application.md)   |                     |
| Dashboard            | [newrelic\_dashboard](newrelic\_dashboard.md)                         |                     |
| Device Configuration | [newrelic\_device\_configuration](newrelic\_device\_configuration.md) |                     |
| Infrastructure Host  | [newrelic\_infrastructure\_host](newrelic\_infrastructure\_host.md)   |                     |
| Mobile Application   | [newrelic\_mobile\_application](newrelic\_mobile\_application.md)     |                     |
| Muting Rule          | [newrelic\_muting\_rule](newrelic\_muting\_rule.md)                   |                     |
| Notification Channel | [newrelic\_notification\_channel](newrelic\_notification\_channel.md) |                     |
| Synthetic Monitor    | [newrelic\_synthetic\_monitor](newrelic\_synthetic\_monitor.md)       |                     |
| User                 | [newrelic\_user](newrelic\_user.md)                                   |                     |
| Workload             | [newrelic\_workload](newrelic\_workload.md)                           |                     |
