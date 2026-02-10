

# MASTERING SYSTEM DESIGN: COMPLETE 25-PHASE SYLLABUS

## Course Overview
**Total Duration:** 25 Phases | **Goal:** Master System Design from fundamentals to interview success

---

## **PHASE 1: FOUNDATIONS & COURSE ORIENTATION**
**Duration:** Week 1 | **Lectures:** 6

### Topics Covered:
1. **What is System Design?**
   - Definition and scope
   - Difference between low-level and high-level design
   - Real-world applications

2. **Why System Design Matters**
   - Industry relevance
   - Career progression
   - Interview importance at FAANG companies

3. **Evolution of System Design (Last 25 Years)**
   - Monolithic to microservices journey
   - Cloud computing revolution
   - Modern distributed systems

4. **Course Structure & Navigation**
   - Learning path overview
   - Best practices for self-study
   - Resource utilization

### Key Concepts:
- System design vs. software design
- Scalability fundamentals
- Distributed computing basics

### Best Practices:
- Set up a learning journal
- Create a GitHub repository for notes
- Join system design communities (Reddit, Discord)

### Practice Problems:
1. Explain system design in your own words
2. Research and document one major system architecture change in the last decade
3. Create a personal learning roadmap

---

## **PHASE 2: NETWORKING FUNDAMENTALS - PART 1**
**Duration:** Week 1-2 | **Lectures:** 4

### Topics Covered:
1. **Introduction to Networking in System Design**
   - OSI Model overview
   - TCP/IP stack
   - Network protocols hierarchy

2. **IP Addresses Deep Dive**
   - IPv4 vs IPv6
   - Public vs Private IPs
   - Subnetting basics
   - NAT (Network Address Translation)

3. **DNS (Domain Name System)**
   - DNS resolution process
   - DNS hierarchy (Root, TLD, Authoritative)
   - DNS caching
   - DNS records (A, AAAA, CNAME, MX, TXT)
   - Round-robin DNS

4. **Client-Server Model**
   - Request-response cycle
   - Stateful vs stateless connections
   - Connection pooling
   - Keep-alive mechanisms

### Key Concepts:
- Latency and bandwidth
- Network hops
- DNS propagation
- IP addressing schemes

### Best Practices:
- Use `dig` and `nslookup` commands
- Analyze network traffic with Wireshark
- Understand your application's network flow

### Practice Problems:
1. Trace a DNS lookup for google.com
2. Calculate subnet masks for different network sizes
3. Diagram the client-server flow for a web request

### Subtopics to Master:
- DNS TTL (Time to Live)
- Anycast vs Unicast vs Multicast
- Network latency calculations
- Three-way handshake

---

## **PHASE 3: NETWORKING FUNDAMENTALS - PART 2**
**Duration:** Week 2 | **Lectures:** 4

### Topics Covered:
1. **Forward Proxy vs Reverse Proxy**
   - **Forward Proxy:**
     - Client-side proxy
     - Anonymity and caching
     - Use cases (corporate networks, VPNs)
   
   - **Reverse Proxy:**
     - Server-side proxy
     - Load distribution
     - SSL termination
     - Examples: Nginx, HAProxy

2. **Load Balancing Introduction**
   - Why load balancing is needed
   - Load balancer types (L4 vs L7)
   - Load balancing algorithms:
     - Round Robin
     - Least Connections
     - IP Hash
     - Weighted Round Robin
     - Least Response Time
   - Health checks and failover

3. **API Gateway**
   - Centralized entry point
   - Request routing
   - Authentication/Authorization
   - Rate limiting
   - API composition
   - Popular gateways: Kong, AWS API Gateway, Azure APIM

4. **Content Delivery Networks (CDN)**
   - CDN architecture
   - Edge locations and PoPs
   - Caching strategies
   - Cache invalidation
   - Popular CDNs: CloudFlare, Akamai, AWS CloudFront
   - Push vs Pull CDNs

### Key Concepts:
- SSL/TLS termination
- Session persistence (sticky sessions)
- Cache hit ratio
- Edge computing

### Best Practices:
- Always use CDN for static assets
- Implement proper cache headers
- Monitor load balancer health
- Use API gateway for microservices

### Practice Problems:
1. Design a load balancing strategy for 1M daily users
2. Calculate CDN cost savings for a global application
3. Configure Nginx as a reverse proxy (hands-on)
4. Implement rate limiting in an API gateway

### Subtopics to Master:
- Geographic load balancing
- Active-active vs active-passive configurations
- CDN cache purging strategies
- API versioning through gateways

---

## **PHASE 4: COMMUNICATION PROTOCOLS - PART 1**
**Duration:** Week 3 | **Lectures:** 3

### Topics Covered:
1. **TCP & UDP**
   - **TCP (Transmission Control Protocol):**
     - Connection-oriented
     - Reliability guarantees
     - Flow control and congestion control
     - Use cases: HTTP, FTP, email
   
   - **UDP (User Datagram Protocol):**
     - Connectionless
     - Low latency
     - No reliability guarantees
     - Use cases: video streaming, gaming, DNS

2. **HTTP - The Backbone of the Web**
   - HTTP/1.0 vs HTTP/1.1 vs HTTP/2 vs HTTP/3
   - Request methods: GET, POST, PUT, DELETE, PATCH
   - Status codes: 2xx, 3xx, 4xx, 5xx
   - Headers (Request & Response)
   - Cookies and sessions
   - HTTPS and SSL/TLS
   - Connection management

3. **REST & RESTfulness**
   - REST principles:
     - Statelessness
     - Client-server separation
     - Cacheability
     - Uniform interface
     - Layered system
   - Resource-based URLs
   - HATEOAS
   - REST best practices
   - Idempotency
   - Versioning strategies

### Key Concepts:
- Keep-alive connections
- Multiplexing (HTTP/2)
- QUIC protocol (HTTP/3)
- RESTful API design patterns

### Best Practices:
- Use appropriate HTTP methods
- Implement proper error handling
- Version your APIs
- Use HTTPS everywhere
- Implement rate limiting

### Practice Problems:
1. Design a RESTful API for a blog platform
2. Compare TCP vs UDP for video conferencing
3. Analyze HTTP/2 multiplexing benefits
4. Create API documentation using OpenAPI/Swagger

### Subtopics to Master:
- Content negotiation
- CORS (Cross-Origin Resource Sharing)
- HTTP caching strategies (ETag, Cache-Control)
- WebSockets for bidirectional communication

---

## **PHASE 5: COMMUNICATION PROTOCOLS - PART 2**
**Duration:** Week 3-4 | **Lectures:** 3

### Topics Covered:
1. **Real-Time Communication Protocols**
   - **WebSockets:**
     - Full-duplex communication
     - Persistent connections
     - Use cases: chat, live updates
   
   - **Server-Sent Events (SSE):**
     - Unidirectional server-to-client
     - Auto-reconnection
     - Use cases: notifications, feeds
   
   - **Long Polling:**
     - HTTP-based real-time simulation
     - Limitations
   
   - **WebRTC:**
     - Peer-to-peer communication
     - Video/audio streaming

2. **Modern API Protocols - Beyond REST**
   - **GraphQL:**
     - Query language for APIs
     - Single endpoint
     - Client-specified queries
     - Over-fetching/under-fetching solutions
   
   - **gRPC:**
     - Protocol Buffers
     - HTTP/2 based
     - Bi-directional streaming
     - Performance benefits
   
   - **SOAP:**
     - Legacy protocol
     - XML-based
     - Enterprise use cases

### Key Concepts:
- Protocol selection criteria
- Latency requirements
- Bandwidth considerations
- Browser compatibility

### Best Practices:
- Choose protocols based on use case
- Implement fallback mechanisms
- Monitor connection health
- Handle reconnection gracefully

### Practice Problems:
1. Build a chat application using WebSockets
2. Compare REST vs GraphQL for a mobile app
3. Implement a notification system with SSE
4. Design a video conferencing system architecture

### Subtopics to Master:
- WebSocket scaling challenges
- GraphQL schema design
- gRPC service definitions
- Protocol Buffers vs JSON

---

## **PHASE 6: ARCHITECTURAL PATTERNS**
**Duration:** Week 4 | **Lectures:** 4

