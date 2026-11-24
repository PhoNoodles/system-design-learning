# Curriculum

Primary source: [The System Design Primer](https://github.com/donnemartin/system-design-primer). Supplemental topics extend the primer for practical engineering. IDs define learning order, not GitHub issue numbers.

## 01 — Fundamentals

[Primer reference](https://github.com/donnemartin/system-design-primer#performance-vs-scalability)

- SD-01.01 — Performance vs scalability
- SD-01.02 — Latency vs throughput
- SD-01.03 — Vertical vs horizontal scaling
- SD-01.04 — Identifying bottlenecks
- SD-01.05 — CPU-bound vs I/O-bound workloads
- SD-01.06 — Availability vs reliability
- SD-01.07 — Capacity estimation and Little's Law
- SD-01.08 — Fundamentals assessment

## 02 — Distributed systems

[Primer reference](https://github.com/donnemartin/system-design-primer#availability-vs-consistency)

- SD-02.01 — CAP theorem
- SD-02.02 — Network partitions
- SD-02.03 — Weak consistency
- SD-02.04 — Eventual consistency
- SD-02.05 — Strong consistency
- SD-02.06 — Read-your-writes and session consistency
- SD-02.07 — Active-passive failover
- SD-02.08 — Active-active failover
- SD-02.09 — Leader-follower replication
- SD-02.10 — Multi-leader replication
- SD-02.11 — Quorums
- SD-02.12 — Availability calculations and SLOs
- SD-02.13 — Timeouts and retry safety
- SD-02.14 — Distributed systems assessment

## 03 — Networking

[Primer reference](https://github.com/donnemartin/system-design-primer#communication)

- SD-03.01 — OSI and TCP/IP models
- SD-03.02 — IP addressing and routing
- SD-03.03 — TCP vs UDP
- SD-03.04 — TCP connections and congestion
- SD-03.05 — DNS resolution and caching
- SD-03.06 — HTTP methods and status codes
- SD-03.07 — HTTP versions and connections
- SD-03.08 — TLS and HTTPS
- SD-03.09 — REST API design
- SD-03.10 — RPC and gRPC
- SD-03.11 — WebSockets and server-sent events
- SD-03.12 — Networking assessment

## 04 — Traffic management

[Primer reference](https://github.com/donnemartin/system-design-primer#load-balancer)

- SD-04.01 — Load balancer fundamentals
- SD-04.02 — Layer 4 vs Layer 7 balancing
- SD-04.03 — Round robin and least connections
- SD-04.04 — Health checks and failover
- SD-04.05 — Reverse proxy vs forward proxy
- SD-04.06 — Sticky sessions
- SD-04.07 — Autoscaling
- SD-04.08 — Rate limiting algorithms
- SD-04.09 — API gateways
- SD-04.10 — Traffic management assessment

## 05 — Application architecture

[Primer reference](https://github.com/donnemartin/system-design-primer#application-layer)

- SD-05.01 — Stateless vs stateful services
- SD-05.02 — Monolith vs microservices
- SD-05.03 — Service boundaries
- SD-05.04 — Service discovery
- SD-05.05 — Synchronous vs asynchronous communication
- SD-05.06 — Idempotency
- SD-05.07 — Circuit breakers
- SD-05.08 — Bulkheads and isolation
- SD-05.09 — Observability: logs metrics traces
- SD-05.10 — Configuration and feature flags
- SD-05.11 — Deployment strategies
- SD-05.12 — Application architecture assessment

## 06 — Databases

[Primer reference](https://github.com/donnemartin/system-design-primer#database)

- SD-06.01 — Relational database fundamentals
- SD-06.02 — ACID transactions
- SD-06.03 — Isolation levels and anomalies
- SD-06.04 — Indexes and query plans
- SD-06.05 — SQL tuning
- SD-06.06 — Connection pooling
- SD-06.07 — Leader-follower database replication
- SD-06.08 — Read replicas and replication lag
- SD-06.09 — Multi-leader database replication
- SD-06.10 — Federation and partitioning
- SD-06.11 — Sharding and shard keys
- SD-06.12 — Denormalization
- SD-06.13 — Key-value databases
- SD-06.14 — Document databases
- SD-06.15 — Wide-column and graph databases
- SD-06.16 — SQL vs NoSQL tradeoffs and assessment

## 07 — Caching

[Primer reference](https://github.com/donnemartin/system-design-primer#cache)

- SD-07.01 — Cache fundamentals and locality
- SD-07.02 — Client and browser caching
- SD-07.03 — CDN caching
- SD-07.04 — Application and database caching
- SD-07.05 — Cache-aside
- SD-07.06 — Read-through and write-through
- SD-07.07 — Write-back and write-around
- SD-07.08 — TTL and eviction policies
- SD-07.09 — Invalidation and cache stampedes
- SD-07.10 — Caching assessment

## 08 — Asynchronous processing

[Primer reference](https://github.com/donnemartin/system-design-primer#asynchronism)

- SD-08.01 — Message queues vs task queues
- SD-08.02 — Publish-subscribe and event streams
- SD-08.03 — Delivery guarantees
- SD-08.04 — Ordering and partition keys
- SD-08.05 — Consumer groups and workers
- SD-08.06 — Retries and dead-letter queues
- SD-08.07 — Idempotent consumers and deduplication
- SD-08.08 — Backpressure and flow control
- SD-08.09 — Transactional outbox and sagas
- SD-08.10 — Asynchronous processing assessment

## 09 — Security

[Primer reference](https://github.com/donnemartin/system-design-primer#security)

- SD-09.01 — Authentication vs authorization
- SD-09.02 — Sessions and cookies
- SD-09.03 — JWT and token lifecycle
- SD-09.04 — OAuth 2.0 and OpenID Connect
- SD-09.05 — RBAC and least privilege
- SD-09.06 — Encryption at rest and in transit
- SD-09.07 — Secrets management
- SD-09.08 — Input validation and injection prevention
- SD-09.09 — Threat modeling and tenant isolation
- SD-09.10 — Security assessment

## 10 — System design practice

[Primer reference](https://github.com/donnemartin/system-design-primer#how-to-approach-a-system-design-interview-question)

- SD-10.01 — Requirements and constraints
- SD-10.02 — Back-of-envelope calculations
- SD-10.03 — High-level design and API contracts
- SD-10.04 — Data modeling and core components
- SD-10.05 — Design URL shortener or Pastebin
- SD-10.06 — Design a social timeline
- SD-10.07 — Design a web crawler
- SD-10.08 — Design a key-value store
- SD-10.09 — Design SAP-to-MES manufacturing integration
- SD-10.10 — Full mock interview and tradeoff defense

## 11 — Advanced architecture

[Primer reference](https://github.com/donnemartin/system-design-primer#system-design-interview-questions-with-solutions)

- SD-11.01 — Push vs pull CDNs
- SD-11.02 — Object storage and distributed files
- SD-11.03 — Consistent hashing
- SD-11.04 — Distributed coordination and consensus
- SD-11.05 — Search indexes and indexing pipelines
- SD-11.06 — Disaster recovery RPO and RTO
- SD-11.07 — Design a sales ranking system
- SD-11.08 — Scale a system to millions of users on AWS

