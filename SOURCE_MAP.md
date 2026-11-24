# Source map

This document maps the educational sections of [The System Design Primer](https://github.com/donnemartin/system-design-primer) to this repository's canonical learning issues. The course has **148 learning issues: 123 main and 25 optional**. All source sections have an explicit disposition: a lesson, an optional exercise, a reference activity, orientation material, or a deliberate administrative exclusion.

**Reviewed:** 2026-11-24, America/Los_Angeles. **Source:** the upstream English README, content blob SHA `9e2cdb88dec86c34c9b49b657f5629a1866c6976`. This is a content fingerprint, not a commit identifier. The links below point to the upstream repository and may evolve after this review.

Coverage means that a learning task exists with an intended scope. It does **not** mean the learner has completed that task. Issue comments, independent assessment evidence and issue state remain the learning record under [LEARNING_PROTOCOL.md](LEARNING_PROTOCOL.md). The closed administrative duplicates #19 and #20 are excluded from the curriculum and mastery counts.

## How to use this map

Read [CURRICULUM.md](CURRICULUM.md) for the learning order and prerequisites. Use this map to find the original source and the issue that records the related work. Prerequisites take priority over numeric IDs: refresh-ahead precedes the caching assessment, and the financial-aggregation exercise precedes the full mock assessment.

The course reorganizes the Primer into a teachable sequence and adds original objectives, exercises and assessments. The issue source classifications distinguish these relationships:

| Classification | Meaning |
| --- | --- |
| `primer` | A topic or worked exercise directly represented in the source, taught through original lesson objectives. |
| `mixed` | A source topic with explicitly expanded practical detail. |
| `extension` | Added course material without a corresponding full Primer lesson. |
| `assessment` | An original course assessment of the listed subject area. |
| `prompt` | An optional design exercise prompted by the source's additional-question list. |
| `reference` | Selected reading from a source directory; completion covers only the selected material. |
| `placeholder` | An original optional exercise extending an upstream entry with no supplied solution. |

Supplemental technical readings will be selected from primary sources when the lesson is taught and recorded in its issue. Historical diagrams, product details, measurements and simplified statements are discussion inputs; concrete modern implementations require current official documentation. The audit checked curriculum coverage, linked issue identities and source structure. It did **not** validate every external link, article, video or assertion in the upstream bibliography.

## Source concepts and learning process

The tables include the instructional headings and their meaningful subtopics. Generic “disadvantages” and “sources/further reading” subheadings inherit their parent topic's mapping: the relevant issue requires tradeoffs, and further reading is selected when useful. Navigation-only headings do not create additional mastery requirements.

### Orientation and review

| Primer topic / source | Canonical learning record | Coverage and scope |
| --- | --- | --- |
| [Study guide](https://github.com/donnemartin/system-design-primer#study-guide) | [Orientation and review](README.md#orientation-and-review) | Orientation explains breadth, depth and adapting the course to the learning goal. |
| [Anki flashcards](https://github.com/donnemartin/system-design-primer#anki-flashcards) | [Orientation and review](README.md#orientation-and-review) | The source provides system-design, system-design-exercise and OOD decks. Use optional retrieval practice; flashcard exposure alone does not establish mastery. |
| [System design topics: start here; scalability lecture; scalability article](https://github.com/donnemartin/system-design-primer#system-design-topics-start-here) | [Orientation and review](README.md#orientation-and-review); [SD-01.03 · #3](https://github.com/PhoNoodles/system-design-learning/issues/3), [SD-04.01 · #37](https://github.com/PhoNoodles/system-design-learning/issues/37), [SD-05.01 · #47](https://github.com/PhoNoodles/system-design-learning/issues/47), [SD-06.07 · #65](https://github.com/PhoNoodles/system-design-learning/issues/65), [SD-06.11 · #69](https://github.com/PhoNoodles/system-design-learning/issues/69), [SD-07.01 · #75](https://github.com/PhoNoodles/system-design-learning/issues/75), [SD-08.01 · #85](https://github.com/PhoNoodles/system-design-learning/issues/85) | Orientation links the starting lecture and scalability article. Their scaling, cache, queue and database concepts are distributed across the main course. |

### Design process and estimation

| Primer topic / source | Canonical learning record | Coverage and scope |
| --- | --- | --- |
| [Interview process: requirements, constraints, assumptions](https://github.com/donnemartin/system-design-primer#step-1-outline-use-cases-constraints-and-assumptions) | [SD-10.01 · #105](https://github.com/PhoNoodles/system-design-learning/issues/105) | Scope use cases, constraints, workload and assumptions before choosing components. |
| [Interview process: high level design](https://github.com/donnemartin/system-design-primer#step-2-create-a-high-level-design) | [SD-10.03 · #122](https://github.com/PhoNoodles/system-design-learning/issues/122) | A canonical issue now covers the component diagram, request paths and API contracts. |
| [Interview process: core components](https://github.com/donnemartin/system-design-primer#step-3-design-core-components) | [SD-10.04 · #107](https://github.com/PhoNoodles/system-design-learning/issues/107) | Model data and design the core read/write behavior from access patterns. |
| [Interview process: scale the design](https://github.com/donnemartin/system-design-primer#step-4-scale-the-design) | [SD-01.04 · #4](https://github.com/PhoNoodles/system-design-learning/issues/4), [SD-10.10 · #113](https://github.com/PhoNoodles/system-design-learning/issues/113), [SD-11.08 · #121](https://github.com/PhoNoodles/system-design-learning/issues/121) | Measure the bottleneck, compare alternatives and evolve the design; do not add components without a requirement. |
| [Back-of-the-envelope calculations](https://github.com/donnemartin/system-design-primer#back-of-the-envelope-calculations) | [SD-01.07 · #7](https://github.com/PhoNoodles/system-design-learning/issues/7), [SD-10.02 · #106](https://github.com/PhoNoodles/system-design-learning/issues/106) | Capacity arithmetic includes units, average versus peak traffic, storage and bandwidth. |

### Fundamentals

| Primer topic / source | Canonical learning record | Coverage and scope |
| --- | --- | --- |
| [Performance vs scalability](https://github.com/donnemartin/system-design-primer#performance-vs-scalability) | [SD-01.01 · #1](https://github.com/PhoNoodles/system-design-learning/issues/1) | Performance at a fixed workload and capacity growth with resources are assessed separately. |
| [Latency vs throughput](https://github.com/donnemartin/system-design-primer#latency-vs-throughput) | [SD-01.02 · #2](https://github.com/PhoNoodles/system-design-learning/issues/2) | The course adds average versus tail-latency interpretation. |

### Consistency, availability and replication

| Primer topic / source | Canonical learning record | Coverage and scope |
| --- | --- | --- |
| [Availability vs consistency; CAP](https://github.com/donnemartin/system-design-primer#availability-vs-consistency) | [SD-02.01 · #9](https://github.com/PhoNoodles/system-design-learning/issues/9), [SD-02.02 · #10](https://github.com/PhoNoodles/system-design-learning/issues/10) | Availability/consistency tradeoffs are assessed using a partition scenario. |
| [CAP theorem](https://github.com/donnemartin/system-design-primer#cap-theorem) | [SD-02.01 · #9](https://github.com/PhoNoodles/system-design-learning/issues/9), [SD-02.02 · #10](https://github.com/PhoNoodles/system-design-learning/issues/10) | State the consistency and availability properties and explain their conflict during a partition. |
| [CP behavior](https://github.com/donnemartin/system-design-primer#cp---consistency-and-partition-tolerance) | [SD-02.01 · #9](https://github.com/PhoNoodles/system-design-learning/issues/9), [SD-02.02 · #10](https://github.com/PhoNoodles/system-design-learning/issues/10) | Trace operations that are rejected or delayed to preserve the required consistency. |
| [AP behavior](https://github.com/donnemartin/system-design-primer#ap---availability-and-partition-tolerance) | [SD-02.01 · #9](https://github.com/PhoNoodles/system-design-learning/issues/9), [SD-02.02 · #10](https://github.com/PhoNoodles/system-design-learning/issues/10) | Trace operations that remain available and identify possible stale/conflicting data. |
| [Consistency patterns](https://github.com/donnemartin/system-design-primer#consistency-patterns) | [SD-02.03 · #11](https://github.com/PhoNoodles/system-design-learning/issues/11), [SD-02.04 · #12](https://github.com/PhoNoodles/system-design-learning/issues/12), [SD-02.05 · #13](https://github.com/PhoNoodles/system-design-learning/issues/13) | Compare the promised observation contract rather than relying only on a label. |
| [Weak consistency](https://github.com/donnemartin/system-design-primer#weak-consistency) | [SD-02.03 · #11](https://github.com/PhoNoodles/system-design-learning/issues/11) | Identify guarantees that were not promised and the resulting user-visible behavior. |
| [Eventual consistency](https://github.com/donnemartin/system-design-primer#eventual-consistency) | [SD-02.04 · #12](https://github.com/PhoNoodles/system-design-learning/issues/12) | Explain convergence conditions without assuming a fixed bound on replication delay. |
| [Strong consistency](https://github.com/donnemartin/system-design-primer#strong-consistency) | [SD-02.05 · #13](https://github.com/PhoNoodles/system-design-learning/issues/13) | Use explicit operation timelines and distinguish linearizability from transaction isolation. |
| [Availability patterns / fail-over](https://github.com/donnemartin/system-design-primer#availability-patterns) | [SD-02.07 · #15](https://github.com/PhoNoodles/system-design-learning/issues/15), [SD-02.08 · #16](https://github.com/PhoNoodles/system-design-learning/issues/16) | Trace detection, traffic changes, recovery and remaining failure risks. |
| [Active-passive failover](https://github.com/donnemartin/system-design-primer#active-passive) | [SD-02.07 · #15](https://github.com/PhoNoodles/system-design-learning/issues/15), [SD-04.04 · #40](https://github.com/PhoNoodles/system-design-learning/issues/40) | Standby promotion and recovery are taught before database-specific application. |
| [Active-active failover](https://github.com/donnemartin/system-design-primer#active-active) | [SD-02.08 · #16](https://github.com/PhoNoodles/system-design-learning/issues/16), [SD-04.04 · #40](https://github.com/PhoNoodles/system-design-learning/issues/40) | Distinguish multiple active service instances from multiple database write leaders. |
| [Replication: master-slave/master-master](https://github.com/donnemartin/system-design-primer#replication) | [SD-02.09 · #17](https://github.com/PhoNoodles/system-design-learning/issues/17), [SD-02.10 · #18](https://github.com/PhoNoodles/system-design-learning/issues/18), [SD-06.07 · #65](https://github.com/PhoNoodles/system-design-learning/issues/65), [SD-06.09 · #67](https://github.com/PhoNoodles/system-design-learning/issues/67) | General topology/failure lessons precede database read/write applications; reuse recorded evidence instead of repeating foundations. |
| [Availability in numbers, three/four nines, parallel/series dependencies](https://github.com/donnemartin/system-design-primer#availability-in-numbers) | [SD-02.12 · #22](https://github.com/PhoNoodles/system-design-learning/issues/22) | Includes series/parallel dependency calculations with independence, failover and common-cause assumptions. SLO terminology is an expansion. |

### DNS, delivery, balancing and proxies

| Primer topic / source | Canonical learning record | Coverage and scope |
| --- | --- | --- |
| [DNS records, resolution, caching, routing](https://github.com/donnemartin/system-design-primer#domain-name-system) | [SD-03.05 · #29](https://github.com/PhoNoodles/system-design-learning/issues/29) | Includes record types, resolver/authoritative flow, TTL, traffic steering and stale failover information. |
| [CDN purpose and tradeoffs](https://github.com/donnemartin/system-design-primer#content-delivery-network) | [SD-07.03 · #77](https://github.com/PhoNoodles/system-design-learning/issues/77), [SD-11.01 · #114](https://github.com/PhoNoodles/system-design-learning/issues/114) | CDN basics are in caching; publication strategies receive a separate main lesson. |
| [Push CDNs](https://github.com/donnemartin/system-design-primer#push-cdns) | [SD-11.01 · #114](https://github.com/PhoNoodles/system-design-learning/issues/114) | Trace deliberate publication and updates to edge storage. |
| [Pull CDNs](https://github.com/donnemartin/system-design-primer#pull-cdns) | [SD-11.01 · #114](https://github.com/PhoNoodles/system-design-learning/issues/114) | Trace origin fetching and first-request behavior. |
| [Load balancer](https://github.com/donnemartin/system-design-primer#load-balancer) | [SD-04.01 · #37](https://github.com/PhoNoodles/system-design-learning/issues/37), [SD-04.03 · #39](https://github.com/PhoNoodles/system-design-learning/issues/39), [SD-04.04 · #40](https://github.com/PhoNoodles/system-design-learning/issues/40), [SD-04.06 · #42](https://github.com/PhoNoodles/system-design-learning/issues/42) | Covers backend selection, health routing, affinity, capacity and the balancer itself. |
| [Layer 4 load balancing](https://github.com/donnemartin/system-design-primer#layer-4-load-balancing) | [SD-04.02 · #38](https://github.com/PhoNoodles/system-design-learning/issues/38) | Compare transport-visible routing information and constraints. |
| [Layer 7 load balancing](https://github.com/donnemartin/system-design-primer#layer-7-load-balancing) | [SD-04.02 · #38](https://github.com/PhoNoodles/system-design-learning/issues/38) | Compare application-aware routing and TLS termination. |
| [Horizontal scaling and state](https://github.com/donnemartin/system-design-primer#horizontal-scaling) | [SD-01.03 · #3](https://github.com/PhoNoodles/system-design-learning/issues/3), [SD-04.07 · #43](https://github.com/PhoNoodles/system-design-learning/issues/43), [SD-05.01 · #47](https://github.com/PhoNoodles/system-design-learning/issues/47) | Connect scale-out with state placement and downstream capacity. |
| [Reverse proxy: TLS termination, caching, compression, static content, failure](https://github.com/donnemartin/system-design-primer#reverse-proxy-web-server) | [SD-04.05 · #41](https://github.com/PhoNoodles/system-design-learning/issues/41) | Includes termination, compression, caching, static assets and proxy availability. |
| [Load balancer vs reverse proxy](https://github.com/donnemartin/system-design-primer#load-balancer-vs-reverse-proxy) | [SD-04.05 · #41](https://github.com/PhoNoodles/system-design-learning/issues/41) | Explicitly compares proxying to a service and distributing work across instances, including product overlap. |

### Application architecture

| Primer topic / source | Canonical learning record | Coverage and scope |
| --- | --- | --- |
| [Application layer / web vs application tiers](https://github.com/donnemartin/system-design-primer#application-layer) | [SD-05.01 · #47](https://github.com/PhoNoodles/system-design-learning/issues/47), [SD-05.02 · #48](https://github.com/PhoNoodles/system-design-learning/issues/48) | Place web/proxy and application responsibilities in a request path; assess service state and boundaries. |
| [Microservices](https://github.com/donnemartin/system-design-primer#microservices) | [SD-05.02 · #48](https://github.com/PhoNoodles/system-design-learning/issues/48), [SD-05.03 · #49](https://github.com/PhoNoodles/system-design-learning/issues/49) | Compare modular monoliths and independently deployed services using actual requirements. |
| [Service discovery](https://github.com/donnemartin/system-design-primer#service-discovery) | [SD-05.04 · #50](https://github.com/PhoNoodles/system-design-learning/issues/50) | Covers registration, lookup, stale entries and the relationship to load balancing. |

### Database models and scaling

| Primer topic / source | Canonical learning record | Coverage and scope |
| --- | --- | --- |
| [RDBMS and ACID](https://github.com/donnemartin/system-design-primer#relational-database-management-system-rdbms) | [SD-06.01 · #59](https://github.com/PhoNoodles/system-design-learning/issues/59), [SD-06.02 · #60](https://github.com/PhoNoodles/system-design-learning/issues/60) | Data modeling and transaction properties receive separate lesson evidence. |
| [Leader-follower database replication](https://github.com/donnemartin/system-design-primer#master-slave-replication) | [SD-06.07 · #65](https://github.com/PhoNoodles/system-design-learning/issues/65), [SD-06.08 · #66](https://github.com/PhoNoodles/system-design-learning/issues/66) | Database lessons cover read/write routing, acknowledgment, replication lag and promotion. |
| [Multi-leader database replication](https://github.com/donnemartin/system-design-primer#master-master-replication) | [SD-06.09 · #67](https://github.com/PhoNoodles/system-design-learning/issues/67) | Assess concurrent updates, ownership, conflicts and database invariants. |
| [Federation](https://github.com/donnemartin/system-design-primer#federation) | [SD-06.10 · #68](https://github.com/PhoNoodles/system-design-learning/issues/68) | Distinguish splits by business function from table partitioning and sharding. |
| [Sharding](https://github.com/donnemartin/system-design-primer#sharding) | [SD-06.11 · #69](https://github.com/PhoNoodles/system-design-learning/issues/69) | Covers key choice, skew, routing, cross-shard work and resharding. |
| [Denormalization](https://github.com/donnemartin/system-design-primer#denormalization) | [SD-06.12 · #70](https://github.com/PhoNoodles/system-design-learning/issues/70) | Assess derived data, write amplification, freshness and repair. |
| [SQL tuning](https://github.com/donnemartin/system-design-primer#sql-tuning) | [SD-06.04 · #62](https://github.com/PhoNoodles/system-design-learning/issues/62), [SD-06.05 · #63](https://github.com/PhoNoodles/system-design-learning/issues/63) | Profile first, then evaluate schema, result size, joins, indexes, partitioning and batching. |
| [Tighten schema](https://github.com/donnemartin/system-design-primer#tighten-up-the-schema) | [SD-06.05 · #63](https://github.com/PhoNoodles/system-design-learning/issues/63) | Schema choice is evaluated against actual workload and engine behavior. |
| [Indices](https://github.com/donnemartin/system-design-primer#use-good-indices) | [SD-06.04 · #62](https://github.com/PhoNoodles/system-design-learning/issues/62), [SD-06.05 · #63](https://github.com/PhoNoodles/system-design-learning/issues/63) | Index choice and query plans include read benefit and write/storage costs. |
| [Avoid expensive joins](https://github.com/donnemartin/system-design-primer#avoid-expensive-joins) | [SD-06.05 · #63](https://github.com/PhoNoodles/system-design-learning/issues/63) | Analyze measured join work and alternatives; avoid universal rules about eliminating joins. |
| [Partition tables](https://github.com/donnemartin/system-design-primer#partition-tables) | [SD-06.05 · #63](https://github.com/PhoNoodles/system-design-learning/issues/63), [SD-06.10 · #68](https://github.com/PhoNoodles/system-design-learning/issues/68) | Separate table partitioning from business-function federation and cross-node sharding. |
| [Tune query cache](https://github.com/donnemartin/system-design-primer#tune-the-query-cache) | [SD-06.05 · #63](https://github.com/PhoNoodles/system-design-learning/issues/63), [SD-07.04 · #78](https://github.com/PhoNoodles/system-design-learning/issues/78) | Historical engine advice is qualified. Verify current support and distinguish database buffers from application result caches. |
| [NoSQL / BASE](https://github.com/donnemartin/system-design-primer#nosql) | [SD-06.13 · #71](https://github.com/PhoNoodles/system-design-learning/issues/71), [SD-06.14 · #72](https://github.com/PhoNoodles/system-design-learning/issues/72), [SD-06.15 · #73](https://github.com/PhoNoodles/system-design-learning/issues/73), [SD-06.16 · #74](https://github.com/PhoNoodles/system-design-learning/issues/74) | BASE and SQL/NoSQL terminology are assessed without assigning universal guarantees to every product in a category. |
| [Key-value store](https://github.com/donnemartin/system-design-primer#key-value-store) | [SD-06.13 · #71](https://github.com/PhoNoodles/system-design-learning/issues/71) | Model key-based access and evaluate persistence, consistency and eviction separately. |
| [Document store](https://github.com/donnemartin/system-design-primer#document-store) | [SD-06.14 · #72](https://github.com/PhoNoodles/system-design-learning/issues/72) | Choose embedding or references, validation, indexes and update boundaries. |
| [Wide-column store](https://github.com/donnemartin/system-design-primer#wide-column-store) | [SD-06.15 · #73](https://github.com/PhoNoodles/system-design-learning/issues/73) | The combined issue requires evidence of wide-column access patterns as its own objective. |
| [Graph database](https://github.com/donnemartin/system-design-primer#graph-database) | [SD-06.15 · #73](https://github.com/PhoNoodles/system-design-learning/issues/73) | The same issue separately requires graph modeling and traversal tradeoffs; GraphQL is not a graph database. |
| [SQL or NoSQL](https://github.com/donnemartin/system-design-primer#sql-or-nosql) | [SD-06.16 · #74](https://github.com/PhoNoodles/system-design-learning/issues/74) | The course adds an original assessment of storage selection and stated guarantees. |

### Caching

| Primer topic / source | Canonical learning record | Coverage and scope |
| --- | --- | --- |
| [Cache principles](https://github.com/donnemartin/system-design-primer#cache) | [SD-07.01 · #75](https://github.com/PhoNoodles/system-design-learning/issues/75) | Assess locality, hit/miss behavior, origin load and local/shared cache tradeoffs. |
| [Client caching](https://github.com/donnemartin/system-design-primer#client-caching) | [SD-07.02 · #76](https://github.com/PhoNoodles/system-design-learning/issues/76) | Adds practical freshness, validation and privacy-aware browser cache policy. |
| [CDN caching](https://github.com/donnemartin/system-design-primer#cdn-caching) | [SD-07.03 · #77](https://github.com/PhoNoodles/system-design-learning/issues/77) | Relates cache keys, location and origin fetches to CDN behavior. |
| [Web server caching](https://github.com/donnemartin/system-design-primer#web-server-caching) | [SD-07.04 · #78](https://github.com/PhoNoodles/system-design-learning/issues/78) | The cache-layer lesson explicitly covers reverse-proxy and response caches. |
| [Database caching](https://github.com/donnemartin/system-design-primer#database-caching) | [SD-07.04 · #78](https://github.com/PhoNoodles/system-design-learning/issues/78) | The cache-layer lesson distinguishes database caching from external result storage. |
| [Application caching](https://github.com/donnemartin/system-design-primer#application-caching) | [SD-07.04 · #78](https://github.com/PhoNoodles/system-design-learning/issues/78), [SD-07.08 · #82](https://github.com/PhoNoodles/system-design-learning/issues/82) | The cache-layer lesson covers application-held values and capacity; expiry/eviction is expanded separately. |
| [Query-level caching](https://github.com/donnemartin/system-design-primer#caching-at-the-database-query-level) | [SD-07.04 · #78](https://github.com/PhoNoodles/system-design-learning/issues/78) | Explicit query-result keys, dependent data and invalidation tradeoffs. |
| [Object-level caching](https://github.com/donnemartin/system-design-primer#caching-at-the-object-level) | [SD-07.04 · #78](https://github.com/PhoNoodles/system-design-learning/issues/78) | Explicit reusable-object keys, dependencies and granularity tradeoffs. |
| [When to update the cache](https://github.com/donnemartin/system-design-primer#when-to-update-the-cache) | [SD-07.05 · #79](https://github.com/PhoNoodles/system-design-learning/issues/79), [SD-07.06 · #80](https://github.com/PhoNoodles/system-design-learning/issues/80), [SD-07.07 · #81](https://github.com/PhoNoodles/system-design-learning/issues/81), [SD-07.09 · #83](https://github.com/PhoNoodles/system-design-learning/issues/83) | Compare update and invalidation strategies using freshness and failure requirements. |
| [Cache-aside](https://github.com/donnemartin/system-design-primer#cache-aside) | [SD-07.05 · #79](https://github.com/PhoNoodles/system-design-learning/issues/79) | Trace hits, misses, population, updates and races. |
| [Write-through](https://github.com/donnemartin/system-design-primer#write-through) | [SD-07.06 · #80](https://github.com/PhoNoodles/system-design-learning/issues/80) | Write-through is direct source coverage; read-through comparison is a course expansion. |
| [Write-behind / write-back](https://github.com/donnemartin/system-design-primer#write-behind-write-back) | [SD-07.07 · #81](https://github.com/PhoNoodles/system-design-learning/issues/81) | Write-back is direct source coverage; write-around comparison is a course expansion. |
| [Refresh-ahead](https://github.com/donnemartin/system-design-primer#refresh-ahead) | [SD-07.11 · #123](https://github.com/PhoNoodles/system-design-learning/issues/123) | A dedicated issue covers proactive refresh, prediction error, failed refreshes and origin load. |

### Asynchronous processing

| Primer topic / source | Canonical learning record | Coverage and scope |
| --- | --- | --- |
| [Asynchronism](https://github.com/donnemartin/system-design-primer#asynchronism) | [SD-05.05 · #51](https://github.com/PhoNoodles/system-design-learning/issues/51), [SD-08.01 · #85](https://github.com/PhoNoodles/system-design-learning/issues/85) | Separate deferred completion from immediate request/response behavior. |
| [Message queues](https://github.com/donnemartin/system-design-primer#message-queues) | [SD-08.01 · #85](https://github.com/PhoNoodles/system-design-learning/issues/85) | Trace producer, broker and worker responsibilities and buffering costs. |
| [Task queues](https://github.com/donnemartin/system-design-primer#task-queues) | [SD-08.01 · #85](https://github.com/PhoNoodles/system-design-learning/issues/85), [SD-08.05 · #89](https://github.com/PhoNoodles/system-design-learning/issues/89) | Relate scheduled execution to worker assignment; consumer-group details extend the source. |
| [Back pressure](https://github.com/donnemartin/system-design-primer#back-pressure) | [SD-08.08 · #92](https://github.com/PhoNoodles/system-design-learning/issues/92) | Assess arrival/service rates, bounded backlog and feedback or rejection policies. |

### Communication and security

| Primer topic / source | Canonical learning record | Coverage and scope |
| --- | --- | --- |
| [HTTP](https://github.com/donnemartin/system-design-primer#hypertext-transfer-protocol-http) | [SD-03.06 · #30](https://github.com/PhoNoodles/system-design-learning/issues/30), [SD-03.07 · #31](https://github.com/PhoNoodles/system-design-learning/issues/31) | HTTP semantics receive a lesson; newer-version behavior is labeled an expansion. |
| [TCP](https://github.com/donnemartin/system-design-primer#transmission-control-protocol-tcp) | [SD-03.03 · #27](https://github.com/PhoNoodles/system-design-learning/issues/27), [SD-03.04 · #28](https://github.com/PhoNoodles/system-design-learning/issues/28) | Compare transport semantics and trace connection, retransmission and congestion behavior. |
| [UDP](https://github.com/donnemartin/system-design-primer#user-datagram-protocol-udp) | [SD-03.03 · #27](https://github.com/PhoNoodles/system-design-learning/issues/27) | Compare datagrams with TCP and state the application responsibilities. |
| [RPC](https://github.com/donnemartin/system-design-primer#remote-procedure-call-rpc) | [SD-03.10 · #34](https://github.com/PhoNoodles/system-design-learning/issues/34) | RPC mechanics and failure tradeoffs are covered; gRPC specifics extend the source. |
| [REST](https://github.com/donnemartin/system-design-primer#representational-state-transfer-rest) | [SD-03.09 · #33](https://github.com/PhoNoodles/system-design-learning/issues/33) | Assess resource/representation design, HTTP semantics and stateless/cacheable interfaces. |
| [RPC and REST comparison](https://github.com/donnemartin/system-design-primer#rpc-and-rest-calls-comparison) | [SD-03.09 · #33](https://github.com/PhoNoodles/system-design-learning/issues/33), [SD-03.10 · #34](https://github.com/PhoNoodles/system-design-learning/issues/34) | Compare contracts, coupling, failure handling and client needs. |
| [Security](https://github.com/donnemartin/system-design-primer#security) | [SD-09.05 · #99](https://github.com/PhoNoodles/system-design-learning/issues/99), [SD-09.06 · #100](https://github.com/PhoNoodles/system-design-learning/issues/100), [SD-09.08 · #102](https://github.com/PhoNoodles/system-design-learning/issues/102) | The source directly covers encryption, least privilege and input/injection controls; the broader security curriculum is explicitly expanded. |

### Appendix, source directories and developing topics

| Primer topic / source | Canonical learning record | Coverage and scope |
| --- | --- | --- |
| [Powers of two table](https://github.com/donnemartin/system-design-primer#powers-of-two-table) | [SD-10.02 · #106](https://github.com/PhoNoodles/system-design-learning/issues/106), [SD-01.07 · #7](https://github.com/PhoNoodles/system-design-learning/issues/7) | Includes powers of two and binary versus decimal units in capacity estimates. |
| [Latency reference table and visualization](https://github.com/donnemartin/system-design-primer#latency-numbers-every-programmer-should-know) | [SD-01.02 · #2](https://github.com/PhoNoodles/system-design-learning/issues/2), [SD-01.07 · #7](https://github.com/PhoNoodles/system-design-learning/issues/7), [SD-10.02 · #106](https://github.com/PhoNoodles/system-design-learning/issues/106) | Use historical numbers for rough relative scale, with explicit workload/hardware assumptions; current guarantees require current evidence. |
| [Additional system design questions](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [All 23 prompt mappings](#additional-practice-questions) | Every one of the 23 named prompts is mapped in the additional-practice table below; shared variants retain distinct evidence where their scope differs. |
| [Real world architectures](https://github.com/donnemartin/system-design-primer#real-world-architectures) | [SD-14.01 · #149](https://github.com/PhoNoodles/system-design-learning/issues/149) | Optional selected-paper comparison. Completion applies only to the named papers studied, not the entire bibliography. |
| [Company architectures](https://github.com/donnemartin/system-design-primer#company-architectures) | [SD-14.02 · #150](https://github.com/PhoNoodles/system-design-learning/issues/150) | Optional selected company architecture study with documented requirements and tradeoffs. |
| [Company engineering blogs](https://github.com/donnemartin/system-design-primer#company-engineering-blogs) | [SD-14.02 · #150](https://github.com/PhoNoodles/system-design-learning/issues/150) | Optional first-party engineering case study; record source, date, measured problem and what can transfer to another workload. |
| [Under development: consistent hashing, MapReduce, scatter-gather](https://github.com/donnemartin/system-design-primer#under-development) | [SD-11.07 · #120](https://github.com/PhoNoodles/system-design-learning/issues/120), [SD-11.03 · #116](https://github.com/PhoNoodles/system-design-learning/issues/116), [SD-11.05 · #118](https://github.com/PhoNoodles/system-design-learning/issues/118) | Explicit expansions: MapReduce in sales ranking, consistent hashing as its own lesson, and scatter-gather in search. The source marks these topics under development. |

## Worked system-design examples

All eight worked examples in the source are represented in the main track. Their sample architectures provide material to critique and compare after an independent attempt; they are not the only valid solutions. Reusable concepts are recorded in their own lessons so later design practice can focus on applying them.

| Worked source example | Canonical issue | Assessed scope |
| --- | --- | --- |
| [Pastebin / URL shortener](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/pastebin/README.md) | [SD-10.05 · #108](https://github.com/PhoNoodles/system-design-learning/issues/108) | Identifier allocation, collisions, create/read flow, caching, storage and abuse constraints; distinguish redirects from stored pastes. |
| [Timeline and search](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/twitter/README.md) | [SD-10.06 · #109](https://github.com/PhoNoodles/system-design-learning/issues/109) | Posting, user timeline, home/news feed, high-follower fan-out, keyword indexing and search freshness. |
| [Web crawler](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/web_crawler/README.md) | [SD-10.07 · #110](https://github.com/PhoNoodles/system-design-learning/issues/110) | Frontier scheduling, fetching, parsing, deduplication, host politeness and scalable worker capacity. |
| [Mint financial aggregation](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/mint/README.md) | [SD-10.11 · #124](https://github.com/PhoNoodles/system-design-learning/issues/124) | Mock account/transaction ingestion, categorization overrides, monthly aggregates, duplicate imports and delayed notifications. |
| [Social-network data structures](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/social_graph/README.md) | [SD-10.12 · #125](https://github.com/PhoNoodles/system-design-learning/issues/125) | Unweighted shortest paths, adjacency data, sharded lookup, high-degree nodes and missing partitions. |
| [Key-value query-result cache](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/query_cache/README.md) | [SD-10.08 · #111](https://github.com/PhoNoodles/system-design-learning/issues/111) | Bounded query-result caching, hit/miss paths, LRU-style eviction, distribution, node loss and a reusable cache API. |
| [Sales ranking](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/sales_rank/README.md) | [SD-11.07 · #120](https://github.com/PhoNoodles/system-design-learning/issues/120) | Category rankings through multi-stage MapReduce, serving, time windows, freshness and late/duplicate events. |
| [Scale to millions on AWS](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/scaling_aws/README.md) | [SD-11.08 · #121](https://github.com/PhoNoodles/system-design-learning/issues/121) | Incremental scaling from measured bottlenecks, with availability, deployment and cost tradeoffs. |

## Object-oriented exercises

This is an **optional** track. The source labels the overall OOD section as under development, but provides six linked solution notebooks. Those six notebooks were present at review. Each exercise records its own design and implementation evidence.

| Source exercise | Canonical issue | Coverage and source status |
| --- | --- | --- |
| [Hash map](https://github.com/donnemartin/system-design-primer/blob/master/solutions/object_oriented_design/hash_table/hash_map.ipynb) | [SD-12.01 · #126](https://github.com/PhoNoodles/system-design-learning/issues/126) | Hashing, collisions, updates, deletion, resizing and operation costs. |
| [LRU cache](https://github.com/donnemartin/system-design-primer/blob/master/solutions/object_oriented_design/lru_cache/lru_cache.ipynb) | [SD-12.02 · #127](https://github.com/PhoNoodles/system-design-learning/issues/127) | Lookup plus recency structures, capacity invariants and eviction. |
| [Call center](https://github.com/donnemartin/system-design-primer/blob/master/solutions/object_oriented_design/call_center/call_center.ipynb) | [SD-12.03 · #128](https://github.com/PhoNoodles/system-design-learning/issues/128) | Calls, employee roles, assignment, escalation and state transitions. |
| [Deck of cards](https://github.com/donnemartin/system-design-primer/blob/master/solutions/object_oriented_design/deck_of_cards/deck_of_cards.ipynb) | [SD-12.04 · #129](https://github.com/PhoNoodles/system-design-learning/issues/129) | Card/deck/hand responsibilities, shuffling, drawing and game-rule separation. |
| [Parking lot](https://github.com/donnemartin/system-design-primer/blob/master/solutions/object_oriented_design/parking_lot/parking_lot.ipynb) | [SD-12.05 · #130](https://github.com/PhoNoodles/system-design-learning/issues/130) | Vehicles, spot constraints, allocation, entry/exit and capacity. |
| [Chat server](https://github.com/donnemartin/system-design-primer/blob/master/solutions/object_oriented_design/online_chat/online_chat.ipynb) | [SD-12.06 · #131](https://github.com/PhoNoodles/system-design-learning/issues/131) | User, conversation, message and session responsibilities; distinct from the distributed chat architecture exercise. |
| [Circular array entry](https://github.com/donnemartin/system-design-primer#object-oriented-design-interview-questions-with-solutions) | [SD-12.07 · #132](https://github.com/PhoNoodles/system-design-learning/issues/132) | Upstream contribution placeholder with no supplied solution. This optional course extension covers logical rotation, indexing and iteration. |

## Additional practice questions

The source names **23 additional prompts**. They map to **16 new optional exercises** plus relevant existing main lessons. Two chat prompts share one optional issue, and the feed/timeline variants share the worked social-system issue. Reuse does not collapse distinct requirements: record the variant and its assessed evidence in the mapped issue. A broad conceptual lesson is not treated as a complete system-design exercise unless its objectives include that design scope.

The source list supplies starting references rather than a complete solution for every problem. Optional exercise objectives are original course material. Choose these exercises deliberately after the relevant prerequisites; the main track does not depend on completing an optional issue.

| Named source prompt | Canonical issue | Track | Coverage and variant handling |
| --- | --- | --- | --- |
| [Design a file sync service like Dropbox](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.01 · #133](https://github.com/PhoNoodles/system-design-learning/issues/133) | Optional | Optional design exercise; design metadata, file/chunk identity, change detection, upload/download and resumable transfer. |
| [Design a search engine like Google](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.02 · #134](https://github.com/PhoNoodles/system-design-learning/issues/134) | Optional | Optional design exercise; connect crawling, document storage, parsing, indexing and query serving. |
| [Design a scalable web crawler like Google](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-10.07 · #110](https://github.com/PhoNoodles/system-design-learning/issues/110) | Main | Covered by the existing scalable crawler exercise; record the chosen workload and constraints. |
| [Design Google docs](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.03 · #135](https://github.com/PhoNoodles/system-design-learning/issues/135) | Optional | Optional design exercise; define document operations, versioning, membership and collaboration semantics. |
| [Design a key-value store like Redis](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.04 · #136](https://github.com/PhoNoodles/system-design-learning/issues/136) | Optional | Optional authoritative storage design; explicitly distinct from disposable query caching. |
| [Design a cache system like Memcached](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-10.08 · #111](https://github.com/PhoNoodles/system-design-learning/issues/111) | Main | The existing query-cache issue includes a generic distributed-cache interface, key placement, eviction, node loss and hot keys. |
| [Design a recommendation system like Amazon's](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.05 · #137](https://github.com/PhoNoodles/system-design-learning/issues/137) | Optional | Optional design exercise; define users/items/events and a basic recommendation objective with cold-start behavior. |
| [Design a tinyurl system like Bitly](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-10.05 · #108](https://github.com/PhoNoodles/system-design-learning/issues/108) | Main | Covered by the existing short-link variant; distinguish it from a stored-paste variant. |
| [Design a chat app like WhatsApp](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.06 · #138](https://github.com/PhoNoodles/system-design-learning/issues/138) | Optional | Optional design exercise; define direct/group chat, message IDs, ordering, acknowledgement and delivery/read semantics. |
| [Design a picture sharing system like Instagram](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.07 · #139](https://github.com/PhoNoodles/system-design-learning/issues/139) | Optional | Optional design exercise; design authenticated media upload, metadata storage and background processing. |
| [Design the Facebook news feed function](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-10.06 · #109](https://github.com/PhoNoodles/system-design-learning/issues/109) | Main | Home/news feed requirements are explicitly included in the social timeline and search issue. |
| [Design the Facebook timeline function](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-10.06 · #109](https://github.com/PhoNoodles/system-design-learning/issues/109) | Main | User/profile timeline requirements are separately included in the same social-system issue. |
| [Design the Facebook chat function](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.06 · #138](https://github.com/PhoNoodles/system-design-learning/issues/138) | Optional | Shares the chat issue with the WhatsApp-style prompt; record the product variant and any changed requirements. |
| [Design a graph search function like Facebook's](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.08 · #140](https://github.com/PhoNoodles/system-design-learning/issues/140) | Optional | Optional graph query/index/ranking design; broader than the main shortest-path traversal exercise. |
| [Design a content delivery network like CloudFlare](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.09 · #141](https://github.com/PhoNoodles/system-design-learning/issues/141) | Optional | Optional end-to-end CDN architecture; expands the main cache and push/pull strategy lessons. |
| [Design a trending topic system like Twitter's](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.10 · #142](https://github.com/PhoNoodles/system-design-learning/issues/142) | Optional | Optional design exercise; define a trend metric, event-time windows and acceptable freshness. |
| [Design a random ID generation system](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.11 · #143](https://github.com/PhoNoodles/system-design-learning/issues/143) | Optional | Optional design exercise; define uniqueness, sortability, unpredictability and allocation-rate requirements. |
| [Return the top k requests during a time interval](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.12 · #144](https://github.com/PhoNoodles/system-design-learning/issues/144) | Optional | Optional design exercise; define event time, window type, exact/approximate results and permitted error. |
| [Design a system that serves data from multiple data centers](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.13 · #145](https://github.com/PhoNoodles/system-design-learning/issues/145) | Optional | Optional design exercise; define regional latency, availability, residency and recovery requirements. |
| [Design an online multiplayer card game](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.14 · #146](https://github.com/PhoNoodles/system-design-learning/issues/146) | Optional | Optional design exercise; define authoritative game state, legal moves, turn ordering and matchmaking. |
| [Design a garbage collection system](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.15 · #147](https://github.com/PhoNoodles/system-design-learning/issues/147) | Optional | Optional design exercise; define the object graph, roots, reachability and reclamation requirements. |
| [Design an API rate limiter](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-04.08 · #44](https://github.com/PhoNoodles/system-design-learning/issues/44) | Main | The main rate-limiter issue includes a complete distributed scenario: keys, concurrent counters, clocks, allowed overshoot and store failure. |
| [Design a Stock Exchange (like NASDAQ or Binance)](https://github.com/donnemartin/system-design-primer#additional-system-design-interview-questions) | [SD-13.16 · #148](https://github.com/PhoNoodles/system-design-learning/issues/148) | Optional | Optional design exercise; define order entry, price-time priority, matching, cancellation and acknowledgements using synthetic orders. |

## Supplemental lessons and original assessments

The Primer is the foundation, not a claim that every course topic appears as a full upstream lesson. The following remaining lessons extend the source or add explicit assessments. Mixed lessons already mapped above also identify their expansions in the issue body. The complete source classification for every lesson is maintained in the curriculum and its issue.

| Canonical issue | Subject | Classification | Scope |
| --- | --- | --- | --- |
| [SD-01.05 · #5](https://github.com/PhoNoodles/system-design-learning/issues/5) | CPU-bound vs I/O-bound workloads | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-01.06 · #6](https://github.com/PhoNoodles/system-design-learning/issues/6) | Availability vs reliability | mixed | The Primer quantifies availability; reliability definitions and success criteria are supplemental. CAP availability is a different formal property, covered in SD-02.01. |
| [SD-02.06 · #14](https://github.com/PhoNoodles/system-design-learning/issues/14) | Read-your-writes and session consistency | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-02.11 · #21](https://github.com/PhoNoodles/system-design-learning/issues/21) | Quorums | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-02.13 · #23](https://github.com/PhoNoodles/system-design-learning/issues/23) | Timeouts and retry safety | extension | Conceptual retry safety precedes HTTP-specific idempotency and the implementation detail in SD-05.06. |
| [SD-03.01 · #25](https://github.com/PhoNoodles/system-design-learning/issues/25) | OSI and TCP/IP models | mixed | The Primer includes an OSI diagram; detailed layer mapping and troubleshooting are supplemental. |
| [SD-03.02 · #26](https://github.com/PhoNoodles/system-design-learning/issues/26) | IP addressing and routing | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-03.08 · #32](https://github.com/PhoNoodles/system-design-learning/issues/32) | TLS and HTTPS | extension | The Primer mentions SSL/TLS termination and encryption but does not provide this TLS lesson. |
| [SD-03.11 · #35](https://github.com/PhoNoodles/system-design-learning/issues/35) | WebSockets and server-sent events | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-04.09 · #45](https://github.com/PhoNoodles/system-design-learning/issues/45) | API gateways | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-05.06 · #52](https://github.com/PhoNoodles/system-design-learning/issues/52) | Idempotency | mixed | The Primer introduces HTTP method idempotency; application keys and atomic deduplication are supplemental. Database atomicity is revisited in SD-06.02 and consumer deduplication in SD-08.07. |
| [SD-05.07 · #53](https://github.com/PhoNoodles/system-design-learning/issues/53) | Circuit breakers | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-05.08 · #54](https://github.com/PhoNoodles/system-design-learning/issues/54) | Bulkheads and isolation | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-05.09 · #55](https://github.com/PhoNoodles/system-design-learning/issues/55) | Observability: logs metrics traces | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-05.10 · #56](https://github.com/PhoNoodles/system-design-learning/issues/56) | Configuration and feature flags | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-05.11 · #57](https://github.com/PhoNoodles/system-design-learning/issues/57) | Deployment strategies | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-06.03 · #61](https://github.com/PhoNoodles/system-design-learning/issues/61) | Isolation levels and anomalies | extension | Specific isolation guarantees vary by database and implementation; use the chosen engine's current documentation when teaching the concrete example. |
| [SD-06.06 · #64](https://github.com/PhoNoodles/system-design-learning/issues/64) | Connection pooling | mixed | The Primer mentions connection pooling in its TCP discussion; database pool sizing and transaction lifecycle are supplemental. |
| [SD-08.02 · #86](https://github.com/PhoNoodles/system-design-learning/issues/86) | Publish-subscribe and event streams | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-08.03 · #87](https://github.com/PhoNoodles/system-design-learning/issues/87) | Delivery guarantees | mixed | The Primer introduces reliable queue delivery; precise delivery and processing guarantees are an extension. |
| [SD-08.04 · #88](https://github.com/PhoNoodles/system-design-learning/issues/88) | Ordering and partition keys | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-08.06 · #90](https://github.com/PhoNoodles/system-design-learning/issues/90) | Retries and dead-letter queues | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-08.07 · #91](https://github.com/PhoNoodles/system-design-learning/issues/91) | Idempotent consumers and deduplication | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-08.09 · #93](https://github.com/PhoNoodles/system-design-learning/issues/93) | Transactional outbox and sagas | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-09.01 · #95](https://github.com/PhoNoodles/system-design-learning/issues/95) | Authentication vs authorization | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-09.02 · #96](https://github.com/PhoNoodles/system-design-learning/issues/96) | Sessions and cookies | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-09.03 · #97](https://github.com/PhoNoodles/system-design-learning/issues/97) | JWT and token lifecycle | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-09.04 · #98](https://github.com/PhoNoodles/system-design-learning/issues/98) | OAuth 2.0 and OpenID Connect | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-09.07 · #101](https://github.com/PhoNoodles/system-design-learning/issues/101) | Secrets management | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-09.09 · #103](https://github.com/PhoNoodles/system-design-learning/issues/103) | Threat modeling and tenant isolation | extension | Original practical engineering lesson; select current primary reading at teaching time. |
| [SD-10.09 · #112](https://github.com/PhoNoodles/system-design-learning/issues/112) | Design SAP-to-MES manufacturing integration | extension | This applied SAP/MES exercise is personalized supplemental material. |
| [SD-11.02 · #115](https://github.com/PhoNoodles/system-design-learning/issues/115) | Object storage and distributed files | mixed | The Primer links GFS/HDFS reference architectures; object-store details extend that reading. |
| [SD-11.04 · #117](https://github.com/PhoNoodles/system-design-learning/issues/117) | Distributed coordination and consensus | mixed | The Primer links Chubby/ZooKeeper; consensus mechanisms require primary supplemental reading. |
| [SD-11.06 · #119](https://github.com/PhoNoodles/system-design-learning/issues/119) | Disaster recovery RPO and RTO | extension | Original practical engineering lesson; select current primary reading at teaching time. |

### Assessment coverage

| Canonical issue | Assessment | Completion boundary |
| --- | --- | --- |
| [SD-01.08 · #8](https://github.com/PhoNoodles/system-design-learning/issues/8) | Fundamentals assessment | Original assessment. Independent evidence and essential objectives are required; a high-level topic mapping is not completion. |
| [SD-02.14 · #24](https://github.com/PhoNoodles/system-design-learning/issues/24) | Distributed systems assessment | Original assessment. Independent evidence and essential objectives are required; a high-level topic mapping is not completion. |
| [SD-03.12 · #36](https://github.com/PhoNoodles/system-design-learning/issues/36) | Networking assessment | Original assessment. Independent evidence and essential objectives are required; a high-level topic mapping is not completion. |
| [SD-04.10 · #46](https://github.com/PhoNoodles/system-design-learning/issues/46) | Traffic management assessment | Original assessment. Independent evidence and essential objectives are required; a high-level topic mapping is not completion. |
| [SD-05.12 · #58](https://github.com/PhoNoodles/system-design-learning/issues/58) | Application architecture assessment | Original assessment. Independent evidence and essential objectives are required; a high-level topic mapping is not completion. |
| [SD-06.16 · #74](https://github.com/PhoNoodles/system-design-learning/issues/74) | SQL vs NoSQL tradeoffs and assessment | Original assessment. Independent evidence and essential objectives are required; a high-level topic mapping is not completion. |
| [SD-07.10 · #84](https://github.com/PhoNoodles/system-design-learning/issues/84) | Caching assessment | Original assessment. Independent evidence and essential objectives are required; a high-level topic mapping is not completion. |
| [SD-08.10 · #94](https://github.com/PhoNoodles/system-design-learning/issues/94) | Asynchronous processing assessment | Original assessment. Independent evidence and essential objectives are required; a high-level topic mapping is not completion. |
| [SD-09.10 · #104](https://github.com/PhoNoodles/system-design-learning/issues/104) | Security assessment | Original assessment. Independent evidence and essential objectives are required; a high-level topic mapping is not completion. |
| [SD-10.10 · #113](https://github.com/PhoNoodles/system-design-learning/issues/113) | Full mock interview and tradeoff defense | Original assessment. Independent evidence and essential objectives are required; a high-level topic mapping is not completion. |

## Deliberate exclusions and review boundaries

| Upstream material | How it is handled |
| --- | --- |
| Motivation and interview-preparation introduction | Reflected in the course purpose and orientation; no separate mastery issue. |
| Translation links and translation requests | Navigation/accessibility resources, not system-design competencies. |
| Contributing instructions, requests to add questions and project-maintenance directions | Administrative source material; not learner assignments. |
| Index and repeated navigation links | Represented by the substantive topic mappings above. |
| Sister repository for coding interview challenges | A separate resource outside this course's system-design scope. It does not create an unrequested coding-interview track. |
| Credits, contact information and license | Preserved as attribution and licensing context, not teaching topics. |
| Every external paper, article, company architecture, blog post and video in a directory | A source bank for selected reading. Its existence does not imply link freshness, factual validation, required completion or learner mastery. |

All educational source sections are accounted for at the section/topic level. Additional resources can be selected during a lesson and recorded in its issue without duplicating already demonstrated fundamentals. If the upstream source changes, update this map and the affected issue scopes; do not silently convert an earlier assessment into evidence for new objectives.

## Attribution and original course material

The source is **The System Design Primer by Donne Martin**, provided under the **Creative Commons Attribution 4.0 International license (CC BY 4.0)**. See the [upstream license statement](https://github.com/donnemartin/system-design-primer#license) and [license terms](https://creativecommons.org/licenses/by/4.0/).

This learning repository reorganizes and links the source, uses updated terminology where helpful, and adds original lesson objectives, exercises, assessments, progress rules and practical expansions. It does not reproduce the Primer's solution collection or present those solutions as original work. Attribution and exact reading links should remain attached when source material is discussed in a learning record.
