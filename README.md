# Jim Johnson

Backend and distributed systems engineer with 20+ years building and operating high-throughput, event-driven platforms. Most recently owned a notifications platform delivering 50M messages per week — redesigned its architecture to eliminate 963M annual webhook sends and cut messaging costs by 56%, and led the Retailer Affinity experiment that generated $11M in annualized GMV within two weeks of rollout.
Most of my production work lives in private company repositories. The public repositories here are tooling, experiments, and instruments I use to reason about systems and automate operational work. They reflect how I think about problems, not the scale I've operated at.

* * *

## Systems Experience

**LTK**  
Distributed notification infrastructure delivering tens of millions of messages per week across push, email, SMS, and in-app channels. Redesigned delivery paths to eliminate 963M annual webhook sends and reduce messaging costs by **56%**.

**MyFitnessPal**  
Backend modernization and event ingestion pipelines supporting a 220M-user platform. Owned the microservices migration that improved deployment latency by **25%** and increased fault isolation across the service fleet.

**2U**  
Reliability improvements across APIs, queues, caching layers, and search systems powering large-scale learning platforms. Designed and launched an **AI-based transcript translation pipeline** supporting **11 languages**.

**OSIsoft**  
Cloud-hosted telemetry ingestion pipelines processing industrial time-series data from distributed customer installations. Built observability tooling that reduced mean time to resolve production issues by **30%**.

**Kraken Forge**  
Independent work building healthcare workflow systems and internal engineering tools. Delivered a patient assignment system and discharge coordination platform now in active use across hospital shifts.

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

