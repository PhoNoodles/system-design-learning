# Curriculum

Primary source: [The System Design Primer by Donne Martin](https://github.com/donnemartin/system-design-primer). See [SOURCE_MAP.md](SOURCE_MAP.md) for a source-section-by-section comparison and [LEARNING_PROTOCOL.md](LEARNING_PROTOCOL.md) for assessment and resume rules.

## How to use this index

This is the canonical plan: **148 unique lessons — 123 on the main path and 25 optional**. The two administrative duplicates (#19 and #20) are excluded. The tables contain no manually maintained completion status; read the linked issue and session comments for actual progress.

Follow the row order below, respecting prerequisites and the latest learning session. Stable lesson IDs identify topics; GitHub issue numbers identify records. Row order deliberately puts SD-07.11 before SD-07.10 and SD-10.11/SD-10.12 before SD-10.10. Existing IDs were preserved when gaps were added. Optional sections 12–14 never block the main path.

A prerequisite can be satisfied by recorded independent evidence or a short diagnostic. Reuse evidence rather than reteaching a mastered concept. An explicit learner choice may change the sequence; record that choice and the next step.

**Source key:** Primer = directly discussed or worked upstream; Primer + extension = source material plus added depth; Supplemental = added course topic; Assessment = course-created section check; Primer prompt = named upstream practice question whose detailed teaching needs supplemental primary sources; Reference activity = selected bibliography reading; Upstream placeholder = source names the exercise without a solution. Source coverage is separate from mastery.

## Sections

| Section | Track | Lessons |
| --- | --- | ---: |
| 01 — Fundamentals | Main | 8 |
| 02 — Distributed systems | Main | 14 |
| 03 — Networking | Main | 12 |
| 04 — Traffic management | Main | 10 |
| 05 — Application architecture | Main | 12 |
| 06 — Databases | Main | 16 |
| 07 — Caching | Main | 11 |
| 08 — Asynchronous processing | Main | 10 |
| 09 — Security | Main | 10 |
| 10 — System design practice | Main | 12 |
| 11 — Advanced architecture | Main | 8 |
| 12 — Optional object-oriented design | Optional | 7 |
| 13 — Optional system-design practice bank | Optional | 16 |
| 14 — Optional architecture reading | Optional | 2 |

## 01 — Fundamentals

| Lesson and canonical issue | Source coverage | Prerequisites |
| --- | --- | --- |
| [SD-01.01 — Performance vs scalability](https://github.com/PhoNoodles/system-design-learning/issues/1) (#1) | Primer | None |
| [SD-01.02 — Latency vs throughput](https://github.com/PhoNoodles/system-design-learning/issues/2) (#2) | Primer + extension | [SD-01.01](https://github.com/PhoNoodles/system-design-learning/issues/1) |
| [SD-01.03 — Vertical vs horizontal scaling](https://github.com/PhoNoodles/system-design-learning/issues/3) (#3) | Primer | [SD-01.01](https://github.com/PhoNoodles/system-design-learning/issues/1) |
| [SD-01.04 — Identifying bottlenecks](https://github.com/PhoNoodles/system-design-learning/issues/4) (#4) | Primer | [SD-01.02](https://github.com/PhoNoodles/system-design-learning/issues/2), [SD-01.03](https://github.com/PhoNoodles/system-design-learning/issues/3) |
| [SD-01.05 — CPU-bound vs I/O-bound workloads](https://github.com/PhoNoodles/system-design-learning/issues/5) (#5) | Supplemental | [SD-01.02](https://github.com/PhoNoodles/system-design-learning/issues/2), [SD-01.04](https://github.com/PhoNoodles/system-design-learning/issues/4) |
| [SD-01.06 — Availability vs reliability](https://github.com/PhoNoodles/system-design-learning/issues/6) (#6) | Primer + extension | [SD-01.01](https://github.com/PhoNoodles/system-design-learning/issues/1) |
| [SD-01.07 — Capacity estimation and Little's Law](https://github.com/PhoNoodles/system-design-learning/issues/7) (#7) | Primer + extension | [SD-01.02](https://github.com/PhoNoodles/system-design-learning/issues/2), [SD-01.04](https://github.com/PhoNoodles/system-design-learning/issues/4) |
| [SD-01.08 — Fundamentals assessment](https://github.com/PhoNoodles/system-design-learning/issues/8) (#8) | Assessment | [SD-01.05](https://github.com/PhoNoodles/system-design-learning/issues/5), [SD-01.06](https://github.com/PhoNoodles/system-design-learning/issues/6), [SD-01.07](https://github.com/PhoNoodles/system-design-learning/issues/7) |

## 02 — Distributed systems

| Lesson and canonical issue | Source coverage | Prerequisites |
| --- | --- | --- |
| [SD-02.01 — CAP theorem](https://github.com/PhoNoodles/system-design-learning/issues/9) (#9) | Primer | [SD-01.06](https://github.com/PhoNoodles/system-design-learning/issues/6) |
| [SD-02.02 — Network partitions](https://github.com/PhoNoodles/system-design-learning/issues/10) (#10) | Primer | [SD-02.01](https://github.com/PhoNoodles/system-design-learning/issues/9) |
| [SD-02.03 — Weak consistency](https://github.com/PhoNoodles/system-design-learning/issues/11) (#11) | Primer | [SD-02.02](https://github.com/PhoNoodles/system-design-learning/issues/10) |
| [SD-02.04 — Eventual consistency](https://github.com/PhoNoodles/system-design-learning/issues/12) (#12) | Primer | [SD-02.03](https://github.com/PhoNoodles/system-design-learning/issues/11) |
| [SD-02.05 — Strong consistency](https://github.com/PhoNoodles/system-design-learning/issues/13) (#13) | Primer | [SD-02.04](https://github.com/PhoNoodles/system-design-learning/issues/12) |
| [SD-02.06 — Read-your-writes and session consistency](https://github.com/PhoNoodles/system-design-learning/issues/14) (#14) | Supplemental | [SD-02.04](https://github.com/PhoNoodles/system-design-learning/issues/12), [SD-02.05](https://github.com/PhoNoodles/system-design-learning/issues/13) |
| [SD-02.07 — Active-passive failover](https://github.com/PhoNoodles/system-design-learning/issues/15) (#15) | Primer + extension | [SD-02.02](https://github.com/PhoNoodles/system-design-learning/issues/10), [SD-02.04](https://github.com/PhoNoodles/system-design-learning/issues/12) |
| [SD-02.08 — Active-active failover](https://github.com/PhoNoodles/system-design-learning/issues/16) (#16) | Primer | [SD-02.07](https://github.com/PhoNoodles/system-design-learning/issues/15) |
| [SD-02.09 — Leader-follower replication](https://github.com/PhoNoodles/system-design-learning/issues/17) (#17) | Primer | [SD-02.04](https://github.com/PhoNoodles/system-design-learning/issues/12), [SD-02.07](https://github.com/PhoNoodles/system-design-learning/issues/15) |
| [SD-02.10 — Multi-leader replication](https://github.com/PhoNoodles/system-design-learning/issues/18) (#18) | Primer | [SD-02.09](https://github.com/PhoNoodles/system-design-learning/issues/17), [SD-02.02](https://github.com/PhoNoodles/system-design-learning/issues/10) |
| [SD-02.11 — Quorums](https://github.com/PhoNoodles/system-design-learning/issues/21) (#21) | Supplemental | [SD-02.09](https://github.com/PhoNoodles/system-design-learning/issues/17), [SD-02.10](https://github.com/PhoNoodles/system-design-learning/issues/18) |
| [SD-02.12 — Availability calculations and SLOs](https://github.com/PhoNoodles/system-design-learning/issues/22) (#22) | Primer + extension | [SD-01.06](https://github.com/PhoNoodles/system-design-learning/issues/6), [SD-02.07](https://github.com/PhoNoodles/system-design-learning/issues/15), [SD-02.08](https://github.com/PhoNoodles/system-design-learning/issues/16) |
| [SD-02.13 — Timeouts and retry safety](https://github.com/PhoNoodles/system-design-learning/issues/23) (#23) | Supplemental | [SD-02.02](https://github.com/PhoNoodles/system-design-learning/issues/10), [SD-02.09](https://github.com/PhoNoodles/system-design-learning/issues/17) |
| [SD-02.14 — Distributed systems assessment](https://github.com/PhoNoodles/system-design-learning/issues/24) (#24) | Assessment | [SD-02.11](https://github.com/PhoNoodles/system-design-learning/issues/21), [SD-02.12](https://github.com/PhoNoodles/system-design-learning/issues/22), [SD-02.13](https://github.com/PhoNoodles/system-design-learning/issues/23) |

## 03 — Networking

| Lesson and canonical issue | Source coverage | Prerequisites |
| --- | --- | --- |
| [SD-03.01 — OSI and TCP/IP models](https://github.com/PhoNoodles/system-design-learning/issues/25) (#25) | Primer + extension | [SD-01.02](https://github.com/PhoNoodles/system-design-learning/issues/2) |
| [SD-03.02 — IP addressing and routing](https://github.com/PhoNoodles/system-design-learning/issues/26) (#26) | Supplemental | [SD-03.01](https://github.com/PhoNoodles/system-design-learning/issues/25) |
| [SD-03.03 — TCP vs UDP](https://github.com/PhoNoodles/system-design-learning/issues/27) (#27) | Primer | [SD-03.02](https://github.com/PhoNoodles/system-design-learning/issues/26) |
| [SD-03.04 — TCP connections and congestion](https://github.com/PhoNoodles/system-design-learning/issues/28) (#28) | Primer | [SD-03.03](https://github.com/PhoNoodles/system-design-learning/issues/27) |
| [SD-03.05 — DNS resolution and caching](https://github.com/PhoNoodles/system-design-learning/issues/29) (#29) | Primer + extension | [SD-03.02](https://github.com/PhoNoodles/system-design-learning/issues/26) |
| [SD-03.06 — HTTP methods and status codes](https://github.com/PhoNoodles/system-design-learning/issues/30) (#30) | Primer + extension | [SD-03.04](https://github.com/PhoNoodles/system-design-learning/issues/28), [SD-03.05](https://github.com/PhoNoodles/system-design-learning/issues/29) |
| [SD-03.07 — HTTP versions and connections](https://github.com/PhoNoodles/system-design-learning/issues/31) (#31) | Supplemental | [SD-03.04](https://github.com/PhoNoodles/system-design-learning/issues/28), [SD-03.06](https://github.com/PhoNoodles/system-design-learning/issues/30) |
| [SD-03.08 — TLS and HTTPS](https://github.com/PhoNoodles/system-design-learning/issues/32) (#32) | Supplemental | [SD-03.04](https://github.com/PhoNoodles/system-design-learning/issues/28), [SD-03.06](https://github.com/PhoNoodles/system-design-learning/issues/30) |
| [SD-03.09 — REST API design](https://github.com/PhoNoodles/system-design-learning/issues/33) (#33) | Primer | [SD-03.06](https://github.com/PhoNoodles/system-design-learning/issues/30) |
| [SD-03.10 — RPC and gRPC](https://github.com/PhoNoodles/system-design-learning/issues/34) (#34) | Primer + extension | [SD-03.09](https://github.com/PhoNoodles/system-design-learning/issues/33), [SD-02.13](https://github.com/PhoNoodles/system-design-learning/issues/23) |
| [SD-03.11 — WebSockets and server-sent events](https://github.com/PhoNoodles/system-design-learning/issues/35) (#35) | Supplemental | [SD-03.06](https://github.com/PhoNoodles/system-design-learning/issues/30), [SD-03.07](https://github.com/PhoNoodles/system-design-learning/issues/31) |
| [SD-03.12 — Networking assessment](https://github.com/PhoNoodles/system-design-learning/issues/36) (#36) | Assessment | [SD-03.08](https://github.com/PhoNoodles/system-design-learning/issues/32), [SD-03.10](https://github.com/PhoNoodles/system-design-learning/issues/34), [SD-03.11](https://github.com/PhoNoodles/system-design-learning/issues/35) |

## 04 — Traffic management

| Lesson and canonical issue | Source coverage | Prerequisites |
| --- | --- | --- |
| [SD-04.01 — Load balancer fundamentals](https://github.com/PhoNoodles/system-design-learning/issues/37) (#37) | Primer | [SD-01.03](https://github.com/PhoNoodles/system-design-learning/issues/3), [SD-03.03](https://github.com/PhoNoodles/system-design-learning/issues/27) |
| [SD-04.02 — Layer 4 vs Layer 7 balancing](https://github.com/PhoNoodles/system-design-learning/issues/38) (#38) | Primer | [SD-04.01](https://github.com/PhoNoodles/system-design-learning/issues/37), [SD-03.06](https://github.com/PhoNoodles/system-design-learning/issues/30), [SD-03.08](https://github.com/PhoNoodles/system-design-learning/issues/32) |
| [SD-04.03 — Round robin and least connections](https://github.com/PhoNoodles/system-design-learning/issues/39) (#39) | Primer + extension | [SD-04.01](https://github.com/PhoNoodles/system-design-learning/issues/37) |
| [SD-04.04 — Health checks and failover](https://github.com/PhoNoodles/system-design-learning/issues/40) (#40) | Primer + extension | [SD-04.01](https://github.com/PhoNoodles/system-design-learning/issues/37), [SD-02.07](https://github.com/PhoNoodles/system-design-learning/issues/15) |
| [SD-04.05 — Reverse proxies, forward proxies and load balancers](https://github.com/PhoNoodles/system-design-learning/issues/41) (#41) | Primer + extension | [SD-04.02](https://github.com/PhoNoodles/system-design-learning/issues/38) |
| [SD-04.06 — Sticky sessions](https://github.com/PhoNoodles/system-design-learning/issues/42) (#42) | Primer | [SD-04.03](https://github.com/PhoNoodles/system-design-learning/issues/39), [SD-04.04](https://github.com/PhoNoodles/system-design-learning/issues/40) |
| [SD-04.07 — Autoscaling](https://github.com/PhoNoodles/system-design-learning/issues/43) (#43) | Supplemental | [SD-04.03](https://github.com/PhoNoodles/system-design-learning/issues/39), [SD-04.04](https://github.com/PhoNoodles/system-design-learning/issues/40), [SD-01.07](https://github.com/PhoNoodles/system-design-learning/issues/7) |
| [SD-04.08 — Rate limiting algorithms](https://github.com/PhoNoodles/system-design-learning/issues/44) (#44) | Primer + extension | [SD-03.06](https://github.com/PhoNoodles/system-design-learning/issues/30), [SD-04.01](https://github.com/PhoNoodles/system-design-learning/issues/37) |
| [SD-04.09 — API gateways](https://github.com/PhoNoodles/system-design-learning/issues/45) (#45) | Supplemental | [SD-04.05](https://github.com/PhoNoodles/system-design-learning/issues/41), [SD-04.08](https://github.com/PhoNoodles/system-design-learning/issues/44) |
| [SD-04.10 — Traffic management assessment](https://github.com/PhoNoodles/system-design-learning/issues/46) (#46) | Assessment | [SD-04.06](https://github.com/PhoNoodles/system-design-learning/issues/42), [SD-04.07](https://github.com/PhoNoodles/system-design-learning/issues/43), [SD-04.09](https://github.com/PhoNoodles/system-design-learning/issues/45) |

## 05 — Application architecture

| Lesson and canonical issue | Source coverage | Prerequisites |
| --- | --- | --- |
| [SD-05.01 — Stateless vs stateful services](https://github.com/PhoNoodles/system-design-learning/issues/47) (#47) | Primer | [SD-04.06](https://github.com/PhoNoodles/system-design-learning/issues/42) |
| [SD-05.02 — Monolith vs microservices](https://github.com/PhoNoodles/system-design-learning/issues/48) (#48) | Primer | [SD-05.01](https://github.com/PhoNoodles/system-design-learning/issues/47) |
| [SD-05.03 — Service boundaries](https://github.com/PhoNoodles/system-design-learning/issues/49) (#49) | Primer + extension | [SD-05.02](https://github.com/PhoNoodles/system-design-learning/issues/48) |
| [SD-05.04 — Service discovery](https://github.com/PhoNoodles/system-design-learning/issues/50) (#50) | Primer | [SD-05.03](https://github.com/PhoNoodles/system-design-learning/issues/49), [SD-04.04](https://github.com/PhoNoodles/system-design-learning/issues/40) |
| [SD-05.05 — Synchronous vs asynchronous communication](https://github.com/PhoNoodles/system-design-learning/issues/51) (#51) | Primer | [SD-05.03](https://github.com/PhoNoodles/system-design-learning/issues/49), [SD-03.10](https://github.com/PhoNoodles/system-design-learning/issues/34) |
| [SD-05.06 — Idempotency](https://github.com/PhoNoodles/system-design-learning/issues/52) (#52) | Primer + extension | [SD-02.13](https://github.com/PhoNoodles/system-design-learning/issues/23), [SD-03.06](https://github.com/PhoNoodles/system-design-learning/issues/30) |
| [SD-05.07 — Circuit breakers](https://github.com/PhoNoodles/system-design-learning/issues/53) (#53) | Supplemental | [SD-02.13](https://github.com/PhoNoodles/system-design-learning/issues/23), [SD-05.05](https://github.com/PhoNoodles/system-design-learning/issues/51) |
| [SD-05.08 — Bulkheads and isolation](https://github.com/PhoNoodles/system-design-learning/issues/54) (#54) | Supplemental | [SD-05.03](https://github.com/PhoNoodles/system-design-learning/issues/49), [SD-05.07](https://github.com/PhoNoodles/system-design-learning/issues/53) |
| [SD-05.09 — Observability: logs metrics traces](https://github.com/PhoNoodles/system-design-learning/issues/55) (#55) | Supplemental | [SD-01.04](https://github.com/PhoNoodles/system-design-learning/issues/4), [SD-05.04](https://github.com/PhoNoodles/system-design-learning/issues/50), [SD-05.05](https://github.com/PhoNoodles/system-design-learning/issues/51) |
| [SD-05.10 — Configuration and feature flags](https://github.com/PhoNoodles/system-design-learning/issues/56) (#56) | Supplemental | [SD-05.03](https://github.com/PhoNoodles/system-design-learning/issues/49), [SD-05.09](https://github.com/PhoNoodles/system-design-learning/issues/55) |
| [SD-05.11 — Deployment strategies](https://github.com/PhoNoodles/system-design-learning/issues/57) (#57) | Supplemental | [SD-05.01](https://github.com/PhoNoodles/system-design-learning/issues/47), [SD-05.09](https://github.com/PhoNoodles/system-design-learning/issues/55), [SD-05.10](https://github.com/PhoNoodles/system-design-learning/issues/56) |
| [SD-05.12 — Application architecture assessment](https://github.com/PhoNoodles/system-design-learning/issues/58) (#58) | Assessment | [SD-05.06](https://github.com/PhoNoodles/system-design-learning/issues/52), [SD-05.08](https://github.com/PhoNoodles/system-design-learning/issues/54), [SD-05.11](https://github.com/PhoNoodles/system-design-learning/issues/57) |

## 06 — Databases

| Lesson and canonical issue | Source coverage | Prerequisites |
| --- | --- | --- |
| [SD-06.01 — Relational database fundamentals](https://github.com/PhoNoodles/system-design-learning/issues/59) (#59) | Primer + extension | [SD-05.03](https://github.com/PhoNoodles/system-design-learning/issues/49) |
| [SD-06.02 — ACID transactions](https://github.com/PhoNoodles/system-design-learning/issues/60) (#60) | Primer | [SD-06.01](https://github.com/PhoNoodles/system-design-learning/issues/59) |
| [SD-06.03 — Isolation levels and anomalies](https://github.com/PhoNoodles/system-design-learning/issues/61) (#61) | Supplemental | [SD-06.02](https://github.com/PhoNoodles/system-design-learning/issues/60) |
| [SD-06.04 — Indexes and query plans](https://github.com/PhoNoodles/system-design-learning/issues/62) (#62) | Primer + extension | [SD-06.01](https://github.com/PhoNoodles/system-design-learning/issues/59) |
| [SD-06.05 — SQL tuning](https://github.com/PhoNoodles/system-design-learning/issues/63) (#63) | Primer | [SD-06.04](https://github.com/PhoNoodles/system-design-learning/issues/62), [SD-01.04](https://github.com/PhoNoodles/system-design-learning/issues/4) |
| [SD-06.06 — Connection pooling](https://github.com/PhoNoodles/system-design-learning/issues/64) (#64) | Primer + extension | [SD-06.02](https://github.com/PhoNoodles/system-design-learning/issues/60), [SD-03.04](https://github.com/PhoNoodles/system-design-learning/issues/28) |
| [SD-06.07 — Leader-follower database replication](https://github.com/PhoNoodles/system-design-learning/issues/65) (#65) | Primer + extension | [SD-02.09](https://github.com/PhoNoodles/system-design-learning/issues/17), [SD-06.02](https://github.com/PhoNoodles/system-design-learning/issues/60) |
| [SD-06.08 — Read replicas and replication lag](https://github.com/PhoNoodles/system-design-learning/issues/66) (#66) | Primer | [SD-06.07](https://github.com/PhoNoodles/system-design-learning/issues/65), [SD-02.06](https://github.com/PhoNoodles/system-design-learning/issues/14) |
| [SD-06.09 — Multi-leader database replication](https://github.com/PhoNoodles/system-design-learning/issues/67) (#67) | Primer + extension | [SD-02.10](https://github.com/PhoNoodles/system-design-learning/issues/18), [SD-06.03](https://github.com/PhoNoodles/system-design-learning/issues/61), [SD-06.07](https://github.com/PhoNoodles/system-design-learning/issues/65) |
| [SD-06.10 — Federation and partitioning](https://github.com/PhoNoodles/system-design-learning/issues/68) (#68) | Primer | [SD-06.01](https://github.com/PhoNoodles/system-design-learning/issues/59), [SD-06.05](https://github.com/PhoNoodles/system-design-learning/issues/63) |
| [SD-06.11 — Sharding and shard keys](https://github.com/PhoNoodles/system-design-learning/issues/69) (#69) | Primer | [SD-06.10](https://github.com/PhoNoodles/system-design-learning/issues/68), [SD-06.07](https://github.com/PhoNoodles/system-design-learning/issues/65) |
| [SD-06.12 — Denormalization](https://github.com/PhoNoodles/system-design-learning/issues/70) (#70) | Primer | [SD-06.05](https://github.com/PhoNoodles/system-design-learning/issues/63), [SD-06.11](https://github.com/PhoNoodles/system-design-learning/issues/69) |
| [SD-06.13 — Key-value databases](https://github.com/PhoNoodles/system-design-learning/issues/71) (#71) | Primer | [SD-06.01](https://github.com/PhoNoodles/system-design-learning/issues/59), [SD-02.04](https://github.com/PhoNoodles/system-design-learning/issues/12) |
| [SD-06.14 — Document databases](https://github.com/PhoNoodles/system-design-learning/issues/72) (#72) | Primer | [SD-06.13](https://github.com/PhoNoodles/system-design-learning/issues/71), [SD-06.12](https://github.com/PhoNoodles/system-design-learning/issues/70) |
| [SD-06.15 — Wide-column and graph databases](https://github.com/PhoNoodles/system-design-learning/issues/73) (#73) | Primer | [SD-06.11](https://github.com/PhoNoodles/system-design-learning/issues/69), [SD-06.14](https://github.com/PhoNoodles/system-design-learning/issues/72) |
| [SD-06.16 — SQL vs NoSQL tradeoffs and assessment](https://github.com/PhoNoodles/system-design-learning/issues/74) (#74) | Assessment | [SD-06.09](https://github.com/PhoNoodles/system-design-learning/issues/67), [SD-06.12](https://github.com/PhoNoodles/system-design-learning/issues/70), [SD-06.15](https://github.com/PhoNoodles/system-design-learning/issues/73) |

## 07 — Caching

| Lesson and canonical issue | Source coverage | Prerequisites |
| --- | --- | --- |
| [SD-07.01 — Cache fundamentals and locality](https://github.com/PhoNoodles/system-design-learning/issues/75) (#75) | Primer | [SD-01.02](https://github.com/PhoNoodles/system-design-learning/issues/2), [SD-06.01](https://github.com/PhoNoodles/system-design-learning/issues/59) |
| [SD-07.02 — Client and browser caching](https://github.com/PhoNoodles/system-design-learning/issues/76) (#76) | Primer + extension | [SD-03.06](https://github.com/PhoNoodles/system-design-learning/issues/30), [SD-07.01](https://github.com/PhoNoodles/system-design-learning/issues/75) |
| [SD-07.03 — CDN caching](https://github.com/PhoNoodles/system-design-learning/issues/77) (#77) | Primer | [SD-03.05](https://github.com/PhoNoodles/system-design-learning/issues/29), [SD-07.01](https://github.com/PhoNoodles/system-design-learning/issues/75) |
| [SD-07.04 — Web server, application, and database caching](https://github.com/PhoNoodles/system-design-learning/issues/78) (#78) | Primer | [SD-06.04](https://github.com/PhoNoodles/system-design-learning/issues/62), [SD-07.01](https://github.com/PhoNoodles/system-design-learning/issues/75) |
| [SD-07.05 — Cache-aside](https://github.com/PhoNoodles/system-design-learning/issues/79) (#79) | Primer | [SD-07.04](https://github.com/PhoNoodles/system-design-learning/issues/78) |
| [SD-07.06 — Read-through and write-through](https://github.com/PhoNoodles/system-design-learning/issues/80) (#80) | Primer + extension | [SD-07.05](https://github.com/PhoNoodles/system-design-learning/issues/79) |
| [SD-07.07 — Write-back and write-around](https://github.com/PhoNoodles/system-design-learning/issues/81) (#81) | Primer + extension | [SD-07.06](https://github.com/PhoNoodles/system-design-learning/issues/80) |
| [SD-07.08 — TTL and eviction policies](https://github.com/PhoNoodles/system-design-learning/issues/82) (#82) | Primer + extension | [SD-07.01](https://github.com/PhoNoodles/system-design-learning/issues/75) |
| [SD-07.09 — Invalidation and cache stampedes](https://github.com/PhoNoodles/system-design-learning/issues/83) (#83) | Primer + extension | [SD-07.05](https://github.com/PhoNoodles/system-design-learning/issues/79), [SD-07.08](https://github.com/PhoNoodles/system-design-learning/issues/82) |
| [SD-07.11 — Refresh-ahead caching](https://github.com/PhoNoodles/system-design-learning/issues/123) (#123) | Primer | [SD-07.05](https://github.com/PhoNoodles/system-design-learning/issues/79), [SD-07.08](https://github.com/PhoNoodles/system-design-learning/issues/82), [SD-07.09](https://github.com/PhoNoodles/system-design-learning/issues/83) |
| [SD-07.10 — Caching assessment](https://github.com/PhoNoodles/system-design-learning/issues/84) (#84) | Assessment | [SD-07.07](https://github.com/PhoNoodles/system-design-learning/issues/81), [SD-07.09](https://github.com/PhoNoodles/system-design-learning/issues/83), [SD-07.11](https://github.com/PhoNoodles/system-design-learning/issues/123) |

## 08 — Asynchronous processing

| Lesson and canonical issue | Source coverage | Prerequisites |
| --- | --- | --- |
| [SD-08.01 — Message queues vs task queues](https://github.com/PhoNoodles/system-design-learning/issues/85) (#85) | Primer | [SD-05.05](https://github.com/PhoNoodles/system-design-learning/issues/51) |
| [SD-08.02 — Publish-subscribe and event streams](https://github.com/PhoNoodles/system-design-learning/issues/86) (#86) | Supplemental | [SD-08.01](https://github.com/PhoNoodles/system-design-learning/issues/85) |
| [SD-08.03 — Delivery guarantees](https://github.com/PhoNoodles/system-design-learning/issues/87) (#87) | Primer + extension | [SD-08.01](https://github.com/PhoNoodles/system-design-learning/issues/85) |
| [SD-08.04 — Ordering and partition keys](https://github.com/PhoNoodles/system-design-learning/issues/88) (#88) | Supplemental | [SD-08.02](https://github.com/PhoNoodles/system-design-learning/issues/86), [SD-08.03](https://github.com/PhoNoodles/system-design-learning/issues/87) |
| [SD-08.05 — Consumer groups and workers](https://github.com/PhoNoodles/system-design-learning/issues/89) (#89) | Supplemental | [SD-08.02](https://github.com/PhoNoodles/system-design-learning/issues/86), [SD-08.04](https://github.com/PhoNoodles/system-design-learning/issues/88) |
| [SD-08.06 — Retries and dead-letter queues](https://github.com/PhoNoodles/system-design-learning/issues/90) (#90) | Supplemental | [SD-02.13](https://github.com/PhoNoodles/system-design-learning/issues/23), [SD-08.03](https://github.com/PhoNoodles/system-design-learning/issues/87) |
| [SD-08.07 — Idempotent consumers and deduplication](https://github.com/PhoNoodles/system-design-learning/issues/91) (#91) | Supplemental | [SD-05.06](https://github.com/PhoNoodles/system-design-learning/issues/52), [SD-08.03](https://github.com/PhoNoodles/system-design-learning/issues/87) |
| [SD-08.08 — Backpressure and flow control](https://github.com/PhoNoodles/system-design-learning/issues/92) (#92) | Primer | [SD-08.01](https://github.com/PhoNoodles/system-design-learning/issues/85), [SD-01.02](https://github.com/PhoNoodles/system-design-learning/issues/2) |
| [SD-08.09 — Transactional outbox and sagas](https://github.com/PhoNoodles/system-design-learning/issues/93) (#93) | Supplemental | [SD-06.02](https://github.com/PhoNoodles/system-design-learning/issues/60), [SD-08.06](https://github.com/PhoNoodles/system-design-learning/issues/90), [SD-08.07](https://github.com/PhoNoodles/system-design-learning/issues/91) |
| [SD-08.10 — Asynchronous processing assessment](https://github.com/PhoNoodles/system-design-learning/issues/94) (#94) | Assessment | [SD-08.05](https://github.com/PhoNoodles/system-design-learning/issues/89), [SD-08.08](https://github.com/PhoNoodles/system-design-learning/issues/92), [SD-08.09](https://github.com/PhoNoodles/system-design-learning/issues/93) |

## 09 — Security

| Lesson and canonical issue | Source coverage | Prerequisites |
| --- | --- | --- |
| [SD-09.01 — Authentication vs authorization](https://github.com/PhoNoodles/system-design-learning/issues/95) (#95) | Supplemental | [SD-03.06](https://github.com/PhoNoodles/system-design-learning/issues/30) |
| [SD-09.02 — Sessions and cookies](https://github.com/PhoNoodles/system-design-learning/issues/96) (#96) | Supplemental | [SD-09.01](https://github.com/PhoNoodles/system-design-learning/issues/95), [SD-03.08](https://github.com/PhoNoodles/system-design-learning/issues/32) |
| [SD-09.03 — JWT and token lifecycle](https://github.com/PhoNoodles/system-design-learning/issues/97) (#97) | Supplemental | [SD-09.01](https://github.com/PhoNoodles/system-design-learning/issues/95), [SD-03.08](https://github.com/PhoNoodles/system-design-learning/issues/32) |
| [SD-09.04 — OAuth 2.0 and OpenID Connect](https://github.com/PhoNoodles/system-design-learning/issues/98) (#98) | Supplemental | [SD-09.01](https://github.com/PhoNoodles/system-design-learning/issues/95), [SD-09.03](https://github.com/PhoNoodles/system-design-learning/issues/97) |
| [SD-09.05 — RBAC and least privilege](https://github.com/PhoNoodles/system-design-learning/issues/99) (#99) | Primer + extension | [SD-09.01](https://github.com/PhoNoodles/system-design-learning/issues/95) |
| [SD-09.06 — Encryption at rest and in transit](https://github.com/PhoNoodles/system-design-learning/issues/100) (#100) | Primer | [SD-03.08](https://github.com/PhoNoodles/system-design-learning/issues/32) |
| [SD-09.07 — Secrets management](https://github.com/PhoNoodles/system-design-learning/issues/101) (#101) | Supplemental | [SD-09.05](https://github.com/PhoNoodles/system-design-learning/issues/99), [SD-09.06](https://github.com/PhoNoodles/system-design-learning/issues/100) |
| [SD-09.08 — Input validation and injection prevention](https://github.com/PhoNoodles/system-design-learning/issues/102) (#102) | Primer | [SD-03.09](https://github.com/PhoNoodles/system-design-learning/issues/33), [SD-06.01](https://github.com/PhoNoodles/system-design-learning/issues/59) |
| [SD-09.09 — Threat modeling and tenant isolation](https://github.com/PhoNoodles/system-design-learning/issues/103) (#103) | Supplemental | [SD-09.05](https://github.com/PhoNoodles/system-design-learning/issues/99), [SD-09.08](https://github.com/PhoNoodles/system-design-learning/issues/102) |
| [SD-09.10 — Security assessment](https://github.com/PhoNoodles/system-design-learning/issues/104) (#104) | Assessment | [SD-09.04](https://github.com/PhoNoodles/system-design-learning/issues/98), [SD-09.07](https://github.com/PhoNoodles/system-design-learning/issues/101), [SD-09.09](https://github.com/PhoNoodles/system-design-learning/issues/103) |

## 10 — System design practice

| Lesson and canonical issue | Source coverage | Prerequisites |
| --- | --- | --- |
| [SD-10.01 — Requirements and constraints](https://github.com/PhoNoodles/system-design-learning/issues/105) (#105) | Primer | [SD-01.08](https://github.com/PhoNoodles/system-design-learning/issues/8) |
| [SD-10.02 — Back-of-envelope calculations](https://github.com/PhoNoodles/system-design-learning/issues/106) (#106) | Primer | [SD-01.07](https://github.com/PhoNoodles/system-design-learning/issues/7), [SD-10.01](https://github.com/PhoNoodles/system-design-learning/issues/105) |
| [SD-10.03 — High-level design and API contracts](https://github.com/PhoNoodles/system-design-learning/issues/122) (#122) | Primer + extension | [SD-03.09](https://github.com/PhoNoodles/system-design-learning/issues/33), [SD-10.01](https://github.com/PhoNoodles/system-design-learning/issues/105), [SD-10.02](https://github.com/PhoNoodles/system-design-learning/issues/106) |
| [SD-10.04 — Data modeling and core components](https://github.com/PhoNoodles/system-design-learning/issues/107) (#107) | Primer | [SD-06.16](https://github.com/PhoNoodles/system-design-learning/issues/74), [SD-10.03](https://github.com/PhoNoodles/system-design-learning/issues/122) |
| [SD-10.05 — Design URL shortener or Pastebin](https://github.com/PhoNoodles/system-design-learning/issues/108) (#108) | Primer | [SD-07.10](https://github.com/PhoNoodles/system-design-learning/issues/84), [SD-10.04](https://github.com/PhoNoodles/system-design-learning/issues/107) |
| [SD-10.06 — Design a social timeline and search](https://github.com/PhoNoodles/system-design-learning/issues/109) (#109) | Primer | [SD-08.10](https://github.com/PhoNoodles/system-design-learning/issues/94), [SD-10.04](https://github.com/PhoNoodles/system-design-learning/issues/107) |
| [SD-10.07 — Design a web crawler](https://github.com/PhoNoodles/system-design-learning/issues/110) (#110) | Primer | [SD-08.10](https://github.com/PhoNoodles/system-design-learning/issues/94), [SD-10.04](https://github.com/PhoNoodles/system-design-learning/issues/107) |
| [SD-10.08 — Design a distributed key-value query cache](https://github.com/PhoNoodles/system-design-learning/issues/111) (#111) | Primer | [SD-07.10](https://github.com/PhoNoodles/system-design-learning/issues/84), [SD-10.04](https://github.com/PhoNoodles/system-design-learning/issues/107) |
| [SD-10.09 — Design SAP-to-MES manufacturing integration](https://github.com/PhoNoodles/system-design-learning/issues/112) (#112) | Supplemental | [SD-08.10](https://github.com/PhoNoodles/system-design-learning/issues/94), [SD-09.10](https://github.com/PhoNoodles/system-design-learning/issues/104), [SD-10.04](https://github.com/PhoNoodles/system-design-learning/issues/107) |
| [SD-10.11 — Design a financial aggregation and budgeting service](https://github.com/PhoNoodles/system-design-learning/issues/124) (#124) | Primer | [SD-08.10](https://github.com/PhoNoodles/system-design-learning/issues/94), [SD-09.10](https://github.com/PhoNoodles/system-design-learning/issues/104), [SD-10.04](https://github.com/PhoNoodles/system-design-learning/issues/107) |
| [SD-10.12 — Design social-network data structures and graph traversal](https://github.com/PhoNoodles/system-design-learning/issues/125) (#125) | Primer | [SD-06.11](https://github.com/PhoNoodles/system-design-learning/issues/69), [SD-06.15](https://github.com/PhoNoodles/system-design-learning/issues/73), [SD-10.04](https://github.com/PhoNoodles/system-design-learning/issues/107) |
| [SD-10.10 — Full mock interview and tradeoff defense](https://github.com/PhoNoodles/system-design-learning/issues/113) (#113) | Assessment | [SD-10.05](https://github.com/PhoNoodles/system-design-learning/issues/108), [SD-10.06](https://github.com/PhoNoodles/system-design-learning/issues/109), [SD-10.11](https://github.com/PhoNoodles/system-design-learning/issues/124) |

## 11 — Advanced architecture

| Lesson and canonical issue | Source coverage | Prerequisites |
| --- | --- | --- |
| [SD-11.01 — Push vs pull CDNs](https://github.com/PhoNoodles/system-design-learning/issues/114) (#114) | Primer | [SD-07.03](https://github.com/PhoNoodles/system-design-learning/issues/77) |
| [SD-11.02 — Object storage and distributed files](https://github.com/PhoNoodles/system-design-learning/issues/115) (#115) | Primer + extension | [SD-06.11](https://github.com/PhoNoodles/system-design-learning/issues/69), [SD-02.12](https://github.com/PhoNoodles/system-design-learning/issues/22) |
| [SD-11.03 — Consistent hashing](https://github.com/PhoNoodles/system-design-learning/issues/116) (#116) | Primer + extension | [SD-06.11](https://github.com/PhoNoodles/system-design-learning/issues/69), [SD-07.01](https://github.com/PhoNoodles/system-design-learning/issues/75) |
| [SD-11.04 — Distributed coordination and consensus](https://github.com/PhoNoodles/system-design-learning/issues/117) (#117) | Primer + extension | [SD-02.01](https://github.com/PhoNoodles/system-design-learning/issues/9), [SD-02.11](https://github.com/PhoNoodles/system-design-learning/issues/21) |
| [SD-11.05 — Search indexes and indexing pipelines](https://github.com/PhoNoodles/system-design-learning/issues/118) (#118) | Primer + extension | [SD-08.10](https://github.com/PhoNoodles/system-design-learning/issues/94), [SD-10.06](https://github.com/PhoNoodles/system-design-learning/issues/109) |
| [SD-11.06 — Disaster recovery RPO and RTO](https://github.com/PhoNoodles/system-design-learning/issues/119) (#119) | Supplemental | [SD-02.12](https://github.com/PhoNoodles/system-design-learning/issues/22), [SD-06.08](https://github.com/PhoNoodles/system-design-learning/issues/66) |
| [SD-11.07 — Design a sales ranking system](https://github.com/PhoNoodles/system-design-learning/issues/120) (#120) | Primer | [SD-08.10](https://github.com/PhoNoodles/system-design-learning/issues/94), [SD-10.04](https://github.com/PhoNoodles/system-design-learning/issues/107) |
| [SD-11.08 — Scale a system to millions of users on AWS](https://github.com/PhoNoodles/system-design-learning/issues/121) (#121) | Primer | [SD-04.10](https://github.com/PhoNoodles/system-design-learning/issues/46), [SD-06.16](https://github.com/PhoNoodles/system-design-learning/issues/74), [SD-07.10](https://github.com/PhoNoodles/system-design-learning/issues/84) |

## 12 — Optional object-oriented design

| Lesson and canonical issue | Source coverage | Prerequisites |
| --- | --- | --- |
| [SD-12.01 — Design a hash map](https://github.com/PhoNoodles/system-design-learning/issues/126) (#126) | Primer | None |
| [SD-12.02 — Design an LRU cache](https://github.com/PhoNoodles/system-design-learning/issues/127) (#127) | Primer | [SD-12.01](https://github.com/PhoNoodles/system-design-learning/issues/126), [SD-07.08](https://github.com/PhoNoodles/system-design-learning/issues/82) |
| [SD-12.03 — Design a call center](https://github.com/PhoNoodles/system-design-learning/issues/128) (#128) | Primer | None |
| [SD-12.04 — Design a deck of cards](https://github.com/PhoNoodles/system-design-learning/issues/129) (#129) | Primer | None |
| [SD-12.05 — Design a parking lot](https://github.com/PhoNoodles/system-design-learning/issues/130) (#130) | Primer | None |
| [SD-12.06 — Design chat-server objects](https://github.com/PhoNoodles/system-design-learning/issues/131) (#131) | Primer | [SD-05.01](https://github.com/PhoNoodles/system-design-learning/issues/47) |
| [SD-12.07 — Design a circular array](https://github.com/PhoNoodles/system-design-learning/issues/132) (#132) | Upstream placeholder | None |

## 13 — Optional system-design practice bank

| Lesson and canonical issue | Source coverage | Prerequisites |
| --- | --- | --- |
| [SD-13.01 — Design file synchronization and conflict resolution](https://github.com/PhoNoodles/system-design-learning/issues/133) (#133) | Primer prompt | [SD-03.09](https://github.com/PhoNoodles/system-design-learning/issues/33), [SD-05.06](https://github.com/PhoNoodles/system-design-learning/issues/52), [SD-08.01](https://github.com/PhoNoodles/system-design-learning/issues/85), [SD-11.02](https://github.com/PhoNoodles/system-design-learning/issues/115) |
| [SD-13.02 — Design a search engine](https://github.com/PhoNoodles/system-design-learning/issues/134) (#134) | Primer prompt | [SD-10.07](https://github.com/PhoNoodles/system-design-learning/issues/110), [SD-11.05](https://github.com/PhoNoodles/system-design-learning/issues/118) |
| [SD-13.03 — Design collaborative document editing](https://github.com/PhoNoodles/system-design-learning/issues/135) (#135) | Primer prompt | [SD-02.02](https://github.com/PhoNoodles/system-design-learning/issues/10), [SD-02.04](https://github.com/PhoNoodles/system-design-learning/issues/12), [SD-03.11](https://github.com/PhoNoodles/system-design-learning/issues/35), [SD-05.06](https://github.com/PhoNoodles/system-design-learning/issues/52) |
| [SD-13.04 — Design a persistent distributed key-value store](https://github.com/PhoNoodles/system-design-learning/issues/136) (#136) | Primer prompt | [SD-06.13](https://github.com/PhoNoodles/system-design-learning/issues/71), [SD-02.09](https://github.com/PhoNoodles/system-design-learning/issues/17), [SD-02.11](https://github.com/PhoNoodles/system-design-learning/issues/21), [SD-11.03](https://github.com/PhoNoodles/system-design-learning/issues/116) |
| [SD-13.05 — Design a recommendation service](https://github.com/PhoNoodles/system-design-learning/issues/137) (#137) | Primer prompt | [SD-08.02](https://github.com/PhoNoodles/system-design-learning/issues/86), [SD-11.02](https://github.com/PhoNoodles/system-design-learning/issues/115), [SD-11.05](https://github.com/PhoNoodles/system-design-learning/issues/118) |
| [SD-13.06 — Design chat delivery and synchronization](https://github.com/PhoNoodles/system-design-learning/issues/138) (#138) | Primer prompt | [SD-03.11](https://github.com/PhoNoodles/system-design-learning/issues/35), [SD-05.06](https://github.com/PhoNoodles/system-design-learning/issues/52), [SD-08.03](https://github.com/PhoNoodles/system-design-learning/issues/87), [SD-08.04](https://github.com/PhoNoodles/system-design-learning/issues/88) |
| [SD-13.07 — Design photo sharing and media delivery](https://github.com/PhoNoodles/system-design-learning/issues/139) (#139) | Primer prompt | [SD-07.03](https://github.com/PhoNoodles/system-design-learning/issues/77), [SD-10.06](https://github.com/PhoNoodles/system-design-learning/issues/109), [SD-11.02](https://github.com/PhoNoodles/system-design-learning/issues/115) |
| [SD-13.08 — Design graph search and ranked results](https://github.com/PhoNoodles/system-design-learning/issues/140) (#140) | Primer prompt | [SD-06.15](https://github.com/PhoNoodles/system-design-learning/issues/73), [SD-10.12](https://github.com/PhoNoodles/system-design-learning/issues/125), [SD-11.05](https://github.com/PhoNoodles/system-design-learning/issues/118) |
| [SD-13.09 — Design a content delivery network](https://github.com/PhoNoodles/system-design-learning/issues/141) (#141) | Primer prompt | [SD-03.05](https://github.com/PhoNoodles/system-design-learning/issues/29), [SD-07.03](https://github.com/PhoNoodles/system-design-learning/issues/77), [SD-07.09](https://github.com/PhoNoodles/system-design-learning/issues/83), [SD-11.01](https://github.com/PhoNoodles/system-design-learning/issues/114) |
| [SD-13.10 — Design trending-topic detection](https://github.com/PhoNoodles/system-design-learning/issues/142) (#142) | Primer prompt | [SD-08.02](https://github.com/PhoNoodles/system-design-learning/issues/86), [SD-08.04](https://github.com/PhoNoodles/system-design-learning/issues/88), [SD-11.07](https://github.com/PhoNoodles/system-design-learning/issues/120) |
| [SD-13.11 — Design distributed unique ID generation](https://github.com/PhoNoodles/system-design-learning/issues/143) (#143) | Primer prompt | [SD-02.02](https://github.com/PhoNoodles/system-design-learning/issues/10), [SD-05.06](https://github.com/PhoNoodles/system-design-learning/issues/52), [SD-11.03](https://github.com/PhoNoodles/system-design-learning/issues/116) |
| [SD-13.12 — Design top-k requests over a time window](https://github.com/PhoNoodles/system-design-learning/issues/144) (#144) | Primer prompt | [SD-08.02](https://github.com/PhoNoodles/system-design-learning/issues/86), [SD-08.04](https://github.com/PhoNoodles/system-design-learning/issues/88), [SD-11.07](https://github.com/PhoNoodles/system-design-learning/issues/120) |
| [SD-13.13 — Design service delivery across data centers](https://github.com/PhoNoodles/system-design-learning/issues/145) (#145) | Primer prompt | [SD-02.01](https://github.com/PhoNoodles/system-design-learning/issues/9), [SD-02.08](https://github.com/PhoNoodles/system-design-learning/issues/16), [SD-06.09](https://github.com/PhoNoodles/system-design-learning/issues/67), [SD-11.06](https://github.com/PhoNoodles/system-design-learning/issues/119) |
| [SD-13.14 — Design an online multiplayer card game](https://github.com/PhoNoodles/system-design-learning/issues/146) (#146) | Primer prompt | [SD-03.11](https://github.com/PhoNoodles/system-design-learning/issues/35), [SD-05.01](https://github.com/PhoNoodles/system-design-learning/issues/47), [SD-05.06](https://github.com/PhoNoodles/system-design-learning/issues/52) |
| [SD-13.15 — Design a garbage collector](https://github.com/PhoNoodles/system-design-learning/issues/147) (#147) | Primer prompt | None |
| [SD-13.16 — Design an exchange order-matching system](https://github.com/PhoNoodles/system-design-learning/issues/148) (#148) | Primer prompt | [SD-05.06](https://github.com/PhoNoodles/system-design-learning/issues/52), [SD-06.02](https://github.com/PhoNoodles/system-design-learning/issues/60), [SD-08.04](https://github.com/PhoNoodles/system-design-learning/issues/88), [SD-11.06](https://github.com/PhoNoodles/system-design-learning/issues/119) |

## 14 — Optional architecture reading

| Lesson and canonical issue | Source coverage | Prerequisites |
| --- | --- | --- |
| [SD-14.01 — Read and compare real-world architecture papers](https://github.com/PhoNoodles/system-design-learning/issues/149) (#149) | Reference activity | [SD-06.16](https://github.com/PhoNoodles/system-design-learning/issues/74), [SD-08.10](https://github.com/PhoNoodles/system-design-learning/issues/94), [SD-11.04](https://github.com/PhoNoodles/system-design-learning/issues/117) |
| [SD-14.02 — Review a company architecture and engineering case study](https://github.com/PhoNoodles/system-design-learning/issues/150) (#150) | Reference activity | [SD-10.10](https://github.com/PhoNoodles/system-design-learning/issues/113) |

## Coverage boundaries

All eight worked system-design examples and every named additional interview prompt in the audited Primer are mapped in SOURCE_MAP.md. Shared variants reuse canonical issues and retain separate evidence where their requirements differ. The six object-oriented notebooks and the circular-array placeholder are explicitly optional. Reference activities sample the architecture and engineering-blog directories; they do not claim mastery of every linked article. Supplemental source selections are verified when each lesson is taught.
