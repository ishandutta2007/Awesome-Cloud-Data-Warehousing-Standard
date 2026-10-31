# Awesome-Cloud-Data-Warehousing-Standard

# Awesome-Cloud-Data-Warehousing-Standard

**Top Cloud Data Warehousing Standard (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Serverless Warehouses, Pay-Per-Query Models, MPP Engines & Self-Hosted Analytical Databases*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Data Warehousing – Standard**. These tools enable organizations to analyze data at scale with predictable or consumption-based pricing—from fully managed serverless warehouses that charge only for what you use to open-source MPP engines that give teams complete control over their analytical infrastructure and cost model.



**Examples** include Snowflake Standard Edition, Amazon Redshift Serverless, Google BigQuery, Azure Synapse Serverless, ClickHouse Cloud, Rockset, Firebolt, SingleStore Helios, and PostgreSQL-based cloud options (the category leaders in commercial space). **Note**: Panoply was referenced in the original request, but current search results identify it as a NASA data visualization tool, not a cloud data warehouse—it has been excluded.



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted analytical databases, MPP engines, and open lakehouse query infrastructure. **Critical note**: The open-source data warehouse landscape is genuinely viable—**Apache Doris** and **StarRocks** offer production-grade MPP with sub-second latency, **ClickHouse** dominates real-time single-table analytics, and **Apache Cloudberry** provides a PostgreSQL-compatible MPP successor to Greenplum. No open-source engine matches Snowflake's fully managed elasticity or BigQuery's serverless simplicity, but for teams willing to operate infrastructure, the analytical engines are competitive at scale.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global Cloud Data Warehousing market is estimated at approximately **$15.8B – $16.5B in 2026** (scaling from ~$12.5B in 2025 at a CAGR of ~22–26% toward over $50B+ in the 2030s). The sector exhibits a **moderately concentrated oligopoly at the top**—dominated by the three hyperscalers (Microsoft, Alphabet/Google, Amazon AWS) and independent powerhouse Snowflake—flanked by a vibrant, **fragmented long-tail** of specialized real-time engines (ClickHouse, SingleStore, Firebolt) and open lakehouse formats (Iceberg, Delta Lake) that prevent a single winner-take-all outcome.

## SaaS/Hosted Platforms

| Platform | Parent Company / Backing | Valuation / Market Cap | Starting Paid Pricing | Free Tier / Trial Limits | Description & Key Strengths |
|---|---|---|---|---|---|
| **[Azure Synapse Serverless SQL](https://azure.microsoft.com/en-us/products/synapse-analytics)** | Microsoft | ~$3.9T Market Cap (FY26 revenue ~$245B+) | $5.00 per TB scanned (pay-per-query, 10 MB minimum per query) | Free trial only: 30 days with $200 Azure credits; no permanent free tier | On-demand lakehouse query service executing T-SQL across ADLS Gen2/Blob storage; zero compute provisioning with automatic scaling. |
| **[Google BigQuery](https://cloud.google.com/bigquery)** | Alphabet (Google) | ~$3.5T – $3.9T Market Cap (FY25 revenue ~$350B+) | $6.25 per TiB scanned (On-Demand) or $0.04 per slot-hour (Standard Edition capacity) | Free forever: 1 TiB queries/mo and 10 GB active storage; new users get 90-day $300 GCP credit | Fully serverless multi-cloud analytical warehouse; decouples compute and storage with built-in ML and seamless Google ecosystem integration. |
| **[Amazon Redshift Serverless](https://aws.amazon.com/redshift/)** | Amazon (AWS) | ~$2.6T – $2.7T Market Cap (FY25 revenue ~$638B+) | $0.375 per RPU-hour (billed per second, 60s minimum; base capacity starts at 4 RPUs) | Free trial: $300 trial credit for 90 days for new Serverless accounts; no permanent serverless free tier | Serverless edition of AWS Redshift automatically scaling data warehouse capacity with zero idle charges and native AWS lake integrations. |
| **[Rockset](https://rockset.com/)** | OpenAI | ~$852B Valuation ($13B+ ARR) | $0.32/compute-unit-hour (~$232/month entry baseline) | Free trial only: 14-day free trial with full feature access and cloud connectors; no permanent free tier | Real-time search and analytics database with compute-compute separation and vector/hybrid indexing; acquired by OpenAI to power real-time AI workloads. |
| **[Snowflake Standard Edition](https://www.snowflake.com/pricing-options/)** | Snowflake Inc. | ~$107B – $110B Market Cap (FY26 revenue ~$3.6B+) | $2.00 per credit (AWS US East; virtual warehouse compute billed per second, 60s minimum) | Free trial only: 30-day free trial with $400 usage credits; no permanent free tier | Multi-cluster shared-data analytical warehouse separating storage and compute with instant auto-resume, Snowpark, and native data sharing. |
| **[ClickHouse Cloud](https://clickhouse.com/cloud)** | ClickHouse Inc. | $15B Valuation ($250M+ ARR) | $0.2181 per compute-unit-hour (Basic Tier, AWS us-east-1) + $25.30/TB compressed storage/mo | Free trial only: 30-day free trial with $300 credits; no permanent managed free tier (engine is open source) | Fully managed columnar OLAP platform offering sub-second queries on wide tables, ClickPipes managed ingestion, and compute separation. |
| **[Firebolt](https://www.firebolt.io/)** | Firebolt Inc. | $1.4B Valuation (~$40M ARR) | $0.92 – $1.00 per engine node/hour (compute billed per second) + $27/TB compressed storage/mo | Free forever plan: Firebolt Core is free forever for self-managed deployments; Cloud offers 14-day / $200 trial credit | Decoupled cloud data warehouse engineered for sub-second, low-latency aggregations and user-facing dashboards at high concurrency. |
| **[Timescale Cloud / Managed PostgreSQL](https://www.postgresql.org/)** | TigerData (formerly Timescale) | $1.0B+ Valuation | $30 – $36/month minimum baseline compute ($0.042/hour micro instances) | Free forever plan: 750 MB free storage database (switches to read-only when full); 30-day Performance trial | Managed cloud service extending PostgreSQL with hypertables, automatic columnar compression, continuous aggregates, and tiered object storage. |
| **[SingleStore Helios](https://www.singlestore.com/cloud-pricing/)** | SingleStore Inc. | ~$1.0B Valuation (~$123M ARR) | $3.96 per credit on-demand (Standard tier 1x multiplier, ~1 credit/hour for small sizes) | Free forever plan: Free Shared Tier / Starter Workspace with 1 GB compressed storage (~4 GB raw data) and 1 attached database | Real-time distributed SQL database combining in-memory OLTP and columnar OLAP (HTAP) for operational analytics and fast transactional ingestion. |

## Open-Source GitHub Projects



- **[Apache Doris](https://github.com/apache/doris)**

  **High-performance, real-time analytical database based on MPP architecture** (Apache 2.0) — **the most balanced open-source MPP engine** for unified real-time and batch analytics, returning sub-second results over massive datasets with 10,000+ QPS concurrency. **Features**: Columnar storage with multiple index types (Sorted Compound Key, Min/Max, BloomFilter, inverted, vector); multiple storage models (Duplicate, Aggregate, Unique with row-level updates); materialized views (single-table and multi-table); MySQL protocol compatibility; hybrid search with vector and full-text indexes. **Architecture**: Integrated storage-compute or decoupled storage-compute (shared S3/HDFS/OSS). **Tech stack**: C++, Java. **Deploy**: Self-hosted. **Trade-off**: Lake integration less mature than StarRocks; not designed for extreme single-table aggregation. **Best for**: enterprise reporting and ad-hoc analytics needing high concurrency and real-time updates—especially MySQL-centric environments.



- **[StarRocks](https://github.com/StarRocks/starrocks)**

  **Next-generation MPP database for all-scenario analytics** (Apache 2.0, Linux Foundation) — **the most performance-optimized open-source MPP engine for multi-table joins and lakehouse queries**, with a fully vectorized engine and new CBO optimizer. **Features**: Multi-Catalog reads Iceberg/Hudi/Delta/Paimon directly; asynchronous incremental materialized views; Primary Key model for real-time updates; MySQL protocol. **Performance**: Reported **3x–5x faster than Trino** on TPC-H benchmarks. **Architecture**: Shared-nothing or shared-data. **Tech stack**: C++, Java. **Deploy**: Self-hosted. **Trade-off**: Acceleration layer, not source of truth; steeper learning curve than ClickHouse. **Best for**: teams with lakehouse architecture needing sub-second BI performance and high concurrency on Iceberg/Hudi/Delta data.



- **[ClickHouse](https://github.com/ClickHouse/ClickHouse)**

  **Column-oriented database for real-time analytics** (Apache 2.0) — **the fastest open-source engine for single-table aggregation and log analytics**. **Features**: MergeTree engine family with rich indexing and partitioning; vectorized execution; excellent for logs, time-series, and wide-table aggregations. **Tech stack**: C++. **Deploy**: Self-hosted or ClickHouse Cloud. **Trade-off**: Weak JOIN performance; not suitable for high-frequency updates; lake integration weaker than StarRocks/Doris. **Best for**: log analysis, user behavior analytics, and read-heavy single-table aggregation.



- **[Apache Cloudberry (Incubating)](https://github.com/apache/cloudberry)**

  **Open-source MPP database for large-scale analytics and AI** (Apache 2.0) — **the successor to Greenplum**, derived from the last open-source version and now under Apache governance. **Features**: PostgreSQL 14 foundation with distributed query planning; **PAX storage format** (hybrid row/column); **dynamic tables** for automatic scheduled refresh; ORCA optimizer improvements; MCP server for AI workflow integration. **Tech stack**: C, PostgreSQL 14. **Deploy**: Self-hosted. **Trade-off**: Incubating project—still maturing; PostgreSQL kernel upgrade in progress. **Best for**: organizations migrating from Greenplum or needing PostgreSQL-compatible MPP with active open-source development.



- **[Apache Druid](https://github.com/apache/druid)**

  **Real-time analytics database** (Apache 2.0) — **the open-source engine for interactive dashboards on streaming data**. **Features**: Time-series optimized columnar storage; real-time ingestion from Kafka/Kinesis; sub-second queries on billions of rows; built-in rollup for pre-aggregation. **Tech stack**: Java. **Deploy**: Self-hosted or Imply Cloud. **Trade-off**: Not a general-purpose warehouse—best for time-series and event data with known query patterns. **Best for**: operational dashboards and real-time analytics on streaming event data.



- **[Apache Pinot](https://github.com/apache/pinot)**

  **Real-time distributed OLAP datastore** (Apache 2.0) — **the engine powering user-facing analytics at LinkedIn, Uber, and Stripe**. **Features**: Columnar storage with inverted indexes; real-time ingestion from Kafka; sub-second queries at high concurrency; upsert support for mutable data. **Tech stack**: Java. **Deploy**: Self-hosted or StarTree Cloud. **Trade-off**: Operational complexity—requires ZooKeeper, controller, broker, and server components. **Best for**: user-facing analytics products needing millisecond query latency at scale.



### Additional Strong Open-Source Options



- **Trino** — Distributed SQL query engine for federated analytics (Apache 2.0). Queries HDFS, Hive, Kafka, MySQL, PostgreSQL, Iceberg, Delta, and more; no storage of its own. **Note**: Query engine only—no storage or materialized views. **Best for**: organizations with data scattered across systems needing a unified SQL interface.

- **Apache Iceberg** — Open table format (Apache 2.0). The de facto standard for open lakehouse storage; enables multiple engines to query the same tables. **Note**: Table format only—needs catalog (Polaris/Nessie) and storage (S3/MinIO). **Best for**: building vendor-neutral lakehouse architecture.

- **Greenplum** — Mature PostgreSQL-based MPP (Apache 2.0). Proven at petabyte scale but aging; **Apache Cloudberry** is the active successor. **Note**: For new deployments, evaluate Cloudberry. **Best for**: organizations with existing Greenplum investment.



**Frameworks for building custom systems**: Combine **MinIO** or S3 for storage with **Apache Iceberg** as the table format, **StarRocks** or **Apache Doris** as the query engine, and **ClickHouse** or **Druid** for real-time analytics—creating an open-source data warehouse stack. **None of these match Snowflake's managed elasticity or BigQuery's serverless simplicity**, but for teams prioritizing cost control and vendor independence, the open engines are production-viable at scale.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Cloud data warehousing platforms handling enterprise data must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls, encryption, and audit logging.

- **The "standard edition" vs. "serverless" vs. "self-hosted MPP" distinction is critical.** **Snowflake Standard** is the entry-level edition of a multi-cluster shared-data platform—core features but no multi-cluster compute or extended governance . **Redshift Serverless** and **BigQuery** are **serverless**—no infrastructure to manage; pay per use . **Azure Synapse Serverless** is a **query service over the lake**—not a full warehouse; no DML . **ClickHouse Cloud, Rockset, Firebolt, and SingleStore Helios** are **managed analytical databases**—consumption or credit-based. **Apache Doris, StarRocks, ClickHouse, and Cloudberry** are **self-hosted MPP engines**—you own operations. **Choose based on whether you need managed convenience, serverless elasticity, or full control.**

- **BigQuery Standard Edition is limited.** It lacks BI Engine acceleration, cross-user caching, advanced workload management, and managed disaster recovery—features that production BI workloads typically require . **Do not assume Standard Edition is sufficient for dashboard-heavy use cases**; validate against Enterprise-tier requirements.

- **Azure Synapse Serverless is not a full data warehouse.** It supports SELECT queries over lake files but **does not support DML** (INSERT/UPDATE/DELETE) . **It is a query service for exploration and logical data warehousing**, not a replacement for a provisioned warehouse when you need to transform and persist data.

- **Rockset's compute-compute separation is a genuine differentiator**—decoupling indexing from query compute lets different clusters share the same real-time data without interference . **Firebolt Core** offers a free self-managed path for teams wanting Firebolt's engine without cloud commitment .

- **Apache Doris and StarRocks are the strongest open-source MPP choices.** Doris offers balanced real-time and batch analytics with both integrated and decoupled architectures. StarRocks is the performance leader for multi-table joins and lakehouse queries, reporting 3x–5x faster than Trino on TPC-H . **Choose Doris for balanced workloads; choose StarRocks for join-heavy and lakehouse scenarios.**

- **Pricing opacity varies.** Snowflake publishes $2.00/credit for Standard . Redshift Serverless is RPU-based with reservation discounts . BigQuery has on-demand and Editions pricing . Synapse Serverless is per-TB-processed . ClickHouse Cloud and Firebolt publish consumption-based pricing . SingleStore publishes credit rates . **Validate with direct vendor conversations against your actual query volume and concurrency requirements.**

- Self-hosted open-source solutions require proper infrastructure (compute clusters, object storage, catalog services), security hardening, and ongoing maintenance. **Data warehouse engines are business-critical**—ensure your deployment meets your organization's reliability and security requirements before migrating production analytical workloads.



---



**Made for data engineers, analytics teams, and organizations building transparent cloud data warehousing solutions.**

Let's make Cloud Data Warehousing Standard more open, data-driven, and cost-transparent.
