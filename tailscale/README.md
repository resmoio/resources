Tailscale
=========
Integrating your Tailscale account with Resmo offers valuable insights into your organization's private networking, device management, and security. Tailscale is a secure, user-friendly VPN service that allows you to create a private network for your devices, making it easy to access resources and communicate securely. Resmo can collect and analyze data from Tailscale, which can be useful for understanding your network configuration, device connections, and access control policies.

Using Resmo's SQL query capabilities, users can ask complex questions about their Tailscale data, such as:

* What are the details of devices on the network, including their operating systems, hostnames, and connectivity status?
* Which devices have specific routes enabled or are blocking incoming connections?
* How are access control policies configured, and what groups or hosts are associated with them?
* What are the DNS preferences and settings for the Tailscale network, such as nameservers and search paths?
* How are Tailscale keys created, and what capabilities do they have?

Setting up change alerts can be helpful for monitoring critical changes in your Tailscale data. For example:

* Get notified when a new device joins the network or an existing device's status changes.
* Receive an alert when a device's routes or security settings are modified.
* Get notified when an access control policy is created, updated, or deleted.
* Receive an alert when DNS preferences or settings change within the Tailscale network.
* Get notified when a Tailscale key is created, expires, or has its capabilities updated.

In conclusion, integrating your Tailscale account with Resmo provides valuable insights into your organization's private networking, device management, and security. By leveraging Resmo's SQL query capabilities and change alerting, you can stay on top of important changes and ensure that your Tailscale configurations are optimized for maximum efficiency and effectiveness.

| **Resources**       | **Key**                                                                 | **Supports Events** |
| ------------------- | ----------------------------------------------------------------------- | ------------------- |
| Access Control List | [tailscale\_access\_control\_list](tailscale\_access\_control\_list.md) |                     |
| Device              | [tailscale\_device](tailscale\_device.md)                               |                     |
| DNS                 | [tailscale\_dns](tailscale\_dns.md)                                     |                     |
| Key                 | [tailscale\_key](tailscale\_key.md)                                     |                     |
