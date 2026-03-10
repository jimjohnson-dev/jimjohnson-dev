# Jim Johnson

Backend engineer focused on distributed systems, event-driven workflows, and data pipelines.

Most of my work sits at the boundaries where systems fail: service interfaces, retry semantics, concurrency, ordering guarantees, and cross-service data flow. I spend most of my time debugging behavior that only appears when multiple services interact under real workloads.

The large-scale systems I’ve worked on live in private company repositories. The public repositories here are mostly tooling, experiments, and internal instruments used to reason about systems and automate operational work.

* * *

## Systems Experience

**LTK**  
Distributed notification infrastructure delivering tens of millions of messages per week across push, email, SMS, and in-app channels.

**MyFitnessPal**  
Backend modernization and event ingestion pipelines supporting a 220M-user platform.

**2U**  
Reliability improvements across APIs, queues, caching layers, and search systems powering large-scale learning platforms.

**OSIsoft**  
Cloud-hosted telemetry ingestion pipelines processing industrial time-series data from distributed customer installations.

**Kraken Forge**  
Independent work building internal engineering tools and research instruments for operational analysis and automation.

* * *

## Engineering Interests

-   Distributed systems and workflow orchestration
-   Event-driven architectures and delivery guarantees
-   Reliability patterns (retry, backoff, idempotency)
-   Observability and production debugging
-   Data pipelines and ingestion systems
-   API client resilience and failure-aware integrations

* * *

## Selected Projects

### evidence-collector

A research instrument for aggregating public operational signals into a two-layer relational model.

Raw payload storage preserves original data for reprocessing. Normalized tables support cross-source analysis. Normalization rules are deterministic and idempotent, allowing safe reprocessing as new insights emerge.

Designed to remain intentionally simple: if manual analysis becomes easier than the system, the system should be retired.

Focus: data pipeline design, normalization architecture, failure isolation

* * *

### file-sanitization-toolkit

Python library for detecting and reversibly obfuscating sensitive data in files such as CSV, JSON, JSONL, and Markdown.

The system uses format-specific processors built on a shared base abstraction, hierarchical configuration, and reversible cryptographic mappings. A backup registry allows safe rollback when restoring sanitized data.

Focus: library architecture, extensibility, reversible transformations

* * *

### jira-team-insights-dev

Analytics tool that extracts issue metrics from Jira to support engineering team retrospectives and review conversations.

The client supports multiple authentication strategies with fallback, configurable rate limiting, retry logic, and structured logging. Configuration is intentionally separated from code to prevent credential leakage.

Focus: API client resilience, operational tooling

* * *

### public-mirror-template

Automation pipeline for creating sanitized public mirrors of private repositories.

The pipeline scans for secrets, sanitizes sensitive content, and synchronizes the cleaned repository to a public mirror after an approval gate. The template includes automated validation to ensure sanitized mirrors remain functional.

Focus: security automation, CI/CD pipelines

* * *

### systems-rfcs

A lightweight RFC system for tracking engineering design decisions.

Each RFC must define the decision trigger, non-goals, kill criteria, and review date before implementation work begins. The goal is to preserve architectural reasoning over time.

Focus: architectural decision management

* * *

### resume-experience-tracker

Small Go service for managing structured career data with a simple REST API and React frontend.

The backend uses clear separation between handlers, storage, and models, along with Swagger documentation and structured file handling for attachments.

Focus: REST API design and service structure

* * *

## Typical Stack

Most projects here use a fairly conventional backend stack.

Languages  
Go, Python, TypeScript, C#

Infrastructure and data  
Relational databases, containerized services, REST APIs, and cloud messaging systems

Tooling  
Docker, GitHub Actions, and standard CLI automation

These tools change depending on the system. The focus is always on system behavior and reliability rather than any specific framework.

* * *

## Contact

LinkedIn  
[https://linkedin.com/in/johnson-james-m](https://linkedin.com/in/johnson-james-m)

Email  
[jmjohnson117@gmail.com](mailto:jmjohnson117@gmail.com)

