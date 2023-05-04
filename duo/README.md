Duo
===
Integrating your Duo account with Resmo offers valuable insights into your organization's multi-factor authentication (MFA) and security configurations. Duo provides a robust MFA solution to protect your organization from unauthorized access, and by collecting and analyzing Duo configuration data, Resmo can help identify potential security risks, ensure adherence to best practices, and optimize configurations for efficiency and effectiveness.

Using Resmo's SQL query capabilities, users can ask complex questions about their Duo configuration data, such as:

* What are the account settings, such as fraud email configuration, helpdesk bypass settings, lockout thresholds, password requirements, and telephony limits?
* What are the details of users, including their aliases, email addresses, group memberships, enrollment status, and associated phones and tokens?
* What are the integration settings, such as admin API permissions, enroll policies, IP whitelists, and username normalization policies?
* What are the details of administrators, including their email addresses, roles, restrictions, and associated admin units?
* What are the phone configurations, such as capabilities, encryption status, fingerprints, phone numbers, and associated users?
* What are the group settings, such as MFA method enablement and group status?
* What are the details of MFA tokens and administrative units, including their restrictions, descriptions, and associated users or integrations?

Setting up change alerts in Resmo for your Duo account can also be beneficial for monitoring critical configuration changes, such as:

* Notifications when account settings change, such as lockout thresholds or password requirements.
* Alerts when new users are created, modified, or deleted, and when their enrollment status or group memberships change.
* Updates when integrations are created, modified, or deleted, and when their settings or policies change.
* Notifications when administrators are added, removed, or have their roles or restrictions changed.
* Alerts when phone configurations change or when phones are added or removed from users.
* Updates when groups, MFA tokens, or administrative units are created, modified, or deleted, and when their settings change.

In conclusion, integrating your Duo account with Resmo provides valuable insights into your organization's MFA and security configurations. By leveraging Resmo's SQL query capabilities and change alerting, you can stay on top of important changes and ensure that your Duo configurations are optimized for maximum efficiency and effectiveness.

| **Resources**       | **Key**                                                   | **Supports Events** |
| ------------------- | --------------------------------------------------------- | ------------------- |
| Account             | [duo\_account](duo\_account.md)                           |                     |
| Admin               | [duo\_admin](duo\_admin.md)                               |                     |
| Administrative Unit | [duo\_administrative\_unit](duo\_administrative\_unit.md) |                     |
| Group               | [duo\_group](duo\_group.md)                               |                     |
| Integration         | [duo\_integration](duo\_integration.md)                   |                     |
| MFA Token           | [duo\_mfa\_token](duo\_mfa\_token.md)                     |                     |
| Phone               | [duo\_phone](duo\_phone.md)                               |                     |
| User                | [duo\_user](duo\_user.md)                                 |                     |
