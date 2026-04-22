AWS and the end user have different responsibilities 

Cloud security framework that define each group's security obligations

IN and OF

AWS is responsible for:
- Physical stuff: regions, AZs, edge locations, physical security
- Software: compute networking, etc.

Customer:
- Configuration of managed services: Platforms, Apps, IAM
- Config of virtual infra: OS, Network, Firewalls
- Security of data: Data Encryption, Server side encryption, customer data

## Changes based on service
EC2 (IaaS – most control)

- AWS → hardware, infrastructure
- You → OS, apps, data, configs

RDS / Lambda (PaaS)

- AWS → OS + platform
- You → data, access, configs

 S3 / DynamoDB (Managed services)

- AWS → almost everything infrastructure
- You → data, permissions, encryption
