OneDrive
========
Integrating your OneDrive account with Resmo offers valuable capabilities for managing and analyzing your organization's files and user data. OneDrive is a cloud storage and file-sharing platform provided by Microsoft. Resmo collects and utilizes various resources from the OneDrive API, enabling you to gain insights, enhance collaboration, and optimize file management processes.

Here are the key resources that Resmo collects from the OneDrive API:

User: Retrieve user information, including account details, contact information, organizational data, license details, manager information, authentication details, and more. This allows you to manage user accounts, track user activity, and analyze user-related data within your OneDrive environment.

Drive: Access drive-specific details, such as drive type, name, owner information, quota, sharing permissions, and SharePoint identifiers. This resource enables you to manage and monitor drives, enforce storage limits, and gain insights into drive usage and collaboration patterns.

Drive Item: Retrieve information about individual files and folders within a drive, including details such as name, creation/modification timestamps, file properties, permissions, and sharing status. This allows you to manage files, track file activities, and analyze file metadata to understand usage patterns and access control.

By leveraging Resmo's capabilities, you can perform various actions and gain insights from the collected OneDrive data:

Manage user accounts and permissions within OneDrive.
Track user activities and access patterns for auditing and security purposes.
Analyze file metadata and usage patterns to optimize file organization and access.
Monitor storage quotas and enforce storage limits for users or groups.
Track and manage file permissions and sharing settings to ensure data security and compliance.
Resmo's custom data integration allows you to define your own resource schemas and send data via webhooks, providing flexibility to integrate additional data sources or address specific file management and security concerns. With Resmo, you can effectively leverage the capabilities of OneDrive to enhance collaboration, streamline file management processes, and ensure the security and compliance of your organization's files and user data.

| **Resources** | **Key**                                           | **Supports Events** |
| ------------- | ------------------------------------------------- | ------------------- |
| Drive         | [onedrive\_drive](onedrive\_drive.md)             |                     |
| Drive Item    | [onedrive\_drive\_item](onedrive\_drive\_item.md) |                     |
| User          | [onedrive\_user](onedrive\_user.md)               | &check;             |
