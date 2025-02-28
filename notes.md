# System Design

- It's about architecting scalable, reliable, and efficiency systems
- It handles: large-scale traffic to optimizing databases

## Main Concepts Overview

### 1. Scalability

- Vertical scaling (scaling up): Adding more resources to a single server (CPU, RAM)
- Horizontal scaling (scaling out): Adding more machines to handle load (distributed architecture)

### 2. Load balancing

- Distributes incoming traffic across multiple servers to ensure availaibility and reliability
- Techniques:
  - Round Robin: requests distributed sequentially
  - Least connections: routes to the server with fewer connections
  - Consistent hashing: ensures requests from the same client go to the same server

### 3. Database design

- SQL(Relational): Structured schema (MySQL, PostgresSQL)
- NoSQL(Non-relational): Flexible schema (MongoDB)
- Sharding: splitting a database into smaller pieces
- Replication: duplicating data across multiple servers for redundancy
- Indexing: improves query performance

### 4. Caching

- Stores frequently accessed data to reduce load on databases
- Techniques:
  - Client-side caching (e.g., browser caching)
  - CDN (Content delivery network): cached data closer to users
  - Application-level cache (e.g., Redis, Memcached)
  - Database cache: cached query results

### 5. Message queues and event-driven architecture

- Message queues: (RabbitMQ, Kafka, SQS): Async processing and decoupling services
- Pub/Sub model: Publishers send messages; subscribers process them

### 6. Microservices vs. Monoliths

- Monolithic architecture: one large application with all services together
- Microservices architecture: independent, loosely couple services communicating via APIs

### 7. Consistency & Availability (CAP Theorem)

- Consistency: All nodes see the same data at the same time
- Availability: system remains operational despite failures
- Partition tolerance: system continues working despite network failures
- Trade-offs: you can only choose 2 of the 3

### 8. CDN & Edge computing

- CDN (Content delivery network: Cloudflare, Akamai): Distributes static content to server closer to users
- Edge computing: Processing data near the user instead of a central server

### 9. Security and authentication

- OAuth2, JWT: Secure authentication mechanisms
- Rate limiting: prevents abuse (e.g., API throttling)
- Encryption: Data security in transit (TLS/SSL) and at rest

### 10. Observability & Monitoring

- Logging (ELK Stack, Datadog): tracks system activity
- Tracing (Jaeger, OpenTelemetry): understands request flow
- Metrics (Prometheus, Grafana): tracks performance

#### Summary

- Scalability: handling growth (vertical vs. horizontal)
- Loading balancing: distributing traffic
- Databases: SQL vs. NoSQL, sharding, replication
- Caching; storing frequently accessed data
- Messaging queues: async processing
- Microservices: decoupling services
- CAP Theorem: trade-offs in distributed systems
- Security: authentication & rate limiting
- Monitoring: logging, tracing, and metrics
