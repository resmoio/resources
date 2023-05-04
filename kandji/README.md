Kandji
======
Integrating your Kandji account with Resmo offers valuable insights into your organization's device management, blueprints, and user information. Kandji is a comprehensive Mobile Device Management (MDM) solution that helps you manage and secure macOS, iOS, and tvOS devices in your organization. Resmo can collect and analyze data from Kandji, which can be useful for understanding your device configurations, blueprints, and user assignments.

Using Resmo's SQL query capabilities, users can ask complex questions about their Kandji data, such as:

* Which devices are enrolled in specific blueprints, and what are their configurations?
* How many devices are missing or removed from the system, and which blueprint do they belong to?
* What are the hardware and software details of each device, including model, OS version, and installed profiles?
* What are the user assignments for each device, and which users are archived?
* How are device parameters configured, and which devices have the Kandji Agent installed?

Setting up change alerts can be helpful for monitoring critical changes in your Kandji data. For example:

* Get notified when a new device is enrolled or an existing device is updated.
* Receive an alert when a blueprint is created, updated, or deleted.
* Get notified when a device's status changes, such as going missing or being removed.
* Receive an alert when a user is added, removed, or their assignment changes on a device.
* Get notified when device parameters or installed profiles are updated or modified.

In conclusion, integrating your Kandji account with Resmo provides valuable insights into your organization's device management, blueprints, and user information. By leveraging Resmo's SQL query capabilities and change alerting, you can stay on top of important changes and ensure that your Kandji configurations are optimized for maximum efficiency and effectiveness.

| **Resources** | **Key**                                   | **Supports Events** |
| ------------- | ----------------------------------------- | ------------------- |
| Blueprint     | [kandji\_blueprint](kandji\_blueprint.md) |                     |
| Device        | [kandji\_device](kandji\_device.md)       |                     |
| User          | [kandji\_user](kandji\_user.md)           |                     |
