# Awesome-API-Request-History-Audit-Logging

A curated list of awesome API request history, logging, and audit trail platforms, frameworks, and tools.

---

## Sector Overview & Market Dynamics

The API request history, log management, and audit logging sector is currently valued at approximately **$3.3B to $4.1B** (within the broader **$18B+** cloud observability, SIEM, and data intelligence market) and is projected to expand to **$6.5B to $10B+** at an estimated CAGR of 12–15%. The market is **moderately concentrated at the enterprise infrastructure layer**—dominated by mega-cap cloud providers (AWS) and unified observability giants (Datadog, Splunk/Cisco)—yet **fragmented at the application and developer tooling layer**, where modern entrants (Better Stack, Coralogix) compete aggressively on consumption economics, hot/cold decoupled storage, and developer experience.

---

## SaaS Products

The table below lists leading SaaS platforms providing API request logging, audit tracking, and centralized log management. The table is sorted in descending order by company size (valuation / market capitalization / revenue).

| Product | Company Size (Valuation / Revenue) | Pricing (Starting Tier) | Free Tier / Free Trial Limits | Key Capabilities |
|---|---|---|---|---|
| **AWS CloudTrail** | Parent Market Cap: **~$2.1T+** / AWS Annual Revenue: **~$105B+** | **$0.10 per 100,000 data events**; additional management event copies at **$2.00 per 100,000 events** | **Free forever plan**: View/filter past 90 days of management events free in Event History; first copy of ongoing management events delivered to S3 is free. CloudTrail Lake offers a 30-day free trial (up to 5 GB ingestion & 5 GB scan). | Comprehensive API audit logging across all AWS services and infrastructure; immutable event history. |
| **Datadog** | Market Cap: **~$65B** / Annual Revenue: **~$4.5B** | **$0.10/GB ingested** + **$1.06 per 1 million events** indexed (3-day retention, annual commitment; or ~$1.27/M for 7-day) | **14-day free trial** with full access to log ingestion, live tail, and indexing features (standard free tier covers infrastructure metrics only up to 5 hosts, excluding full log search). | Full-stack observability, unified API log ingestion, trace correlation, real-time alerting, and automated anomaly detection. |
| **Splunk Cloud Platform** | Valuation: **$28B** (Acquired by Cisco) / Annual Revenue: **~$3.8B–$4B** | **~$1,800 to $2,500 per GB/day annually** (approx. starting list ingest price; workload pricing also available based on SVC units) | **14-day free trial** with a limit of **5 GB per day** ingestion (self-hosted Splunk Free offers perpetual 500 MB/day indexing). | Enterprise-scale log aggregation, SIEM security compliance, sophisticated SPL search, and high-throughput audit indexing. |
| **Papertrail** | Valuation: **$4.4B** (SolarWinds acquisition by Turn/River) / SolarWinds Revenue: **~$797M** | Starts at **$7.00/month** for 1 GB/month (includes 1 week search and 1 year archive) | **Free forever plan**: **50 MB per month** transfer, **48 hours** search retention, **7 days** archive retention, unlimited systems and users. | Lightweight, instant-setup cloud log management with live-tail streaming search and fast regex querying. |
| **Sumo Logic** | Valuation: **$1.7B** (Acquired by Francisco Partners) / Revenue: **~$242M** | **Flex Pricing**: **$0/GB ingest**, pay-per-TB scanned estimated at **$3.14/TB scanned** (entry packages start around ~$297/month) | **30-day free trial** with full platform capabilities; perpetual free tier provides **500 MB/day** ingestion, **7-day** retention, and up to **3 users**. | Cloud-native analytics, automated threat detection, audit compliance dashboards, and Flex scan-based pricing. |
| **Coralogix** | Valuation: **$1.6B** (Series F) / Annual Revenue: **~$90M+** | **$1.50 per unit** (Logs: **$0.42 to $1.15 per GB** based on priority tier; 0.12–0.75 units/GB) | **14-day free trial** with full access to all features, capped at **8 Coralogix Units (CXUs)** (~$12 worth of data pipeline processing). | Streama real-time stream analysis without indexing, long-term archive querying, and automated cost-optimization pipelines. |
| **Better Stack** | Valuation: **~$40M–$60M** (Series A) / Annual Revenue: **~$3.5M–$4M** | **$25/month** billed annually ($30/month monthly) for the Nano plan (40 GB storage, $0.10/GB extra ingestion) | **Free forever plan**: **3 GB logs/month** (3-day retention), **3 GB traces/month**, **30 GB metrics/month**, up to **10 monitors**, Slack/email alerts. | Modern ClickHouse-powered developer-friendly log management, unified telemetry, uptime monitoring, and built-in incident management. |

---

## Open-Source & Self-Hosted Solutions

For teams needing on-premise deployment, data sovereignty, or open-source infrastructure:

| Project | License | GitHub Stars | Description |
|---|---|---|---|
| **Graylog** | Open Source (GPL / SSPL) | ~7,200+ | Fast, centralized log management platform with Elasticsearch/OpenSearch indexing, alerting, and audit dashboards. |
| **Elastic Logstash** | Open Source (Apache 2.0 / Elastic) | ~14,000+ | Server-side data processing and log ingestion pipeline that ingests data from multiple sources simultaneously, transforms it, and ships it to Elasticsearch. |
| **Fluent bit / Fluentd** | Open Source (Apache 2.0 - CNCF Graduated) | ~16,000+ | High-performance, lightweight log processor and forwarder for collecting API events and distributing them across cold storage and analytics backends. |
| **Signoz** | Open Source (Apache 2.0 / MIT) | ~19,000+ | Open-source alternative to Datadog providing native OpenTelemetry support, log aggregation, and distributed tracing on ClickHouse. |
