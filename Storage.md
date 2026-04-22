Elastic Block Store (EBS) - Data is split into evenly split blocks, single write volume, accessed by OS, snapshots, encryption, elasticity

Elastic File Storage (EFS) - File is stored with data and metadata. Multiple connections via a network share (SHARE FILES BETWEEN SERVERS), multiple reads

Amazon Simple Storage Service (S3) - Object is stored with data, Scales unlimited, no lock in read and write


S3 - Intro
What is object storage: data storage architecture that manages data objects

- Unlimited storage

S3 Object - Objects contain your data, they are like files

Objects may contain: Key, Value, Version ID, Metadata

S3 Buckets hold objects and folders

**S3 Storage Classes** (Down cheaper)

S3 Default - 99.99 availability, 11 9's durable, 3 AZs
S3 Intelligent Tiering - ML to analyze objects usage and determine the appropriate class
S3 - Standard IA - Infrequent access
S3 One Zone IA - Only one AZ, cheaper than above
S3 Glacier - Long term cold storage
S3 Glacier Deep Archive - cheap af but 12 hr retrieval

#### **AWS Snow Family** - storage and compute devices used to physically move data in or out of the cloud
Snowcone, Snowball edge, snowmobile (100PB, literally a truck)

Storage Services
Storage Gateway - hybrid cloud storage service that extends to (sends your on prem shi to AWS)
- **File Gateway** → presents a *file* interface (NFS/SMB) with local caching
- **Volume Gateway** → *block* storage with cached or stored volumes
- **Tape Gateway** → virtual tape library for backups on-premises, cached file system

AWS Backup - fully managed backup service that makes it easy to automate the backup of data across multiple AWS services, you can create plans

Amazon FSx - highly performant file system


## Database

#### What is a warehouse
A relational datastore designed for analytic workloads. Designed to be HOT, fast query

Key-value store - a type of non-relational NoSQL

Document database - NoSQL database that stores documents, like JSON
--> DynamoDb, it is the flagship db

RDS
- MariaDB
- MySQL
- PostGres
- Oracle
- MS sql server
- Aurora - fully managed database of either mySql and PSQL
	- Aurora Serverless

Other db services
**Redshift** - a petabyte size data-warehouse, used for Online Analytical processing
**Elasticache** - managed db of in-memory and caching open source dbs Redis, adds a caching layer
**Neptune** - Managed graph db, data is represented as nodes
**Amazon Timestreams** - fully managed time series database. Measure how things change over time.
**Amazon quantum ledger db** - fully managed ledger db that provides transparent logs, history of financial transactions maybe
**Database migration service** (DMS) - obvious, change engines, on-premise to cloud


