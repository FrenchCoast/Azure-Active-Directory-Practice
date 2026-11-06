# Azure-Active-Directory-Practice
Learning how to manage accounts and group policies in a cloud version of Active Directory (IAAS Solution)

Azure AD Notes
Azure helps by giving me the admin access to managing my tenant, within that there's my user's, groups and devices. 
Microsoft is responsible for backing up my tenant and storing the data. Objects have attributes such as First Name, Last Name, Email, etc. 
Data is kept inside a primary data center and ultimately replicated over and over again to other data centers as read-only's to 
prevent the lose of data or failure. 

Azure AD User Accounts
(Creating and managing users)
- Admin Roles
Use Zero trust to give admins the correct roles they need. This limits the scope of access needed for their specified role. 
Admins do not need licensing so even guest accounts can technically be admins.
- Assigning License to a user)
Assigning licensing to users give them access to Microsoft 365 workflows and other various paid services.
- Deleting and restoring users
Deleting accounts is useful for users who leave the company.
If accidental deletion happens go to the deleted users tab and click on restore user. The deleted user's data is saved
for 30 days, then the data is permanently deleted.
-Password Reset
Password resets are done by navigating to the troubled user's account. Then on the top of overview, click on the reset password. A temporary password will be populated and I will give them the password. I'm able to also provide them with an option to do a self-service password reset by giving them different authentication methods for user to do their own password reset. 

Administrating Groups
-First step of the creation process is choosing between a security groups or a Microsoft 365 group. Security group is used for permissions and 365 is used as a fully collaborative group. Used to differentiate departments. Group usually get an owner in the group who's able invite members into the group. 
-In security groups there's dynamic membership rules. These rules are used to dynamically add users into the group based
on their properties. If any of these proerties change they will automatically leave the group. 

Azure AD Security
- Security defaults is a great to secure the tenant in Azure. Usually not turned on if there are already pre existing conditions 
or policers set up. Though it is a good line of defense if the tenant is new and no official security measures are set up.
-Authentication methods 