### Topics Covered:
1. **Software Architecture Patterns & Styles**
   - Layered Architecture
   - Clean Architecture
   - Hexagonal Architecture (Ports & Adapters)
   - Onion Architecture
   - CQRS (Command Query Responsibility Segregation)
   - Saga Pattern

2. **Multi-Tier Architecture**
   - **Presentation Tier:**
     - User interface
     - Client-side logic
   
   - **Application Tier:**
     - Business logic
     - Processing layer
   
   - **Data Tier:**
     - Database layer
     - Data persistence
   
   - **N-Tier variations:**
     - 2-tier vs 3-tier vs N-tier
     - Pros and cons

3. **Microservices Architecture**
   - Service decomposition
   - Domain-Driven Design (DDD)
   - Service boundaries
   - Inter-service communication
   - Service discovery
   - API gateway pattern
   - Database per service
   - Shared database anti-pattern
   - Circuit breaker pattern
   - Bulkhead pattern
   
   - **Microservices vs Monolith:**
     - When to use each
     - Migration strategies

4. **Event-Driven Architecture**
   - Event producers and consumers
   - Event bus/broker
   - Event sourcing
   - Event streaming (Kafka, RabbitMQ)
   - Publish-Subscribe pattern
   - Message queues
   - Asynchronous processing

### Key Concepts:
- Bounded contexts
- Service mesh (Istio, Linkerd)
- Choreography vs Orchestration
- Eventual consistency

### Best Practices:
- Start monolith, evolve to microservices
- Define clear service boundaries
- Implement proper monitoring
- Use API versioning
- Design for failure

### Practice Problems:
1. Decompose a monolithic e-commerce app into microservices
2. Design an event-driven order processing system
3. Compare CQRS vs traditional CRUD
4. Create a service dependency map for a complex system

### Subtopics to Master:
- Service mesh architecture
- Strangler fig pattern (migration)
- Backends for Frontends (BFF)
- Distributed tracing

---

## **PHASE 7: WEB CONCEPTS & FUNDAMENTALS**
**Duration:** Week 5 | **Lectures:** 4

### Topics Covered:
1. **Web Sessions: Managing State**
   - Stateless HTTP challenge
   - Session management strategies:
     - Cookies
     - Session tokens
     - JWT (JSON Web Tokens)
     - OAuth tokens
   - Session storage:
     - Client-side
     - Server-side
     - Distributed sessions (Redis)
   - Session expiration and renewal
   - Session hijacking prevention

2. **Serialization: Data Exchange & Storage**
   - **Serialization formats:**
     - JSON (human-readable, widely supported)
     - XML (verbose, legacy systems)
     - Protocol Buffers (efficient, binary)
     - Avro (schema evolution)
     - MessagePack (binary JSON)
   
   - **When to use each:**
     - API responses: JSON
     - High-performance: Protobuf
     - Big data: Avro
   
   - Schema evolution
   - Backward/forward compatibility

3. **CORS: Cross-Origin Resource Sharing**
   - Same-origin policy
   - CORS headers:
     - Access-Control-Allow-Origin
     - Access-Control-Allow-Methods
     - Access-Control-Allow-Headers
   - Preflight requests (OPTIONS)
   - Security implications
   - CORS vs JSONP

### Key Concepts:
- Stateful vs stateless design
- Token-based authentication
- Content type negotiation
- Security headers

### Best Practices:
- Use HTTPOnly and Secure flags for cookies
- Implement CSRF protection
- Choose appropriate serialization format
- Configure CORS restrictively
- Use distributed session stores for scalability

### Practice Problems:
1. Implement JWT-based authentication
2. Design a session management system for 10M users
3. Compare JSON vs Protobuf performance
4. Configure CORS for a microservices architecture

### Subtopics to Master:
- SameSite cookie attribute
- Token refresh strategies
- Schema registry (for Avro/Protobuf)
- XSS and CSRF prevention

---

## **PHASE 8: SCALABILITY - CORE CONCEPTS**
**Duration:** Week 5-6 | **Lectures:** 4

### Topics Covered:
1. **Introduction to Scalability**
   - **What is scalability?**
     - Handling increased load
     - Performance metrics (throughput, latency)
   
   - **Scalability dimensions:**
     - User scalability
     - Data scalability
     - Geographic scalability
   
   - **Bottlenecks:**
     - CPU-bound
     - Memory-bound
     - I/O-bound
     - Network-bound

2. **Scaling Strategies**
   - **Vertical Scaling (Scale Up):**
     - Add more resources to single machine
     - Pros: Simple, no code changes
     - Cons: Hardware limits, single point of failure
     - Cost implications
   
   - **Horizontal Scaling (Scale Out):**
     - Add more machines
     - Pros: Infinite scaling, fault tolerance
     - Cons: Complexity, distributed systems challenges
     - Stateless design requirements
   
   - **Diagonal Scaling:**
     - Combination of vertical and horizontal
     - Use cases

3. **Load Balancers Deep Dive**
   - **Types:**
     - Hardware vs Software
     - Layer 4 (Transport) vs Layer 7 (Application)
   
   - **Algorithms:**
     - Round Robin
     - Weighted Round Robin
     - Least Connections
     - IP Hash
     - Least Response Time
     - Geo-based
   
   - **Cloud Solutions:**
     - AWS ELB/ALB/NLB
     - Azure Load Balancer
     - Google Cloud Load Balancing
   
   - **Advanced concepts:**
     - Health checks
     - Session affinity (sticky sessions)
     - SSL offloading
     - Connection draining

4. **Autoscaling & Best Practices**
   - **Autoscaling strategies:**
     - Reactive (metric-based)
     - Predictive (ML-based)
     - Scheduled
   
   - **Scaling metrics:**
     - CPU utilization
     - Memory usage
     - Request rate
     - Custom metrics
   
   - **Best practices:**
     - Stateless application design
     - Health check implementation
     - Graceful shutdown
     - Connection pooling
     - Caching strategies

### Key Concepts:
- Horizontal vs vertical scaling trade-offs
- Stateless vs stateful services
- Auto-scaling thresholds
- Load balancer health checks

### Best Practices:
- Design stateless services for horizontal scaling
- Implement proper health check endpoints
- Use connection pooling
- Monitor scaling metrics continuously
- Test auto-scaling policies

### Practice Problems:
1. Calculate infrastructure costs: vertical vs horizontal scaling
2. Design auto-scaling policy for e-commerce Black Friday
3. Compare L4 vs L7 load balancing for different scenarios
4. Implement health check endpoint for microservice

### Subtopics to Master:
- Blue-green deployment
- Canary releases
- Circuit breaker pattern implementation
- Scaling databases (covered in next phase)

---

## **PHASE 9: STORAGE SYSTEMS - PART 1**
**Duration:** Week 6-7 | **Lectures:** 4

### Topics Covered:
1. **Introduction to Storage & CAP Theorem**
   - **Storage requirements in distributed systems**
   - **CAP Theorem:**
     - **C**onsistency: All nodes see same data
     - **A**vailability: System always responds
     - **P**artition Tolerance: System works despite network failures
   
   - **Trade-offs:**
     - CP systems (Consistency + Partition Tolerance): HBase, MongoDB
     - AP systems (Availability + Partition Tolerance): Cassandra, DynamoDB
     - CA systems (Consistency + Availability): Traditional RDBMS (not truly distributed)
   
   - **PACELC Theorem:**
     - Extension of CAP
     - Latency considerations

2. **Database Models: SQL vs NoSQL**
   - **Relational Databases (SQL):**
     - ACID properties:
       - Atomicity
       - Consistency
       - Isolation
       - Durability
     - Schema-based
     - Joins and relationships
     - Examples: PostgreSQL, MySQL, Oracle
     - Use cases: Financial systems, transactions
   
   - **NoSQL Databases:**
     - **Document Stores:**
       - MongoDB, CouchDB
       - Flexible schema
       - JSON-like documents
       - Use cases: Content management, catalogs
     
     - **Key-Value Stores:**
       - Redis, DynamoDB
       - Simple key-value pairs
       - High performance
       - Use cases: Caching, sessions
     
     - **Column-Family Stores:**
       - Cassandra, HBase
       - Wide-column storage
       - Use cases: Time-series data, IoT
     
     - **Graph Databases:**
       - Neo4j, Amazon Neptune
       - Relationship-focused
       - Use cases: Social networks, recommendations
   
   - **NewSQL:**
     - Combines SQL and NoSQL benefits
     - Examples: CockroachDB, Google Spanner

