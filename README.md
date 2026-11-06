# Azure Active Directory Practice

Learning how to manage user accounts, groups, and security settings in the cloud version of Active Directory (Azure AD / Microsoft Entra ID).

## Azure AD Notes

Azure provides administrative access to manage my tenant. Within the tenant, I can manage users, groups, and devices.

Microsoft manages the underlying cloud infrastructure that stores and protects tenant data. Objects within Azure AD contain attributes such as first name, last name, email address, and other identifying information.

Microsoft uses data replication and redundancy across its infrastructure to help protect information and maintain service availability in the event of a failure.

## Azure AD User Accounts

*Creating and managing users*

### Admin Roles

- The Zero Trust approach helps ensure that administrators receive only the roles and permissions they need to perform their specific responsibilities.
- Limiting administrative access helps reduce unnecessary permissions and improves security.
- Administrative roles do not automatically require a license, although access to certain Microsoft services and features may require one.

### Assigning Licenses to Users

Assigning licenses to users gives them access to Microsoft 365 workflows and other paid Microsoft services, depending on the license assigned.

### Deleting and Restoring Users

Deleting accounts is useful when employees leave an organization and no longer need access.

If an account is accidentally deleted, it can be restored by navigating to the **Deleted Users** section and selecting the restore option.

Deleted user accounts can generally be restored within 30 days. After that period, they are permanently deleted.

### Password Reset

Password resets can be performed by navigating to the affected user's account. From the **Overview** page, select **Reset Password**.

Azure generates a temporary password that can be provided to the user so they can regain access to their account.

Administrators can also enable Self-Service Password Reset (SSPR), allowing users to reset their own passwords using configured authentication methods.

## Administrating Groups

- When creating a group, the first step is choosing between a **Security Group** and a **Microsoft 365 Group**.
- Security groups are primarily used to manage permissions and control access to resources.
- Microsoft 365 groups are designed for collaboration and provide access to shared Microsoft 365 resources.
- Groups can be used to organize users by department or job responsibility.
- A group can have an assigned owner who is responsible for managing the group and inviting or adding members.

### Dynamic Membership Rules

Security groups can use dynamic membership rules to automatically add or remove users based on their account properties.

For example, users can be added to a department group based on a specific property, such as their department name.

If a user's properties change and they no longer meet the membership requirements, they are automatically removed from the group.

## Azure AD Security

### Security Defaults

Security Defaults are a useful way to improve the security of an Azure AD tenant.

They provide basic security protections, such as requiring multifactor authentication (MFA) for certain accounts and blocking legacy authentication.

Security Defaults are generally useful for new tenants that do not already have custom security policies configured. They may not be appropriate for organizations that already use more advanced security policies or Conditional Access.
