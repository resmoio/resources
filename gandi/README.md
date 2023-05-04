Gandi
=====
Integrating your Gandi account with Resmo can provide valuable insights into your domain management, SSL certificates, and DNS configurations. Gandi is a popular domain registrar and web hosting company that offers a wide range of services, including domain registration, SSL certificates, and DNS management. Resmo collects and analyzes Gandi's configuration data, which can help identify security risks, ensure adherence to best practices, and optimize configurations for efficiency and security.

Using Resmo's SQL query capabilities, users can ask complex questions about their Gandi configuration data, such as:

* Which domains have auto-renew enabled or disabled, and when are they set to expire?
* What are the SSL certificate details, including issuance and expiration dates, for each domain?
* How many glue records and DNSSEC keys are configured for each domain, and what are their details?
* What web redirection settings are in place for each domain, and are they using the correct protocols?
* How are contacts and organizations associated with domains, and what roles do they play?

Setting up change alerts in Resmo for your Gandi account can also be beneficial for monitoring critical configuration changes, such as:

* Notifications when domains are registered, updated, or deleted.
* Alerts when SSL certificates are issued, renewed, or expire.
* Updates when domain contacts or organizations are modified or removed.
* Notifications when DNS configurations, such as glue records or DNSSEC keys, are changed.
* Alerts when domain web redirection settings or LiveDNS information are modified.

In conclusion, integrating your Gandi account with Resmo offers valuable insights into your organization's domain management, SSL certificates, and DNS configurations. By leveraging Resmo's SQL query capabilities and change alerting, you can stay on top of important changes and ensure that your Gandi configurations are optimized for maximum security and efficiency.

| **Resources**              | **Key**                                                                       | **Supports Events** |
| -------------------------- | ----------------------------------------------------------------------------- | ------------------- |
| Certificate                | [gandi\_certificate](gandi\_certificate.md)                                   |                     |
| DNSSEC Key Detail          | [gandi\_dnssec\_key\_detail](gandi\_dnssec\_key\_detail.md)                   |                     |
| Domain                     | [gandi\_domain](gandi\_domain.md)                                             |                     |
| Domain Contact             | [gandi\_domain\_contact](gandi\_domain\_contact.md)                           |                     |
| Domain DNSSEC Key          | [gandi\_domain\_dnssec\_key](gandi\_domain\_dnssec\_key.md)                   |                     |
| Domain Glue Record         | [gandi\_domain\_glue\_record](gandi\_domain\_glue\_record.md)                 |                     |
| Domain LiveDNS Information | [gandi\_domain\_livedns\_information](gandi\_domain\_livedns\_information.md) |                     |
| Domain Record              | [gandi\_domain\_record](gandi\_domain\_record.md)                             |                     |
| Domain Renewal Information | [gandi\_domain\_renewal\_information](gandi\_domain\_renewal\_information.md) |                     |
| Domain Web Redirection     | [gandi\_domain\_webredir](gandi\_domain\_webredir.md)                         |                     |
| Organization               | [gandi\_organization](gandi\_organization.md)                                 |                     |
| User                       | [gandi\_user](gandi\_user.md)                                                 |                     |
