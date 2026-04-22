**High scalability** - my ability to increase your capacity based on increasing demand of traffic

Elastic load balancers

Vertical scaling - bigger servers
Horizontal scaling - more servers 

**High Elasticity** - Automatically increase and decrease capacity, AWS Auto scaling


## **High Durability** - Disaster recovery

Cloud Endure Disaster Recovery - continuously replicates machines into low cost areas in case of failure

Business Continuity Plans (BCP) - a document that outlines how a business will continue to operate during unplanned disruptions

- Recovery point objective - max amount of data loss acceptable expressed as time
- Recovery time objective - how much downtime till a significant loss is incurred

![[Screenshot 2026-04-05 at 12.02.23 PM.png]]


Options for disaster recovery

![[Screenshot 2026-04-05 at 12.04.48 PM.png]]


#### AWS APIs
API - application programming interface, softwares that allows two apps to talk to each other
-> Most common is HTTP

- DEVELOPER TOOLS, no one uses http calls to aws
	- Management Console - ClickOps
	- SDK - use it in a programming language
	- CLI - command line interface
		- Powershell for windows, CAN USE ***CLOUDSHELL*** on mac
	- Infrastructure as Code (IaC) is the practice of managing and provisioning computing infrastructure through machine-readable definition files (Config files)


AWS Account ID: 12 digits with a non-root user account

CloudShell - a cli in the web

Amazon resource names - Uniquely identify AWS resources

IaC
- AWS CloudFormation (CFN) - explicit, uses scripting languages JSON, YAML
	- Can lead to large files
- AWS CDK - Cloud Development Kit, implicit, uses programming languages

Access Key - a key and secret needed to have programmatic access to AWS resources when interacting with the API out of the Console