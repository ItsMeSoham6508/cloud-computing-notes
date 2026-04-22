IAM - Identity Access Management
- Set policies
- permission boundaries
- SCP - service control policies - org wide policies
- Conditions
	- time
	- sourceIp
	- Requested Region
	- MFA


Amazon lowk not that good at Zero trust - need to use diff services
AWS Cloudtrail - Tracks API Calls - who is fucking around in the org
AWS GuardDuty - Detects suspicious or malicious activity based on cloudtrail
AWS Detective - Used to analyze security issues from GuardDuty

AWS SSO - Log in once and access multiple AWS accounts and apps without re-entering credentials, one identity that can be used for ton of things
- Manage access centrally across your AWS organization


Directory Service - maps the name of network resources to their network addresses. Shared infra for locating, managing resources, like DNS


![[Screenshot 2026-04-07 at 11.16.35 AM.png]]


Principle of least privilege: You should grant your users only the permissions they need when they need them and nothing more.

IAM roles deal with resources

AWS Account root user
- AWS account holds all of your resources
	- Root user, special account with full access that cannot be deleted
		- Tasks that should only be done with root user
			- **Change account settings**
			- Restore IAM user permissions
			- Activate IAM access to billing and management console
			- **Close AWS account**
			- **Change AWS support plan**
		- only way to limit root users is through SCPs
	- User, common tasks with permissions