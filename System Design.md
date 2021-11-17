# System Design

**1. Distributed Systems**

Links:

   * 

Characteristics of Distributed Systems:
* Scalability
* Reliability
* Availability
* Efficiency
* Serviceability


**2. Load balancer**

What it is? Why we use it?

Links:

   * https://www.thegeekstuff.com/2016/01/load-balancer-intro/
   * https://medium.com/must-know-computer-science/system-design-load-balancing-1c2e7675fc27

Load-balancing Algorithms:

* Least Connections Method
* Least Response Time Method
* Least Bandwidth Method
* IP hashing
* Round Robin
* Weighted Round Robin  

Example software/tools used in load-balancing:

* Haproxy
* Nginx (** Learn this one)

**3. Caching**

What it is? Why we cache?

Links:

   * https://medium.com/must-know-computer-science/system-design-caching-acbd1b02ca01
   * https://roadmap.sh/guides/http-caching

Concepts:

* Cache Hit
* Cache Miss
* Cache Invalidation
    * Write through cache
    * Write around cache
    * Write back cache
* Cache Eviction 
    * Policies:
        * FIFO (First In First Out)
        * LIFO (Last In First Out)
        * LRU (Least Recently Used)
        * Most Recently Used
        * Least Frequently Used
        * Random Replacement
* Time To Live (TTL)
* Server Side vs Client side 
* CDN (Content Delivery Network)

Example software/tools used in caching:

* Redis (** Learn this one)
* Memcache 

**4. Proxy**

What it is? Why we use it?

Links:

   * https://medium.com/must-know-computer-science/system-design-proxies-ef5f2c2676f2
   * https://roadmap.sh/guides/proxy-servers

Types:

* Reverse proxy
* Forward proxy

**5. Webservers**

What it is? Why we use it? How they work.

Links:

   * 
   
Examples:

* Apache
* NodeJS

**6. Client-Server Model**

What it is? 

Links:

   * https://medium.com/must-know-computer-science/system-design-client-server-communication-674818ca448d
   
Client-Server Communication techniques:  

* Ajax Long polling
* HTTP Long polling
* Web Sockets
    * Concepts: Keep-alive
* HTML5 Event Source (Server-sent event)
* Message Queues
* Streaming over HTTP 
   
**7. Logging**

Why we log?

Links:

   *
   
Concepts:

* Log levels
* Logrotation
  
**8. Data partitioning**

What it is? Why we do it?

Links:

   * https://medium.com/must-know-computer-science/system-design-sharding-data-partitioning-b7201596aafa
   * https://dev.mysql.com/doc/mysql-partitioning-excerpt/5.7/en/partitioning-types.html
   * https://www.digitalocean.com/community/tutorials/understanding-database-sharding
   
Partitioning Methods:

* Horizontal partitioning/Sharding
* Vertical partitioning
* Directory-based partitioning

Partitioning Criteria:

* Range partitioning
* Key or hash-based partitioning
* List partitioning
* Round-robin partitioning 
* Composite partitioning
  
**9. Performance**

Links:

   * https://medium.com/must-know-computer-science/system-design-redundancy-and-replication-e9946aa335ba
   * https://roadmap.sh/guides/what-is-sli-slo-sla
   
Metrics:

* Latency 
* Throughput:
    *Measuring throughput (percentiles vs averages)
* Availability (9s -https://www.vxchnge.com/blog/what-99.999-network-uptime-really-means )
* SLA (Service Level Agreement)
* Reliability 
* Consistency

Performance enhancing concepts:

* Redundancy and replication
* Scaling :Horizontal vs Vertical
   
**10. Other Technical Concepts**   

Links:

   * https://medium.com/must-know-computer-science/system-design-consistent-hashing-f66fa9b75f3f
  
Concepts:
 
* Hashing (Consistent hashing)
* Checksum
* Deduplication
* CRON jobs
* Event-driven architecture
* Servers-splitting - Depending on type of HTTP request eg: long polling reads might need separate server from write requests, Persistent connections might need their own server for instance in Chat Servers,


**11. Other General System Design Concepts**   

Links:

   * 
   
Requirements analysis:

* Functional - What the system is supposed to achieve.
* Non-functional - Other secondary things to be achieved e.g: security, reliability, availability.
* Other - Includes: Telemetry(analytics), API access by 3rd parties

Design considerations e.g:

* Should we cap the upload size in a photo system to 10MB
* Should we limit the size of a key in the DB
     
Capacity Estimation & Constraints - Estimate how much the system is supposed to handle:
* Traffic (requests/second)
* Bandwidth (KB/second) - Measure both ingress and egress
* Storage - Both database and object store. Calculate daily storage using
    daily writes & the estimated size of a request. e.g 1 million (daily writes) * 10KB (average request size) = 10GB/day 
* Memory - Applies if we have a cache.

Database design - Make observations about the nature of the data we are storing:
* How many records e.g 1 billion
* Size of each type of data being stored eg small (a few KBs)
* Is our system read-heavy or write-heavy
* Check if our entities have relations
