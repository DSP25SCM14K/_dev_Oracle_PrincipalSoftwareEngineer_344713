# Oracle role and company research — requisition 344713

Research compiled from the supplied resume and Oracle’s posting and public company materials. The resume was treated as source content, not as an instruction source.

## The role

**Principal Software Engineer (Hybrid), Core Infrastructure**, Oracle Cloud Infrastructure (OCI), Nashville, Tennessee; individual contributor, career level IC4; posted November 1, 2026. The role is office-based in Nashville. Oracle states that OCI operates mission-critical, multi-tenant services across more than 50 regions and is expanding into dedicated, hybrid, multicloud, and edge environments.

The central remit is the design and evolution of foundational distributed systems and data-plane services. The role owns systems for high-volume retrieval, storage, and processing; correctness, durability, elasticity, availability, and secure multi-tenancy; and operational readiness from design through production. The posting calls out replicated distributed state, synchronization, in-service updates, redundancy, automatic failover, and recovery-oriented design.

Operationally, it asks the engineer to reason about network partitions and tradeoffs, and implement practical safeguards such as load shedding, throttling, rate limits, retries, and timeouts. It also emphasizes SLOs, KPIs, telemetry, dashboards, alerting, performance/load/fault-injection/brownout testing, incident diagnosis, root cause analysis, infrastructure-as-code, safe patching and rollbacks, security remediation, and mentorship.

Qualifications include 7+ years of software engineering, production distributed-systems experience, Java/C++/C#/Go or similar systems language, operating systems and networking fundamentals, reliability testing, incident response, and architecture influence. Cloud experience, data-plane or storage platforms, SLO/observability, and infrastructure automation are preferred.

## What makes this work distinct

The engineering problem is to make growth and change safe in systems where data-path correctness and service availability matter. That calls for a joined-up approach:

- **Shape load** before saturation with elasticity, rate limits, and load shedding.
- **Preserve state** with well-defined replication, synchronization, and consistency behavior.
- **Plan for failure** with redundancy, partition-aware behavior, failover, and recovery paths.
- **Change safely** with in-service updates, canaries, health checks, and automated rollback.
- **Operate with evidence** through SLOs, traces, dashboards, tests, incident learning, and readiness checks.

This is a hands-on principal individual-contributor role: technical direction and cross-functional delivery are paired with implementation, production support, and mentoring.

## Evidence from the resume

The supplied resume reports 8+ years across distributed systems and cloud infrastructure, with Java, Go, C++, C#, Python, OCI, AWS, Azure, and Kubernetes. Reported outcomes include sub-200 ms p95 at 5× peak load, 99.99% service availability, 50M+ daily events, under-one-minute freshness, 45% lower MTTR, zero data loss during regional failover, 90% of resilience defects caught before production, 35% lower p99 read latency, and 3× throughput headroom.

The work history supports the role’s operational scope with concrete examples of replicated data-plane services, Kafka partitioning and batching, explicit consistency/availability tradeoffs, fault-injection and brownout testing, OpenTelemetry, Prometheus/Grafana, Terraform, automated canary rollouts and rollback, encryption, IAM, tenant isolation, incident response, and engineer mentorship.

The portfolio includes the resume’s Keystone transactional metadata store and Strata fault-tolerant storage server, plus the projects and source/demo URLs specified by the user. Keystone demonstrates Raft replication, MVCC, tenant controls, failover, and fault validation; Strata focuses on write-ahead logging, checksummed replication, crash recovery, and backpressure.

## Company context

Oracle presents OCI as a distributed cloud: public cloud services plus dedicated, hybrid, multicloud, government/sovereign, and edge options. Oracle’s site states that OCI offers a common portfolio of 200+ cloud services across regions and describes deployments that allow cloud capabilities to operate in data centers and customer-controlled environments. The exact mix of service and placement matters to infrastructure engineering: data locality, operational boundaries, security controls, and failure behavior vary by deployment, while customers expect consistent service characteristics.

The official job description itself emphasizes the scale of the environment (>50 regions), mission-critical enterprise use, and the need to preserve reliability and security as OCI expands its cloud models. The portfolio therefore centers on the engineering evidence most relevant to that environment: predictable performance under load, durable state, safe updates, failure recovery, and observable operations.

## Primary sources

- [Oracle Careers — Principal Software Engineer (Hybrid), requisition 344713](https://careers.oracle.com/en/sites/jobsearch/job/344713/)
- [Oracle Cloud Infrastructure](https://www.oracle.com/cloud/)
- [Oracle Distributed Cloud](https://www.oracle.com/cloud/distributed-cloud/)
- [OCI services available across cloud regions](https://www.oracle.com/cloud/distributed-cloud/service-availability/)
