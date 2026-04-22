Application integration is the process of letting 2 independent apps to communicate and work with each other.

cloud workloads encourage systems and services to be loosely ***coupled*** and so AWS has many services for this

Common design patterns for integration include:
- Queueing - a waiting line for tasks
	- Messaging system - provide async communication and decouple processes via messages
	- A queueing system is a messaging system that deletes messages once they are consumed, not real time
- Streaming
	- Real time stuff, multiple consumers can react to events
- Pub/Sub - publish-subscribe pattern
	- Publishers do not send their messages directly to receivers
		- they send their messages to an **event bus** which categorizes their messages into groups.
		- messages are immediately pushed to subscribers
- API Gateways
	- API gateway is a program that sits between a single-entry point and multiple backends. 
- State Machine
	- Abstract model that decides how one state moves to another based on a series of conditions
	- FLOW CHART
- Event Bus
	- Receives events from a source and routes events to a target based on rules


**Simple Queueing Service (SQS)** - fully managed queueing service that enables you to decouple and scale microservices, long running tasks that are many in number like signup emails 

**Amazon kinesis** - full managed solution or collecting, processing, and analyzing streaming data in the cloud.

**Amazon Simple Notification Service** - fully managed service for pub sub

OrderService publishes → "order.placed" event
                              │
              ┌───────────────┼───────────────┐
              ▼               ▼               ▼
       EmailService    InventoryService   AnalyticsService
      (sends receipt)  (reserves stock)  (logs the sale)


**Amazon API Gateway** - solution for creating secure APIs in my cloud environment at any scale.

**AWS Step Functions** - Coordinate multiple aws services into a serverless workflow. Graphical conole to visualize the components of your app.

![[Screenshot 2026-04-08 at 11.03.42 AM.png]]

**AWS EventBridge** - serverless event bus service that is used for application integration by streaming real time data to your applications

**Amazon MQ** - is a managed message broker service that uses Apache MQ

**Managed kafka service (MSK)** - kafka is another real time streaming data pipeline builder.

**AppSync**  - fully managed graphQL service.



