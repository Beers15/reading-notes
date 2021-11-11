[Home](README.md)
 
# Readings: AWS: Events
 
## Review, Research, and Discussion
 
---------------

### Vocabulary terms

1) Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server

  * The Gateway service and ExpressJS can both be used for creating REST APis, with lambda being able to assist with the creation REST APIs. Lambda functions can be used for containerizing route handlers. All 3 let you perform CRUD operations.
  
2) List the AWS Database offerings and talk about the pros and cons of each (grouping together by type)

  * Amazon Aurora, Amazon RDS, Amazon Redshift
  
    Pros: Good for CRM and ecommerce apps 
    Cons: the number of connections and resources are limited, CPU and Storage performance is not guaranteed

  * Amazon DynamoDB

    Pros: Very fast, highly scalable  
    Cons: no foreign keys to refer to different tables, bad for complicated queries

  * Amazon MemoryDB for Redis, Amazon ElasticCache

    Pros: good for caching and geo-spatial apps
    Cons: High learning curve, expensive services

  * Amazon DocumentDB

    Pros: MongoDB capability, 
    Cons: lack of Atomicity, less secure than alternatives

  * Amazon Keyspaces

    Pros: No need to manage servers, has good performance at any scale
    Cons: Single region deployment, fixed cluster settings

  * Amazon Neptune

    Pros: Great for graph queries and graph applications in general, fast
    
    Cons: Good for its use cases, not so much for anything else

  * Amazon Timestream

    Pros: fast and cheap, serverless, has auto-scaling 
    
    Cons: Lackluster reporting of issues, poorly documented

  * Amazon Ledger Database Services

    Pros: Good for cryptographic use cases, such as financial apps. Has a "transparent, immutable, and cryptographically verifiable transaction log."
    Cons: Good for ledger database use cases, not so much for other cases

    https://aws.amazon.com/products/databases/

    Also referenced various posts on https://www.trustradius.com/products/

3) What’s the difference between a FIFO and a standard queue?

  * FIFO Queues only allow messages to be processed once and in order. This is not guaranteed in standard queues. The catch is that FIFO queues have much lower throughput.
  
    https://medium.com/awesome-cloud/aws-difference-between-sqs-standard-and-fifo-first-in-first-out-queues-28d1ea5e153

4) How can the server be assured a message was properly received?

  * Using a AWS SQS with a FIFO queue is one way to accomplish this.

### Document the following Vocabulary Terms

Serverless API

  * An API that breaks down its functionality into microservices. These services are hosted on containers instead of all existing on a monolithic server.

Triggers

  * Events that cause a lambda function to activate, when configured.

Dynamo vs Mongo

  * Both are NoSQL Dbs. Dynamo is only available on AWS. Both have document based storage. Mongo has a rich query language, while dynamo does not. Database behavior is transparent with Mongo. This is not the case for Dynamo.

Dynamoose vs Mongoose

  * Both are ORM libraries for their respective NoSQL DB.

    https://www.mongodb.com/compare/mongodb-dynamodb

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?
  
    * Publisher/subscriber design pattern, messaging queues, using AWS Lambdas

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    * How to use AWS SQS in applications to handle scalability

    * When to use  an AWS SQS vs an AWS SNS, or when to use both

    * Making Pub/Sub messaging applications

3) What are you most excited about trying to implement or see how it works?

    * Linking together all these AWS services that we have been using to create an API that uses serverless architecture
