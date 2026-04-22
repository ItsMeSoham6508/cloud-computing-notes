VMs, resizable compute capacity

Choose OS -> choose instance type -> add EBS of EFS -> config, IAM, Key pairs


What are instance families? - different combinations of CPU Memory etc. 

General Purpose (balanced), Compute Optimized (ideal for compute bound aps that benefit from high performance processor), Memory Optimized (fast performance for workloads that process large data sets in memory), Accelerated optimized (hardware accelerators), Storage optimized (need fast read write speeds)

Just imagine what each of these would be good for


Instance Types - particular size and family

Nano, micro, etc.


### Pricing
- On Demand - low cost, flexible, per hour, **short term** workloads
	- Pay as you go
	- Default pricing model
- Spot (save 90%) - request spare computing capacity, need to be able to handle interruptions, consistent uptime is not an issue
	- AWS unused capacity
	- AWS batch is associated with this [[Compute]]
- Reserved (up to 75%) - Steady state predictable usage, long term savings
	- All upfront, Partial upfront, or No upfront, AURI, NURI, PURI
- Dedicated - Dedicated servers

#### AWS Savings plan
- Compute Savings Plan
	- Reduce costs by 66%
- EC2 instance savings plan
	- 72%
- Sagemaker savings plan

Zero-Trust model - security model based on trust no one and verify everything. [[Zero Trust]]


VM import/export