### Key Concepts:
- ACID vs BASE (Basically Available, Soft state, Eventual consistency)
- Eventual consistency
- Strong consistency
- Read/write patterns

### Best Practices:
- Choose database based on data model
- Understand consistency requirements
- Plan for data growth
- Implement proper indexing

### Practice Problems:
1. Choose appropriate database for: social network, e-commerce, analytics
2. Design data model for SQL vs NoSQL for same use case
3. Analyze CAP trade-offs for a global application
4. Compare ACID vs eventual consistency for banking system

### Subtopics to Master:
- Database normalization (1NF, 2NF, 3NF, BCNF)
- Denormalization strategies
- Consistency models (strong, eventual, causal)
- Quorum consensus

---

## **PHASE 10: STORAGE SYSTEMS - PART 2**
**Duration:** Week 7 | **Lectures:** 3

### Topics Covered:
1. **Advanced Database Topics**
   - **Sharding (Horizontal Partitioning):**
     - Range-based sharding
     - Hash-based sharding
     - Directory-based sharding
     - Consistent hashing
     - Shard rebalancing
     - Challenges: cross-shard queries, transactions
   
   - **Replication:**
     - Master-slave replication
     - Master-master replication
     - Synchronous vs asynchronous
     - Replication lag
     - Read replicas
     - Conflict resolution
   
   - **Partitioning:**
     - Vertical partitioning
     - Horizontal partitioning
     - Functional partitioning
   
   - **Polyglot Persistence:**
     - Using multiple database types
     - Choosing right tool for each job
     - Data synchronization challenges

2. **Object Storage in Modern Systems**
   - Object storage vs block storage vs file storage
   - **Object storage characteristics:**
     - Flat namespace
     - Metadata-rich
     - Scalability
     - Durability
   
   - **Popular solutions:**
     - Amazon S3
     - Google Cloud Storage
     - Azure Blob Storage
   
   - **Use cases:**
     - Media storage
     - Backups
     - Data lakes
   
   - **Best practices:**
     - Lifecycle policies
     - Versioning
     - Access control
     - Cost optimization

3. **File Systems and Distributed Storage**
   - Traditional file systems (ext4, NTFS)
   - **Distributed file systems:**
     - HDFS (Hadoop Distributed File System)
     - GFS (Google File System)
     - Amazon EFS
   
   - **Characteristics:**
     - Fault tolerance
     - Replication
     - Block-based storage
   
   - **Use cases:**
     - Big data processing
     - Shared storage for clusters

### Key Concepts:
- Database sharding keys
- Replication topologies
- Object storage metadata
- Distributed consensus

### Best Practices:
- Choose sharding key carefully
- Monitor replication lag
- Implement retry logic
- Use object storage for immutable data
- Implement proper backup strategies

### Practice Problems:
1. Design sharding strategy for 100M user database
2. Calculate storage costs: S3 vs EBS vs EFS
3. Handle cross-shard transactions
4. Design replication topology for global application

### Subtopics to Master:
- Consistent hashing algorithm
- Vector clocks for conflict resolution
- Multi-master replication conflicts
- S3 storage classes and lifecycle policies

---

## **PHASE 11: STORAGE SYSTEMS - PART 3**
**Duration:** Week 8 | **Lectures:** 2

### Topics Covered:
1. **Big Data Fundamentals**
   - **3 Vs of Big Data:**
     - Volume: Massive amounts of data
     - Velocity: Speed of data generation
     - Variety: Different data types
   
   - **Additional Vs:**
     - Veracity: Data quality
     - Value: Business value extraction
   
   - **Big Data Storage:**
     - Data lakes vs Data warehouses
     - Columnar storage (Parquet, ORC)
     - Data lake architectures
   
   - **Processing frameworks:**
     - Batch processing: Hadoop MapReduce
     - Stream processing: Apache Kafka, Flink
     - Hybrid: Apache Spark
   
   - **Data warehouse solutions:**
     - Amazon Redshift
     - Google BigQuery
     - Snowflake

2. **Choosing the Right Storage Solution**
   - **Decision matrix:**
     - Data structure
     - Query patterns
     - Scalability needs
     - Consistency requirements
     - Cost considerations
   
   - **When to use what:**
     - RDBMS: Transactional, structured data
     - NoSQL: Unstructured, high scalability
     - Object storage: Blobs, media files
     - File systems: Shared file access
     - Data warehouse: Analytics, BI

### Key Concepts:
- Data lake vs data warehouse
- OLTP vs OLAP
- Lambda architecture
- Kappa architecture

### Best Practices:
- Separate OLTP and OLAP workloads
- Use appropriate compression
- Partition data logically
- Implement data retention policies
- Monitor storage costs

### Practice Problems:
1. Design data architecture for analytics platform
2. Compare data lake vs data warehouse for BI use case
3. Choose storage solutions for: user profiles, product catalog, analytics, media files
4. Design ETL pipeline for big data

### Subtopics to Master:
- Data partitioning strategies
- Columnar storage benefits
- Star schema vs snowflake schema
- Data lineage and governance

---

## **PHASE 12: SYSTEM PERFORMANCE - PART 1**
**Duration:** Week 8-9 | **Lectures:** 3

### Topics Covered:
1. **Introduction to System Performance**
   - **Performance metrics:**
     - Latency: Response time
     - Throughput: Requests per second
     - Bandwidth: Data transfer rate
     - Resource utilization: CPU, memory, disk, network
   
   - **Performance vs Scalability:**
     - Performance: Speed for single user
     - Scalability: Speed as users increase
   
   - **Bottleneck identification:**
     - Profiling
     - Monitoring
     - Load testing
   
   - **SLIs, SLOs, SLAs:**
     - Service Level Indicators
     - Service Level Objectives
     - Service Level Agreements

2. **Caching for Speed Optimization**
   - **Why caching?**
     - Reduce latency
     - Reduce database load
     - Improve user experience
   
   - **Cache levels:**
     - Client-side (browser cache)
     - CDN
     - Application cache
     - Database cache
   
   - **Caching strategies:**
     - Cache-aside (lazy loading)
     - Write-through
     - Write-behind (write-back)
     - Refresh-ahead
   
   - **Cache eviction policies:**
     - LRU (Least Recently Used)
     - LFU (Least Frequently Used)
     - FIFO (First In First Out)
     - TTL (Time To Live)
   
   - **Distributed caching:**
     - Redis
     - Memcached
     - Hazelcast
   
   - **Challenges:**
     - Cache invalidation
     - Cache stampede
     - Cold start problem

### Key Concepts:
- Cache hit ratio
- Cache coherence
- Cache warming
- Thundering herd problem

### Best Practices:
- Set appropriate TTL
- Monitor cache hit rates
- Implement cache fallback
- Use cache for read-heavy workloads
- Avoid caching user-specific data globally

### Practice Problems:
1. Calculate cache hit ratio improvement on latency
2. Design multi-level caching strategy
3. Handle cache invalidation for product price updates
4. Choose between Redis and Memcached

### Subtopics to Master:
- Cache coherence protocols
- Distributed cache consistency
- Cache-aside vs read-through patterns
- Redis data structures and use cases

---

## **PHASE 13: SYSTEM PERFORMANCE - PART 2**
**Duration:** Week 9 | **Lectures:** 3

### Topics Covered:
1. **Messaging & Queues for Decoupling**
   - **Why message queues?**
     - Asynchronous processing
     - Decoupling services
     - Load leveling
     - Reliability
   
   - **Message queue patterns:**
     - Point-to-point (queue)
     - Publish-subscribe (topic)
     - Request-reply
   
   - **Popular message brokers:**
     - **RabbitMQ:**
       - AMQP protocol
       - Flexible routing
       - Use cases: Task queues
     
     - **Apache Kafka:**
       - High throughput
       - Log-based storage
       - Use cases: Event streaming, analytics
     
     - **Amazon SQS:**
       - Managed service
       - Standard vs FIFO queues
     
     - **Redis Pub/Sub:**
       - Lightweight
       - In-memory
   
   - **Key concepts:**
     - Message acknowledgment
     - Dead letter queues
     - Message ordering
     - At-least-once vs exactly-once delivery
     - Idempotency

