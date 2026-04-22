Cloud Native Networking Services

VPC - a logically isolated section of the AWS Cloud where you can launch AWS resources
- Choose a range of CIDR IPs: 10.0.0.0/16
Internet Gateway - enables access to the internet
Subnets - logical partitions of an IP network into smaller segments
Security Groups - firewalls at the instance level
- Implicitly deny all traffic, must create rules to allow em in
NACLs  (network access control lists) - Firewall at a subnet level 
- Not implicit, allow and deny rules

![[Screenshot 2026-04-07 at 10.33.03 AM.png]]


Enterprise-Hybrid
On premise + AWS

AWS VPN - secure connections between offices
DirectConnect - Very fast connection from on premise to AWS
Private Links - Keeps traffic within AWS network, no internet



