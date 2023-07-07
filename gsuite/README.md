Google Workspace
================
Google Workspace (formerly known as G Suite) is a suite of cloud computing, productivity, and collaboration tools, software, and products developed and marketed by Google. Resmo can connect to a Google Workspace account to collect configuration data from various resources, including user accounts, groups, mobile devices, and calendars. Resmo can help users monitor the configuration of their Google Workspace resources, detect security issues, and ensure best practices are followed.

With Resmo's SQL queries, users can ask complex questions about their Google Workspace configuration data. For example:

* Which users have not logged into their Google Workspace account in the last 30 days?
* Which groups have external members with access to sensitive information?
* Which devices have not received a security update in the last 60 days?
* Which resources are being shared with users outside of the organization?
* Which users have been granted administrative privileges?

Users can also set alarms to receive notifications when critical changes occur in their Google Workspace resources. For example:

* Receive an alert when a new user is added to the domain.
* Receive an alert when a user's account is accessed from a new device.
* Receive an alert when a group's membership changes.
* Receive an alert when a device is wiped remotely.
* Receive an alert when a user's password is changed by an administrator.

| **Resources**                 | **Key**                                                                     | **Supports Events** |
| ----------------------------- | --------------------------------------------------------------------------- | ------------------- |
| Delegate                      | [gmail\_delegate](gmail\_delegate.md)                                       |                     |
| Filter                        | [gmail\_filter](gmail\_filter.md)                                           |                     |
| Forwarding Address            | [gmail\_forwarding\_address](gmail\_forwarding\_address.md)                 |                     |
| Application Specific Password | [gsuite\_asp](gsuite\_asp.md)                                               |                     |
| Browser Enrollment Token      | [gsuite\_browser\_enrollment\_token](gsuite\_browser\_enrollment\_token.md) |                     |
| Chrome Browser                | [gsuite\_chrome\_browser](gsuite\_chrome\_browser.md)                       |                     |
| Customer                      | [gsuite\_customer](gsuite\_customer.md)                                     |                     |
| Domain                        | [gsuite\_domain](gsuite\_domain.md)                                         | &check;             |
| Group                         | [gsuite\_group](gsuite\_group.md)                                           | &check;             |
| Group Member                  | [gsuite\_group\_member](gsuite\_group\_member.md)                           | &check;             |
| Group Settings                | [gsuite\_group\_settings](gsuite\_group\_settings.md)                       | &check;             |
| Mobile Device                 | [gsuite\_mobile\_device](gsuite\_mobile\_device.md)                         | &check;             |
| Organizational Unit           | [gsuite\_org\_unit](gsuite\_org\_unit.md)                                   |                     |
| Privilege                     | [gsuite\_privilege](gsuite\_privilege.md)                                   |                     |
| Building                      | [gsuite\_resource\_building](gsuite\_resource\_building.md)                 | &check;             |
| Calendar                      | [gsuite\_resource\_calendar](gsuite\_resource\_calendar.md)                 | &check;             |
| Role                          | [gsuite\_role](gsuite\_role.md)                                             | &check;             |
| Role Assignment               | [gsuite\_role\_assignment](gsuite\_role\_assignment.md)                     | &check;             |
| Token                         | [gsuite\_token](gsuite\_token.md)                                           |                     |
| User                          | [gsuite\_user](gsuite\_user.md)                                             | &check;             |