2. **Concurrency & Parallelism**
   - **Concurrency vs Parallelism:**
     - Concurrency: Multiple tasks in progress
     - Parallelism: Multiple tasks executing simultaneously
   
   - **Concurrency patterns:**
     - Multi-threading
     - Multi-processing
     - Asynchronous I/O
     - Event-driven
   
   - **Challenges:**
     - Race conditions
     - Deadlocks
     - Livelocks
     - Starvation
   
   - **Synchronization:**
     - Locks and mutexes
     - Semaphores
     - Atomic operations
     - Lock-free data structures
   
   - **Actor model:**
     - Message-based concurrency
     - Akka, Erlang

3. **Database Performance Optimization**
   - **Indexing:**
     - B-tree indexes
     - Hash indexes
     - Bitmap indexes
     - Full-text indexes
     - Composite indexes
     - Index strategies
   
   - **Query optimization:**
     - Query execution plans
     - Query analysis (EXPLAIN)
     - Avoiding N+1 queries
     - Batch operations
   
   - **Connection pooling:**
     - Reduce connection overhead
     - Pool sizing
   
   - **Denormalization:**
     - When to denormalize
     - Materialized views
     - Caching computed values
   
   - **Database-specific optimizations:**
     - Vacuuming (PostgreSQL)
     - Query cache (MySQL)
     - Read replicas
     - Partitioning

### Key Concepts:
- Message durability
- Consumer groups
- Backpressure
- Database query planning

### Best Practices:
- Use message queues for async tasks
- Implement idempotent consumers
- Index based on query patterns
- Monitor queue depth
- Use connection pooling
- Profile slow queries

### Practice Problems:
1. Design email notification system with message queue
2. Handle exactly-once message delivery
3. Optimize slow database queries
4. Design concurrent data processing pipeline

### Subtopics to Master:
- Kafka partitions and consumer groups
- Message serialization formats
- Database explain plans
- Optimistic vs pessimistic locking

---

## **PHASE 14: SYSTEM RELIABILITY**
**Duration:** Week 10 | **Lectures:** 4

### Topics Covered:
1. **Introduction to System Reliability**
   - **Reliability metrics:**
     - Uptime/downtime
     - MTBF (Mean Time Between Failures)
     - MTTR (Mean Time To Repair)
     - Availability percentage (99.9%, 99.99%, 99.999%)
   
   - **Nines of availability:**
     - 99% = 3.65 days downtime/year
     - 99.9% = 8.76 hours downtime/year
     - 99.99% = 52.56 minutes downtime/year
     - 99.999% = 5.26 minutes downtime/year
   
   - **Failure types:**
     - Hardware failures
     - Software bugs
     - Network issues
     - Human errors

2. **High Availability, Fault Tolerance & Failover**
   - **High Availability:**
     - Redundancy
     - No single point of failure
     - Active-active configuration
     - Active-passive configuration
   
   - **Fault Tolerance:**
     - System continues despite failures
     - Graceful degradation
     - Self-healing systems
   
   - **Failover mechanisms:**
     - Automatic failover
     - Manual failover
     - Failover testing
   
   - **Redundancy strategies:**
     - Server redundancy
     - Data redundancy
     - Network redundancy
     - Geographic redundancy
   
   - **Health checks:**
     - Liveness probes
     - Readiness probes
     - Deep health checks

3. **Backup & Recovery Strategies**
   - **Backup types:**
     - Full backup
     - Incremental backup
     - Differential backup
   
   - **Backup strategies:**
     - 3-2-1 rule (3 copies, 2 media types, 1 offsite)
     - Backup frequency
     - Retention policies
   
   - **Recovery objectives:**
     - RPO (Recovery Point Objective): Data loss tolerance
     - RTO (Recovery Time Objective): Downtime tolerance
   
   - **Database backups:**
     - Hot backups
     - Cold backups
     - Point-in-time recovery

4. **Disaster Recovery**
   - **Disaster recovery planning:**
     - Risk assessment
     - DR site selection
     - Runbooks
   
   - **DR strategies:**
     - Backup and restore (low cost, high RTO)
     - Pilot light (minimal running, faster RTO)
     - Warm standby (running at reduced capacity)
     - Hot standby/multi-site (expensive, lowest RTO)
   
   - **DR testing:**
     - Regular drills
     - Tabletop exercises
     - Failover testing

### Key Concepts:
- Five nines availability
- RTO vs RPO
- Single point of failure (SPOF)
- Chaos engineering

### Best Practices:
- Eliminate SPOFs
- Automate failover
- Test backup restoration regularly
- Document DR procedures
- Implement circuit breakers
- Use health checks
- Practice DR drills

### Practice Problems:
1. Calculate availability for system with multiple components
2. Design HA architecture for critical application
3. Choose DR strategy based on RTO/RPO requirements
4. Calculate backup storage needs

### Subtopics to Master:
- Circuit breaker pattern
- Bulkhead pattern
- Retry with exponential backoff
- Multi-region deployment

---

## **PHASE 15: SECURITY IN SYSTEM DESIGN**
**Duration:** Week 10-11 | **Lectures:** 4

### Topics Covered:
1. **Introduction to Security in System Design**
   - **Security principles:**
     - Defense in depth
     - Principle of least privilege
     - Secure by default
     - Fail securely
   
   - **Security threats:**
     - Injection attacks (SQL, XSS, CSRF)
     - DDoS attacks
     - Man-in-the-middle attacks
     - Data breaches
   
   - **OWASP Top 10:**
     - Injection
     - Broken authentication
     - Sensitive data exposure
     - XML external entities
     - Broken access control
     - Security misconfiguration
     - XSS
     - Insecure deserialization
     - Using components with known vulnerabilities
     - Insufficient logging

2. **Authentication & Authorization**
   - **Authentication:**
     - Username/password
     - Multi-factor authentication (MFA)
     - Biometric authentication
     - SSO (Single Sign-On)
     - Social login (OAuth)
   
   - **Authorization:**
     - RBAC (Role-Based Access Control)
     - ABAC (Attribute-Based Access Control)
     - ACL (Access Control Lists)
   
   - **Token-based auth:**
     - JWT (JSON Web Tokens)
     - OAuth 2.0 flows
     - OpenID Connect
   
   - **Session management:**
     - Session tokens
     - Cookie security
     - Session timeout

3. **Data Protection & Secure Communication**
   - **Encryption:**
     - Symmetric encryption (AES)
     - Asymmetric encryption (RSA)
     - Hashing (SHA-256, bcrypt)
   
   - **Data at rest:**
     - Database encryption
     - Disk encryption
     - Encrypted backups
   
   - **Data in transit:**
     - TLS/SSL
     - Certificate management
     - Perfect forward secrecy
   
   - **Data in use:**
     - Application-level encryption
     - Key management
   
   - **Key management:**
     - Key rotation
     - HSM (Hardware Security Modules)
     - AWS KMS, Azure Key Vault

4. **Network & Infrastructure Security**
   - **Network security:**
     - Firewalls
     - VPN (Virtual Private Networks)
     - Network segmentation
     - DMZ (Demilitarized Zone)
   
   - **DDoS protection:**
     - Rate limiting
     - CloudFlare, AWS Shield
     - Traffic filtering
   
   - **Security monitoring:**
     - IDS/IPS (Intrusion Detection/Prevention)
     - SIEM (Security Information and Event Management)
     - Log aggregation
   
   - **Cloud security:**
     - IAM (Identity and Access Management)
     - Security groups
     - Network ACLs
     - VPC (Virtual Private Cloud)
   
   - **Container security:**
     - Image scanning
     - Runtime protection
     - Secrets management

### Key Concepts:
- Zero-trust architecture
- Defense in depth
- Security by design
- Encryption at rest and in transit

### Best Practices:
- Never store passwords in plain text
- Use HTTPS everywhere
- Implement rate limiting
- Regular security audits
- Principle of least privilege
- Security headers (CSP, HSTS)
- Input validation and sanitization
- Dependency scanning

### Practice Problems:
1. Design authentication system with MFA
2. Implement OAuth 2.0 flow
3. Design secure API with rate limiting
4. Create security architecture for PCI-DSS compliance

