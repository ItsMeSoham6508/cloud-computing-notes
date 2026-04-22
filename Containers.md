What are microservices??

Monolithic architecture, one app which is responsible for everything

vs.

Microservice architecture - multiple apps are responsible for one thing each

Kubernetes - open source container orchestration system for automating deployment, scaling and management of containers.

**Primary Services**

- **ECS** – AWS's container orchestration service running on self-managed EC2. _Unmanaged_
- **AWS Fargate** – Serverless compute engine for containers with AWS-managed infrastructure. _Managed_
- **EKS** – Managed Kubernetes service that avoids vendor lock-in via open source. _Managed_
- **AWS Lambda** – Serverless, event-driven compute for short-running code or containers. _Fully Managed_

**Provisioning & Deployment**

- **Elastic Beanstalk** – PaaS that abstracts ECS setup for easier app deployment. _Managed_
- **App Runner** – Fully managed PaaS designed specifically for containerized apps. _Fully Managed_
- **AWS Copilot CLI** – CLI tool to build, release, and operate containerized apps on ECS/Fargate/App Runner. _Tool (not a service)_

**Supporting Services**

- **ECR** – Private Docker image registry for storing and managing container images. _Fully Managed_
- **X-Ray** – Distributed tracing service to analyze and debug microservices. _Fully Managed_
- **Step Functions** – Workflow orchestrator that stitches together Lambda and ECS tasks. _Fully Managed_

