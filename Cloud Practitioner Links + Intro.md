https://github.com/kananinirav/AWS-Certified-Cloud-Practitioner-Notes/blob/master/practice-exam/practice-exam-1.md

https://quizlet.com/392359849/aws-cloud-practitioner-exam-questions-flash-cards/?i=2u6uqa&x=1jqY

[[AWS-Certified-Cloud-Practitioner_Exam-Guide.pdf]] - Full list of services

https://youtu.be/NhDYbskXRgc?si=NXTHAvWX6NAirZyz&t=43610

**Dedicated servers - physical**
- Guess capacity and is very hard to provision and maintain

**Types of Cloud Computing:**
- Software as a service: product that is run and managed by the privder
- Platform as a service: focus on the dev of apps, basically beanstalk
- Infra as a service, building blocks for cloud IT, basically cloud providers

**Deployment Models**
- Public Cloud - everything is on the cloud, cloud first approach
	- startups
	- saas 
- Private - On-premise
	- public sector
	- hospitals
- Hybrid - both
	- Banks
	- fintech
- Cross cloud - using multiple providers

US-east-1 is the most central area, has all of the access

**Advantages**
- Metered billing/variable expense.
- Massive economies of scales
- Scale on demand, no guess capacity
- Increase speed, one click away
- Focus on infra, don't maintain data centers
- Go global in minutes, AWS regions
- Pay as you go
- Fault tolerance
- Elastic - automated scaling

# AWS GLOBAL INFRA - globally distributed hardware
- Regions
	- Geographically distinct locations consisting of 1/more AZs, generally 3
	- Some AWS services operate across regions like s3, cloudfront, Route53, and are GLOBAL
- Availability zones
	- Physical location made up of one or more data centers
	- Common to run workloads in 3 AZs

![[Screenshot 2026-04-04 at 5.21.08 PM.png]]

Subnet - is associated with an AZ, every region has a default VPC


##### MULTI AZ -> HIGH AVAILABILITY
**Fault Tolerance** 
- Fault domains are sections of a network vulnerable to damage is a critical system fails. The idea is to isolate damage, a fault level is a collection of domains
- -> EACH AWS REGION is isolated from the others
	- AZs are their own failure zones

**Edge Locations** - on and off ramps to the AWS global network, accelerators, cdns, **CACHED**
Point of Presence is a middleman 

Cloudfront - CDN

S3 Transfer Acceleration - I can generate a special url that end users can use to upload files to edge locations

Global accelerator - finds the optimal path for my end users to web-servers, can send to edge locations

AWS direct connect - private dedication connection between datacenter or office [[Networking]]

Local zones - datacenters in densely populated areas for 1-digit ms transactions

Wavelength zones - 5G low latency applications

Outposts - physical server racks that you get from AWS that connect via voodoo magic

**Data residency**
- geographical locations of wherr resources reside
- Compliance boundaries describe where resources are allowed to reside
- Data Sovereignty is jurisdictional control that can be asserted over data
- AWS CONFIG - rules to check expectations and alerts you if they deviate
	- Service control policies are within orgs