### Subtopics to Master:
- JWT structure and validation
- OAuth 2.0 flows (authorization code, implicit, client credentials)
- TLS handshake process
- Common attack vectors and mitigations

---

## **PHASE 16: SYSTEM DESIGN INTERVIEW APPROACH**
**Duration:** Week 11 | **Lectures:** 1

### Topics Covered:
1. **The 4-Step System Design Approach**
   
   **STEP 1: Understand the Problem & Define Scope (5-10 minutes)**
   - Ask clarifying questions
   - Define functional requirements
   - Define non-functional requirements
   - Identify constraints
   - Example questions:
     - Who are the users?
     - What features are needed?
     - How many users?
     - What's the expected traffic?
     - What are the latency requirements?
   
   **STEP 2: Estimate Scale & Identify Bottlenecks (5-10 minutes)**
   - Back-of-envelope calculations:
     - DAU (Daily Active Users)
     - QPS (Queries Per Second)
     - Storage requirements
     - Bandwidth requirements
   - Identify potential bottlenecks
   - Example calculations:
     - 100M DAU, 10 actions/day = 100M × 10 / 86400 ≈ 11,574 QPS
   
   **STEP 3: High-Level Design (15-20 minutes)**
   - Draw architecture diagram
   - Define main components/services
   - Design APIs
   - Choose communication protocols
   - Data flow
   - Keep it simple initially
   
   **STEP 4: Deep Dive & Tech Decisions (15-20 minutes)**
   - Database choice (SQL vs NoSQL)
   - Caching strategy
   - Load balancing
   - Scaling approach
   - Data partitioning
   - Address bottlenecks
   - Trade-offs discussion

### Key Concepts:
- Requirements gathering
- Capacity estimation
- Component design
- Trade-off analysis

### Best Practices:
- Think out loud
- Ask clarifying questions
- Start simple, then iterate
- Discuss trade-offs
- Use standard components
- Draw clear diagrams
- Focus on what interviewer cares about
- Manage time effectively

### Interview Tips:
- Don't jump to solution immediately
- It's okay to make assumptions (state them clearly)
- No perfect solution exists
- Interviewer is evaluating thought process
- Be ready to defend your choices
- Listen to hints from interviewer

---

## **PHASE 17-25: PRACTICAL SYSTEM DESIGN PROBLEMS**

Each of the remaining phases covers a complete system design problem following the 4-step approach.

---

## **PHASE 17: URL SHORTENER**
**Duration:** Week 12 | **Lectures:** 5

### Problem Statement:
Design a URL shortening service like bit.ly or TinyURL.

### Step 1: Requirements & Scope
**Functional Requirements:**
- Shorten long URLs
- Redirect short URL to original URL
- Custom short URLs (optional)
- URL expiration (optional)
- Analytics (click tracking)

