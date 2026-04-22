Ec2 allows you to launch virtual machines

A VM is a emulation of a physical computer using software. Server virtualization allows you to easily create, copy, resize, migrate, server

AMI - Amazon machine image, predefined config for VM

Amazon Lightsail - Managed virtual server service, don't need much knowledge, batteries included

Containers - virtualizing OS to run multiple workloads on a single OS instance. 

- ECS - Elastic Container Service - container orchestration service that supports docker
- ECR - Elastic container registry - repository for container images. Need an image to launch container so store here.
- ECS Fargate - serverless orchestration, same as ECS, but pay on demand per running container because you don't handle EC2 server
- Elastic kubernetes service (EKS) - Kubernetes by google
- AWS Lambda - serverless functions service, just run the friggin code


Edge computing - push computing workloads outside of your networks to run close to the destination location


### Cost and Capacity Management
- EC2 Spot instances, reserved, and savings plan
- AWS Batch - plans, schedules, and executess, batch computing workloads, can use Spot instance
- AWS Compute Optimizer - Suggests to you how to reduce costs and improve perfomance
- Elastic Beanstalk - tool to easily deploy web apps, don't need to understand underlying AWS architecture