# System Design

- It's about architecting scalable, reliable, and efficiency systems
- It handles: large-scale traffic to optimizing databases

## Main Concepts Overview

### 1. Scalability

- Vertical scaling (scaling up): Adding more resources to a single server (CPU, RAM)
- Horizontal scaling (scaling out): Adding more machines to handle load (distributed architecture)

### 2. Load balancing

- Distributes incoming traffic across multiple servers to ensure availaibility and reliability
- Techniques
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

### 5. Message queues and event-driven architecture

### 6. Microservices vs. Monoliths

### 7. Consistency & Availability

### 8. CDN & Edge computing

### 9. Security and authentication

### 10. Observability & Monitoring

#### Summary