**Non-Functional Requirements:**
- High availability
- Low latency redirects
- Scalable (billions of URLs)
- Durable (URLs don't get lost)

**Assumptions:**
- 100M URLs created per month
- 10:1 read:write ratio

### Step 2: Capacity Estimation
**Traffic:**
- Write: 100M / month = 100M / (30 × 24 × 3600) ≈ 40 writes/sec
- Read: 40 × 10 = 400 reads/sec

**Storage:**
- Average URL size: 500 bytes
- 100M URLs/month × 12 months × 5 years = 6B URLs
- 6B × 500 bytes = 3 TB

**Bandwidth:**
- Write: 40 req/s × 500 bytes = 20 KB/s
- Read: 400 req/s × 500 bytes = 200 KB/s

**Short URL length:**
- Base62 encoding [a-zA-Z0-9] = 62 characters
- 62^7 = 3.5 trillion unique URLs

### Step 3: High-Level Design
**Components:**
1. **API Gateway** - Entry point
2. **URL Shortening Service** - Generate short URLs
3. **Redirection Service** - Handle redirects
4. **Database** - Store URL mappings
5. **Cache** - Store popular URLs
6. **Analytics Service** - Track clicks

**APIs:**
```
POST /api/shorten
Request: { "longUrl": "https://example.com/very/long/url" }
Response: { "shortUrl": "https://short.ly/abc123" }

GET /{shortCode}
Response: HTTP 302 redirect
```

**Database Schema:**
```
urls table:
- id (primary key)
- short_code (unique index)
- long_url
- user_id
- created_at
- expires_at

analytics table:
- id
- short_code
- timestamp
- ip_address
- user_agent
```

### Step 4: Detailed Design & Tech Decisions

**URL Generation Strategies:**
1. **MD5 Hash + Base62:**
   - Hash long URL
   - Take first 7 characters
   - Handle collisions with counter

2. **Counter-based:**
   - Auto-incrementing ID
   - Convert to Base62
   - More predictable, simpler

3. **Pre-generated keys:**
   - Generate keys in advance
   - Store in key generation service
   - Distributed coordination needed

**Chosen Approach: Counter-based with distributed ID generation**
- Use Snowflake ID or similar
- Guarantees uniqueness
- No collision handling needed

**Database Choice:**
- **Primary DB:** Cassandra/DynamoDB
  - Massive scale
  - High write throughput
  - Eventually consistent (acceptable for this use case)

- **Alternative:** PostgreSQL with sharding
  - ACID guarantees
  - Shard by hash(short_code)

**Caching:**
- Redis for hot URLs
- LRU eviction
- TTL based on expiration
- Cache read-heavy URLs (80/20 rule)

**Scaling:**
- Stateless services for easy horizontal scaling
- Database sharding by short_code hash
- Read replicas for read-heavy load
- CDN for static assets

**Additional Features:**
- Rate limiting (prevent abuse)
- Custom URLs (check availability)
- Analytics (async processing with message queue)

### Best Practices:
- Use 301 (permanent) vs 302 (temporary) redirect appropriately
- Implement URL validation
- Handle edge cases (malicious URLs)
- Monitor popular URLs for caching

### Practice Problems:
1. How would you handle 10x traffic increase?
2. Design analytics pipeline for click tracking
3. Handle URL expiration cleanup
4. Implement custom short URL feature

### Common Follow-up Questions:
- How to prevent abuse?
- How to handle hot URLs?
- Database choice justification?
- How to scale to 100x traffic?

---

## **PHASE 18: TICKETING SYSTEM**
**Duration:** Week 12 | **Lectures:** 5

### Problem Statement:
Design a ticketing system for events (concerts, movies, sports).

### Step 1: Requirements & Scope
**Functional Requirements:**
- Browse events
- Search events
- View seat availability
- Book tickets
- Payment processing
- Cancel booking
- Prevent double booking

**Non-Functional Requirements:**
- High availability
- Strong consistency (no double booking)
- Handle traffic spikes
- Low latency for booking

**Assumptions:**
- 10M users
- 1M events
- 100M bookings/year

### Step 2: Capacity Estimation
**Traffic:**
- Peak: 10,000 bookings/sec (concert releases)
- Average: 100M / year ≈ 3 bookings/sec
- Read:Write = 100:1

**Storage:**
- Events: 1M × 1KB = 1GB
- Bookings: 100M × 500 bytes = 50GB/year
- Total: ~500GB over 5 years

### Step 3: High-Level Design
**Components:**
1. **Event Service** - Manage events
2. **Booking Service** - Handle reservations
3. **Payment Service** - Process payments
4. **Notification Service** - Send confirmations
5. **Seat Inventory Service** - Track availability

**APIs:**
```
GET /events?city=NYC&date=2026-03-01
POST /bookings
  { "eventId": 123, "seats": ["A1", "A2"], "userId": 456 }
POST /payments
  { "bookingId": 789, "amount": 100, "paymentMethod": "card" }
```

**Database Schema:**
```
events:
- id, name, venue, date, total_seats

seats:
- id, event_id, section, row, number, price, status (available/booked/locked)

bookings:
- id, event_id, user_id, seats[], status, created_at

payments:
- id, booking_id, amount, status
```

### Step 4: Detailed Design & Tech Decisions

**Critical Challenge: Preventing Double Booking**

**Approach 1: Database Transactions (Pessimistic Locking)**
```sql
BEGIN TRANSACTION;
SELECT * FROM seats WHERE id IN (1,2,3) FOR UPDATE;
-- Check if available
UPDATE seats SET status='booked' WHERE id IN (1,2,3);
COMMIT;
```
- Pros: Strong consistency
- Cons: Locks can cause contention

**Approach 2: Optimistic Locking (Version Number)**
```sql
UPDATE seats 
SET status='booked', version=version+1 
WHERE id IN (1,2,3) AND version=5;
```
- Pros: Better concurrency
- Cons: Retry logic needed

**Approach 3: Distributed Lock (Redis)**
```
SETNX lock:event:123:seat:A1 1
SET lock:event:123:seat:A1 1 EX 10
```
- Pros: Fast, scalable
- Cons: Additional complexity

**Chosen Approach: Hybrid**
- Optimistic locking for normal load
- Distributed locking for high-demand events
- Temporary "hold" for 10 minutes during payment

**Seat Inventory Management:**
- Cache seat availability in Redis
- Update DB and cache atomically
- Periodic consistency checks

**Handling Traffic Spikes:**
- Queue system for booking requests
- Rate limiting per user
- CAPTCHA for bot prevention
- Virtual waiting room

**Database Choice:**
- PostgreSQL for strong consistency
- Read replicas for event browsing
- Sharding by event_id for large events

**Payment Flow:**
1. Reserve seats (temporary hold)
2. Process payment (external gateway)
3. Confirm booking or release seats
4. Send confirmation

**Scaling:**
- Separate read and write paths
- Cache event details and seat maps
- Async processing for non-critical tasks
- Partition database by geography

### Best Practices:
- Implement idempotency for payments
- Use saga pattern for distributed transactions
- Implement proper timeout handling
- Monitor seat availability accuracy

### Practice Problems:
1. Handle 100K concurrent users for popular event
2. Design seat hold timeout mechanism
3. Implement fair queuing for high-demand events
4. Handle payment failures and retries

---

## **PHASE 19: NEWS FEED (Social Media Feed)**
**Duration:** Week 13 | **Lectures:** 5

### Problem Statement:
Design a news feed system like Facebook, Twitter, or Instagram.

### Step 1: Requirements & Scope
**Functional Requirements:**
- Post creation (text, images, videos)
- Follow/unfollow users
- View personalized feed
- Like, comment, share
- Real-time updates

**Non-Functional Requirements:**
- Highly available
- Low latency (< 200ms for feed)
- Scalable (500M users)
- Eventually consistent

**Assumptions:**
- 500M DAU
- Average 5 posts viewed per session
- 100M new posts/day

### Step 2: Capacity Estimation
**Traffic:**
- Feed reads: 500M × 5 / 86400 ≈ 29,000 QPS
- Post writes: 100M / 86400 ≈ 1,157 QPS
- Peak: 3x average

**Storage:**
- Posts: 100M/day × 1KB = 100GB/day = 36TB/year
- Media: 50% with images (500KB avg) = 25TB/day
- Total: ~10PB over 5 years

**Bandwidth:**
- Reads: 29K QPS × 10KB (with images) = 290 MB/s
- Writes: 1.2K QPS × 1KB = 1.2 MB/s

### Step 3: High-Level Design
**Components:**
1. **Post Service** - Create/manage posts
2. **Feed Generation Service** - Build feeds
3. **Feed Service** - Serve feeds
4. **Fanout Service** - Distribute posts
5. **Graph Service** - Manage relationships
6. **Media Service** - Handle images/videos
7. **Notification Service** - Real-time updates

**APIs:**
```
POST /posts
  { "userId": 123, "content": "Hello", "mediaUrls": [] }

GET /feed?userId=123&page=1
  Response: [ { postId, author, content, timestamp, likes, comments } ]

POST /follow
  { "followerId": 123, "followeeId": 456 }
```

### Step 4: Detailed Design & Tech Decisions

**Feed Generation: Critical Design Decision**

**Approach 1: Pull Model (News Feed on Read)**
- Generate feed when user requests
- Query posts from all followed users
- Sort by timestamp
- **Pros:** Fresh content, simple writes
- **Cons:** Slow reads, database intensive

**Approach 2: Push Model (Fanout on Write)**
- Pre-compute and store feeds
- When user posts, push to all followers' feeds
- **Pros:** Fast reads
- **Cons:** Expensive writes for celebrities

**Approach 3: Hybrid**
- **Push for regular users** (< 10K followers)
- **Pull for celebrities** (> 10K followers)
- Merge at read time

**Chosen: Hybrid Approach**

**Feed Storage:**
```
user_feed:user_id → List of post_ids (sorted by timestamp)
```
- Store in Redis (in-memory, fast)
- Limit to latest 1000 posts per user
- Older posts fetched from database

**Fanout Service:**
```
1. User creates post
2. Fetch follower list from graph service
3. If followers < 10K:
     - Push post_id to each follower's feed (Redis)
   Else:
     - Mark for pull
4. Async processing via message queue
```

**Ranking & Personalization:**
- Simple: Chronological
- Advanced: ML-based ranking
  - User interactions
  - Post engagement
  - Recency
  - Content type preference

**Database Schema:**
```
posts:
- id, user_id, content, media_urls, created_at, likes_count

follows:
- follower_id, followee_id, created_at

user_feed:
- user_id, post_ids[] (in Redis)
```

**Database Choice:**
- **Posts:** Cassandra (write-heavy, time-series data)
- **Follows:** PostgreSQL (relational queries)
- **Feed:** Redis (fast reads)
- **Media:** S3 + CDN

**Scaling:**
- Shard posts by user_id or post_id
- Shard feeds by user_id
- Cache hot posts
- Use message queues for fanout
- Async processing for non-critical tasks

**Real-time Updates:**
- WebSocket connections for active users
- Push notifications for offline users
- Long polling as fallback

### Best Practices:
- Denormalize for read performance
- Cache celebrity posts
- Implement pagination
- Use CDN for media
- Monitor feed generation latency

### Practice Problems:
1. Handle celebrity with 100M followers posting
2. Implement post ranking algorithm
3. Design comment threading
4. Handle deleted/edited posts in feeds

---

## **PHASE 20: NOTIFICATION SYSTEM**
**Duration:** Week 13 | **Lectures:** 5

### Problem Statement:
Design a notification system supporting push notifications, SMS, and email.

### Step 1: Requirements & Scope
**Functional Requirements:**
- Send notifications via multiple channels (push, email, SMS)
- User notification preferences
- Priority-based delivery
- Template management
- Delivery tracking
- Retry failed notifications

**Non-Functional Requirements:**
- Scalable (10M notifications/day)
- Reliable delivery
- Low latency for high-priority
- Exactly-once delivery (best effort)

### Step 2: Capacity Estimation
**Traffic:**
- 10M notifications/day = 115 notifications/sec
- Peak: 1000 notifications/sec
- Mix: 60% push, 30% email, 10% SMS

**Storage:**
- Notification logs: 10M/day × 500 bytes = 5GB/day

### Step 3: High-Level Design
**Components:**
1. **Notification API** - Accept notification requests
2. **Notification Service** - Orchestrate delivery
3. **Channel Services:**
   - Push Notification Service (FCM, APNS)
   - Email Service (SendGrid, SES)
   - SMS Service (Twilio)
4. **Template Service** - Manage templates
5. **User Preference Service** - Store preferences
6. **Queue** - Buffer notifications
7. **Tracking Service** - Monitor delivery

**APIs:**
```
POST /notifications
{
  "userId": 123,
  "type": "ORDER_SHIPPED",
  "channels": ["push", "email"],
  "priority": "high",
  "data": { "orderId": 456, "trackingId": "ABC123" }
}
```

### Step 4: Detailed Design & Tech Decisions

**Architecture Flow:**
```
1. Service → Notification API
2. Validate & enrich (fetch user preferences)
3. Route to appropriate queues (by channel & priority)
4. Workers pick from queues
5. Send via channel providers
6. Track delivery status
7. Retry on failure
```

**Queue Strategy:**
- Separate queues per channel
- Priority queues (high/medium/low)
- Dead letter queue for failed deliveries
- Use Kafka or RabbitMQ

**User Preferences:**
```
user_preferences:
- user_id
- email_enabled, push_enabled, sms_enabled
- quiet_hours (start, end)
- notification_types { "ORDER": true, "MARKETING": false }
```

**Template Management:**
```
templates:
- id, type, channel, subject, body
- Variables: {{userName}}, {{orderId}}
```

**Delivery Guarantees:**
- **At-least-once:** Use message queue acknowledgment
- **Idempotency:** Deduplication key (hash of user_id + notification_type + timestamp)
- **Rate limiting:** Per user, per channel

**Third-party Integration:**
- **Push:** FCM (Android), APNS (iOS)
- **Email:** SendGrid, AWS SES
- **SMS:** Twilio, AWS SNS
- Handle provider failures with circuit breaker

**Retry Strategy:**
- Exponential backoff: 1s, 2s, 4s, 8s, 16s
- Max 5 retries
- Move to dead letter queue
- Alert on high failure rate

**Tracking:**
```
notification_events:
- notification_id, event_type (sent/delivered/failed/clicked), timestamp
```

**Database:**
- PostgreSQL for user preferences
- Cassandra for notification logs (time-series)
- Redis for rate limiting and deduplication

**Scaling:**
- Horizontal scaling of workers
- Partition queues by user_id or channel
- Cache user preferences
- Async processing

### Best Practices:
- Respect user preferences always
- Implement unsubscribe mechanism
- Monitor delivery rates
- Handle provider downtime
- Batch email sends for efficiency

### Practice Problems:
1. Design rate limiting for marketing notifications
2. Handle timezone-aware delivery
3. Implement notification grouping (merge similar notifications)
4. Design analytics for notification effectiveness

---

## **PHASE 21: CHAT APPLICATION**
**Duration:** Week 14 | **Lectures:** 5

### Problem Statement:
Design a real-time chat application like WhatsApp or Slack.

### Step 1: Requirements & Scope
**Functional Requirements:**
- One-on-one messaging
- Group chat
- Online/offline status
- Message delivery status (sent/delivered/read)
- Media sharing
- Message history
- Push notifications

**Non-Functional Requirements:**
- Real-time delivery (< 100ms)
- High availability
- Scalable (1B users)
- Message persistence
- End-to-end encryption (optional)

### Step 2: Capacity Estimation
**Traffic:**
- 1B users, 100M DAU
- Average 50 messages/user/day
- 5B messages/day = 57,870 messages/sec
- Peak: 3x = 173K messages/sec

**Storage:**
- Messages: 5B/day × 100 bytes = 500GB/day = 182TB/year
- Media: 20% with images = 36TB/day

### Step 3: High-Level Design
**Components:**
1. **Chat Service** - Handle messaging
2. **WebSocket Service** - Real-time connections
3. **Message Service** - Store/retrieve messages
4. **Presence Service** - Online/offline status
5. **Group Service** - Manage groups
6. **Notification Service** - Push notifications
7. **Media Service** - Handle file uploads

**APIs:**
```
WebSocket connection: ws://chat.app/connect?userId=123

Send message:
{
  "type": "message",
  "to": "user456",
  "content": "Hello",
  "timestamp": 1234567890
}

HTTP fallback:
POST /messages
GET /messages?conversationId=123&page=1
```

### Step 4: Detailed Design & Tech Decisions

**Real-time Communication:**
- **WebSockets** for bi-directional real-time
- Long polling as fallback
- Heartbeat for connection health

**Message Flow:**
```
1. User A sends message via WebSocket
2. Chat server receives message
3. Store in database (async)
4. Check if User B online
5. If online: Push via WebSocket
   If offline: Queue for push notification
6. Return acknowledgment to User A
```

**Message Storage:**
```
messages:
- message_id, from_user_id, to_user_id, content, 
  timestamp, delivery_status

group_messages:
- message_id, group_id, user_id, content, timestamp

conversations:
- conversation_id, participant_ids[], last_message_id,
  last_updated
```

**Database Choice:**
- **Messages:** Cassandra (time-series, write-heavy)
  - Partition by conversation_id
  - Sort by timestamp
- **User data:** PostgreSQL
- **Cache:** Redis for recent messages

**WebSocket Connection Management:**
- WebSocket servers (stateful)
- Connection registry (user_id → server_id) in Redis
- Heartbeat every 30 seconds
- Reconnection logic

**Message Delivery:**
```
Sent → Server acknowledged
Delivered → Recipient device received
Read → Recipient viewed
```

**Presence Service:**
- User connects → Update status to online
- Heartbeat timeout → Update to offline
- Store in Redis: user_id → {status, last_seen}
- Broadcast status to contacts

**Group Chat:**
```
1. Message sent to group
2. Fanout to all group members
3. Store single copy in database
4. Delivery tracking per member
```

**Scaling Challenges:**

**Challenge 1: WebSocket Connection Scaling**
- Single server limit: ~100K connections
- Use WebSocket servers cluster
- Load balance by user_id (consistent hashing)
- Service discovery (Consul, etcd)

**Challenge 2: Message Fanout (Group Chat)**
- For small groups (< 100): Direct fanout
- For large groups: Pagination, lazy loading

**Challenge 3: Message Ordering**
- Use message sequence numbers
- Client-side reordering if needed
- Lamport timestamps for distributed ordering

**Media Handling:**
- Upload to S3
- Generate thumbnail
- Send media URL in message
- Lazy loading

**Security:**
- Authentication via JWT
- Optional E2E encryption (Signal Protocol)
- Message encryption at rest

**Offline Support:**
- Queue messages for offline users
- Sync on reconnection
- Push notifications

### Best Practices:
- Implement message batching
- Compress messages
- Use CDN for media
- Monitor WebSocket connection health
- Implement typing indicators efficiently

### Practice Problems:
1. Handle 1M concurrent connections
2. Design message search functionality
3. Implement message edit/delete
4. Design read receipts for group chats

---

## **PHASE 22: AUCTION PLATFORM**
**Duration:** Week 14 | **Lectures:** 5

### Problem Statement:
Design an online auction platform like eBay.

### Step 1: Requirements
**Functional:**
- List items for auction
- Place bids
- Real-time bid updates
- Automatic bidding
- Auction end handling
- Payment processing
- Fraud detection

**Non-Functional:**
- Real-time bid updates (< 500ms)
- Strong consistency for bids
- Scalable (10M users)
- Fair auction (prevent manipulation)

### Step 2: Capacity Estimation
- 1M active auctions
- 100K concurrent bidders
- 1000 bids/second
- Peak: 10K bids/second

### Step 3: High-Level Design
**Components:**
1. Auction Service
2. Bidding Service
3. Notification Service
4. Payment Service
5. Fraud Detection Service

### Step 4: Detailed Design

**Bid Processing:**
```sql
BEGIN TRANSACTION;
SELECT current_bid, highest_bidder FROM auctions WHERE id = 123 FOR UPDATE;
IF new_bid > current_bid THEN
  UPDATE auctions SET current_bid = new_bid, highest_bidder = user_id;
  INSERT INTO bids (auction_id, user_id, amount, timestamp);
COMMIT;
```

**Critical Considerations:**
- Transaction isolation (prevent race conditions)
- Optimistic locking for better concurrency
- Distributed locks for high-traffic auctions

**Real-time Updates:**
- WebSockets for active bidders
- Server-Sent Events for watchers
- Push notifications for outbid alerts

**Automatic Bidding:**
```
proxy_bids:
- user_id, auction_id, max_bid, increment
```
- Trigger on new bid
- Auto-increase up to max_bid

**Auction End:**
- Scheduled job to close auctions
- Winner determination
- Notification to winner and seller
- Payment flow initiation

**Scaling:**
- Shard by auction_id
- Cache hot auctions
- Queue bid processing
- Rate limiting per user

### Practice Problems:
1. Handle 100K concurrent bids on single item
2. Design sniping prevention
3. Implement bid history compression
4. Design fraud detection rules

---

## **PHASE 23: ONLINE RENTAL PLATFORM (Airbnb)**
**Duration:** Week 15 | **Lectures:** 5

### Problem Statement:
Design property rental platform like Airbnb.

### Step 1: Requirements
**Functional:**
- List properties
- Search properties (location, dates, price)
- Booking management
- Payment processing
- Reviews and ratings
- Host/guest messaging

**Non-Functional:**
- Low latency search (< 200ms)
- High availability for bookings
- Prevent double bookings
- Scalable (10M properties)

### Step 2: Capacity Estimation
- 10M properties
- 100M searches/day
- 1M bookings/day
- 500K concurrent users

### Step 3: High-Level Design
**Components:**
1. Property Service
2. Search Service
3. Booking Service
4. Payment Service
5. Review Service
6. Messaging Service

### Step 4: Detailed Design

**Search Implementation:**
```
Geo-spatial search:
- Elasticsearch with geo-point fields
- Filter by: location (lat/lon + radius), dates, price, amenities
- Ranking: distance, price, ratings, availability
```

**Data Model:**
```
properties:
- id, host_id, title, description, location (geo-point),
  price, amenities[], images[]

bookings:
- id, property_id, guest_id, check_in, check_out, 
  status, price

availability:
- property_id, date, available (boolean)
```

**Preventing Double Bookings:**
```sql
BEGIN TRANSACTION;
SELECT * FROM availability 
WHERE property_id = 123 
  AND date BETWEEN '2026-03-01' AND '2026-03-05'
  AND available = true
FOR UPDATE;

-- If all dates available:
UPDATE availability SET available = false
WHERE property_id = 123 AND date IN (...);
INSERT INTO bookings (...);
COMMIT;
```

**Search Optimization:**
- Elasticsearch cluster
- Cache popular searches
- Pre-computed filters
- Pagination

**Pricing:**
- Dynamic pricing engine
- Demand-based adjustments
- Seasonal pricing
- Last-minute discounts

### Practice Problems:
1. Design map-based search with clustering
2. Handle high-demand property bookings
3. Implement flexible date search
4. Design review fraud detection

---

## **PHASE 24: CLOUD STORAGE SYSTEM (Dropbox/Google Drive)**
**Duration:** Week 15 | **Lectures:** 5

### Problem Statement:
Design a cloud storage and file synchronization system.

### Step 1: Requirements
**Functional:**
- Upload/download files
- File sync across devices
- File sharing
- Version history
- File recovery
- Real-time collaboration

**Non-Functional:**
- Reliable (no data loss)
- Fast sync (< 1s for small files)
- Efficient bandwidth usage
- Scalable (1B users, 10PB data)

### Step 2: Capacity Estimation
- 1B users, 100M DAU
- Average 10GB per user
- 10B files
- 100M file operations/day

### Step 3: High-Level Design
**Components:**
1. File Upload Service
2. File Download Service
3. Sync Service
4. Metadata Service
5. Block Storage
6. Notification Service

### Step 4: Detailed Design

**File Chunking:**
```
Large file (100MB):
- Split into chunks (4MB each)
- Hash each chunk (SHA-256)
- Upload only changed chunks (deduplication)
```

**Sync Algorithm:**
```
1. Client calculates file hashes
2. Compare with server metadata
3. Upload only changed chunks
4. Server reconstructs file
5. Notify other clients
6. Clients download changes
```

**Metadata:**
```
files:
- file_id, name, path, size, created_at, modified_at,
  owner_id, parent_folder_id

chunks:
- chunk_id, file_id, chunk_index, hash, size,
  storage_location

versions:
- version_id, file_id, chunk_ids[], timestamp
```

**Storage:**
- **Metadata:** PostgreSQL
- **Chunks:** S3 or distributed storage
- **Cache:** Redis for frequently accessed files

**Deduplication:**
- Content-based chunking
- Hash-based deduplication
- Save storage costs

**Conflict Resolution:**
- Last-write-wins (simple)
- Operational transformation (complex)
- Create conflict copies

**Offline Support:**
- Queue operations locally
- Sync on reconnection
- Merge conflicts

### Practice Problems:
1. Design real-time collaborative editing
2. Handle large file uploads (GB)
3. Implement efficient delta sync
4. Design file recovery from trash

---

## **PHASE 25: VIDEO SHARING PLATFORM (YouTube)**
**Duration:** Week 16 | **Lectures:** 5

### Problem Statement:
Design a video sharing platform like YouTube.

### Step 1: Requirements
**Functional:**
- Upload videos
- Stream videos
- Video recommendations
- Comments and likes
- Search videos
- Video transcoding

**Non-Functional:**
- Low latency streaming
- Scalable (1B users)
- Highly available
- Efficient storage

### Step 2: Capacity Estimation
- 1B users, 500M DAU
- 1M video uploads/day
- 5B video views/day
- Average video: 50MB, 5 minutes
- Storage: 50TB/day for new videos

### Step 3: High-Level Design
**Components:**
1. Upload Service
2. Transcoding Service
3. CDN
4. Video Service
5. Recommendation Engine
6. Search Service

### Step 4: Detailed Design

**Video Upload Flow:**
```
1. Client uploads video → Upload Service
2. Store original in S3
3. Queue for transcoding
4. Transcode to multiple resolutions (360p, 720p, 1080p)
5. Generate thumbnails
6. Update metadata
7. Notify user of completion
```

**Video Streaming:**
- **Adaptive Bitrate Streaming:**
  - HLS (HTTP Live Streaming)
  - DASH (Dynamic Adaptive Streaming)
  - Multiple quality levels
  - Client adapts based on bandwidth

**Storage:**
```
videos:
- video_id, title, description, user_id, upload_date,
  views, likes, duration

video_files:
- video_id, resolution, format, file_path, size

thumbnails:
- video_id, thumbnail_paths[]
```

**CDN Strategy:**
- Distribute popular videos to edge locations
- Cache based on popularity
- Origin servers for long-tail content

**Recommendation System:**
- Collaborative filtering
- Content-based filtering
- Watch history analysis
- ML model training pipeline

**Search:**
- Elasticsearch for video metadata
- Full-text search on title, description
- Tags and categories
- Autocomplete suggestions

**View Count:**
- Increment asynchronously
- Buffer in Redis
- Batch update to database
- Handle bots and fraud

**Scaling:**
- Separate upload and streaming
- Shard by video_id
- Use CDN extensively
- Async processing for transcoding

### Practice Problems:
1. Design live streaming feature
2. Handle viral video (1M concurrent viewers)
3. Implement view deduplication
4. Design copyright detection system

---

## **BONUS PHASES: Additional Advanced Topics**

### Advanced Topics to Study (Self-guided):
1. **Search Engine Design**
2. **E-commerce Platform**
3. **Ride-Sharing App (Uber/Lyft)**
4. **Collaborative Document Editor (Google Docs)**
5. **Rate Limiter**
6. **Distributed Cache**
7. **Metrics and Monitoring System**
8. **Ad Click Aggregation**

---

## **STUDY PLAN & PRACTICE STRATEGY**

### Weekly Schedule:
- **Week 1-2:** Phases 1-3 (Foundations, Networking)
- **Week 3-4:** Phases 4-6 (Protocols, Architecture)
- **Week 5-6:** Phases 7-9 (Web Concepts, Scalability, Storage)
- **Week 7-8:** Phases 10-12 (Storage, Performance)
- **Week 9-10:** Phases 13-15 (Performance, Reliability, Security)
- **Week 11:** Phase 16 (Interview Approach)
- **Week 12-16:** Phases 17-25 (Practical Problems)

### Daily Routine:
1. **Study:** 2 hours (watch conceptual videos, read documentation)
2. **Practice:** 1 hour (solve problems, draw diagrams)
3. **Review:** 30 minutes (revise notes, flashcards)

### Resources to Use:
1. **System Design Primer** (GitHub repository)
2. **Designing Data-Intensive Applications** (Book by Martin Kleppmann)
3. **System Design Interview** (Books by Alex Xu)
4. **Tech blogs:** Netflix, Uber, Airbnb, Facebook Engineering
5. **YouTube channels:** Gaurav Sen, Tech Dummies, System Design Interview
6. **Practice platforms:** SystemDesign.io, LeetCode, Pramp

### Practice Strategy:
1. **After each phase:** Solve 2-3 related problems
2. **Weekly:** Design 1 complete system end-to-end
3. **Monthly:** Mock interview with peer
4. **Keep a design journal:** Document your designs

### Interview Preparation (Final 4 weeks):
1. **Week 1:** Review all fundamental concepts
2. **Week 2:** Practice 10 common system design problems
3. **Week 3:** Mock interviews (2-3 per week)
4. **Week 4:** Review mistakes, refine approach

---
