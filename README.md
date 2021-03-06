# 1. Products - Web, Mobile, Data, APIs, Desktop, Console, Voice, AR/VR

**Stateless & Stateful:**
* Global Load Balancing, DNS-based & SDN Anycast
* Caching & CDN
* CAP Theorem
* Edge & Cloud Computing
* Availability, Regions & Zones

1. Synchronous, Serving System 
2. Asynchronous, Event Driven System

For Improvements Ask End Users, Developers to be critical & actively seek Feedback.

1. Prime Days - https://aws.amazon.com/blogs/aws/prime-day-2021-two-chart-topping-days/

# 2. Infrastructure - Compute, Storage & Network

**Large-scale distributed infrastructure:**
 
1. **Authenticate & Authorize**

* AWS Identity - [over 400 million API calls EVERY SECOND](https://aws.amazon.com/blogs/aws/happy-10th-birthday-aws-identity-and-access-management/)
* 

2. **"The Log"**

* [Event-Driven Architectures - The Queue vs The Log](https://jack-vanlightly.com/blog/2018/5/20/event-driven-architectures-the-queue-vs-the-log)

* Kafka:
  * Benchmarking - https://www.confluent.io/blog/kafka-fastest-messaging-system/
  * [Kafka Improvement Proposals](https://cwiki.apache.org/confluence/display/KAFKA/Kafka+Improvement+Proposals)
    * Tiered Storage
    * [Replace Zookeeper - A Raft Protocol for the Metadata Quorum](https://cwiki.apache.org/confluence/display/KAFKA/KIP-595%3A+A+Raft+Protocol+for+the+Metadata+Quorum)
  * [Vectorized](https://vectorized.io/) **Redpanda** - Kafka® API compatible, C++ Implementation
  * Write Ahead Log - https://wepay.github.io/waltz/docs/introduction
* Queue:
  * https://engineering.fb.com/2021/02/22/production-engineering/foqs-scaling-a-distributed-priority-queue/

3. **Purpose-built Databases**

Managing state - one of the hardest problem in distributed systems
* Key/Value - Cassandra; ScyllaDB, Apache Cassandra in C++
* Distributed SQL 

4. **Data Warehouse / Data Lake**

* Storage - [Cloud, S3](https://www.allthingsdistributed.com/2021/03/happy-15th-birthday-amazon-s3.html) / Open Source https://delta.io/
* Data Processing - </>

5. **Networking**

* Kubernetes - https://cloud.google.com/blog/products/containers-kubernetes/new-gke-gateway-controller-implements-kubernetes-gateway-api / https://smi-spec.io/#ecosystem

6. **Telemetry**
* eBPF - https://github.com/cloudflare/ebpf_exporter / https://engineering.fb.com/2021/04/27/developer-tools/reverse-debugging/

8. **Linux / Unix**
* Evolution of the Unix System Architecture ("Besides historical details, it also has a number of interesting lessons for software architecture evolution") - https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8704965
 
# 3. References

**1. As a service:**
![](https://github.com/ankumar/Architecture/blob/main/images/Cumulative%20CAPEX.jpg)

Source: https://www.platformonomics.com/2021/02/follow-the-capex-cloud-table-stakes-2020-retrospective/

> hyperscalers (Amazon, Google and Microsoft) have moved far outside their initial niche of standard IT infrastructure services. In addition to providing services for developers to reduce time-to-market, they have built specialist services targeted at the major technology trends such as blockchain, 5G, machine learning, artificial intelligence and digital identity. Moreover, they are adding many industry-focused solutions.

* **Cloud Native DB's**
  * **Distributed SQL** - GCP Spanner,  YugaByte DB (PostgreSQL), MariaDB SkySQL, CockroachDB, ...
  * **Key/Value** - Migrating Amazon retail services to NoSQL, **DynamoDB** ; re:Invent & Twitch Talks from Rick Houlihan 

* **IAM** 
  * https://www.okta.com/ / https://auth0.com/  
  * https://www.authorizon.com/ 
  * https://authzed.com/ 
  
* **Kubernetes**
  * [Google Cloud Run - FAQ](https://github.com/ahmetb/cloud-run-faq)

**2. Building:**

[@scale](https://atscaleconference.com/)

* [LogDevice](https://logdevice.io/)
* [Mcrouter (pronounced mc router)](https://github.com/facebook/mcrouter)
* https://db.cs.cmu.edu/archived-events/

---

**1. Blogs:**

* [Client-side load balancing technique](https://blog.twitter.com/engineering/en_us/topics/infrastructure/2019/daperture-load-balancer.html)
* [DNS based GSLB](https://dropbox.tech/infrastructure/intelligent-dns-based-load-balancing-at-dropbox)
* [Shard Manager](https://engineering.fb.com/production-engineering/scaling-services-with-shard-manager/)
* [Consensus Algorithms at Scale](https://www.planetscale.com/blog/blog-series-consensus-algorithms-at-scale-1)
* [Steve Yegge’s Google Platforms Rant](https://gist.github.com/chitchcock/1281611)
* [Excel is still going strong, just became a Turing-complete programming language!](https://www.microsoft.com/en-us/research/blog/lambda-the-ultimatae-excel-worksheet-function/)
* [The Distributed Operating System Void](https://nivenly.com/lib/2021-04-02-operating-system-interface/)
* [COSI - The Common Operating System Interface](https://docs.google.com/document/d/1OuwTSsSsIPefDViheK-nzaF9xSOg1Mn62mwR2FmGPu8/edit#heading=h.1grxkjflkt7d)

---

**2. Papers:**

* [The Datacenter as a Computer](http://bnrg.eecs.berkeley.edu/~randy/Courses/CS294.F09/wharehousesizedcomputers.pdf)
* [Fail at Scale](https://queue.acm.org/detail.cfm?id=2839461)
* [Zero downtime deployments at Facebook](https://dl.acm.org/doi/abs/10.1145/3387514.3405885)
* [Pitfalls of Anycast](https://www.usenix.org/sites/default/files/conference/protected-files/srecon17emea_slides_murali_suriar.pdf)
* [Influence of heavy-tailed distributions on load balancing](http://www.cs.cmu.edu/~harchol/ISCA15show.pdf)
* [Akamai DNS: Providing Authoritative Answers to the World’s Queries](https://groups.cs.umass.edu/ramesh/wp-content/uploads/sites/3/2020/07/sigcomm2020-final289.pdf)
* [Monarch: Google’s Planet-Scale In-Memory Time Series Database](http://www.vldb.org/pvldb/vol13/p3181-adams.pdf)
* [Read-Write Quorum Systems Made Practical](https://mwhittaker.github.io/publications/quoracle.html)
* [Zanzibar: Google’s Consistent, Global Authorization System](https://news.ycombinator.com/item?id=26980254)
* [Colossus - Google’s Storage Foundation](https://www.infoq.com/news/2021/04/google-colossus/)
* [Designing a Serverless Cloud-Native Database-as-a-Service Based on Apache Cassandra™](https://www.datastax.com/sites/default/files/content/whitepaper/files/2021-06/Astra%20Serverless%20Whitepaper_0.pdf)

---

**3. Tech Talks:**

* [Quarantine Database Tech Talks (2020)](https://www.youtube.com/playlist?list=PLSE8ODhjZXjagqlf1NxuBQwaMkrHXi-iz)
* [New Directions in Cloud Programming](https://www.youtube.com/watch?v=FeRg-7Sr1L8)
