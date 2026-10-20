![Ana Nurkaromah](img/github-header-banner.png)


###### Data engineer with 6+ years in environmental engineering and industrial consulting. Skilled in Python, SQL, dbt, Docker, and Databricks, trained through DataTalksClub Zoomcamp 2026 and DataExpert.io
---

## Skills & Tools
- **Languages:** Python, SQL
- **Data engineering:** ETL/ELT, batch ingestion, REST APIs, idempotent loading (UPSERT), incremental models, historical backfill, deduplication, data validation, data reconciliation
- **Data quality and monitoring:** dbt tests, uniqueness and not-null checks, failure alerting (Discord webhooks), CI checks
- **Databases and warehouses:** PostgreSQL, BigQuery
- **Transformation and orchestration:** dbt, Apache Airflow, Bruin
- **Cloud and DevOps:** Google Cloud Platform (GCS, BigQuery), Terraform, Docker, Docker Compose, Git, GitHub Actions
- **Data modeling and BI:** Medallion (bronze/silver/gold) architecture, dimensional modeling, fact tables, Metabase, Looker Studio
- **Familiar with (training and early-stage projects):** Apache Spark/PySpark, Kafka, Kestra, dlt, Databricks, Supabase, pgvector, embeddings, RAG

---

## Projects & Portfolio

### - UK Property ELT Pipeline | uk-estate-pipeline 
<a href="https://github.com/ananurkaromah/uk-estate-pipeline">Repo</a>

**Tech Stack:** Apache Airflow, PostgreSQL, dbt, Docker, Metabase.
<br>**Highlights:**
- Developed an Airflow + dbt ELT pipeline loading HM Land Registry Price Paid Data, ONS NSPL and postcodes.io into a bronze/silver/gold PostgreSQL warehouse, with monthly updates and a 2021-2025 historical backfill (5.2 million transactions).
- Diagnosed data loss (row counts decreasing because the source file is not cumulative) and solved it with an idempotent UPSERT and an incremental dbt model.
- Increased geographic coverage from 94.8% to 99.99% by fixing an ingestion defect (1 of 150 NSPL files) and adding ONS-first postcode reconciliation.
- Added failure alerting (Discord webhook), atomic reference-table reloads, dbt data quality tests and GitHub Actions CI that builds the Airflow and dbt images and tests the dbt project on every push; verified end to end with a clean clone-and-run.
- Delivered a three-tab Metabase dashboard on the gold layer (data quality KPIs, price trends and top districts by CAGR, segmentation by property type), flagging price outliers above £10M and applying minimum-sample rules to keep metrics reliable.

### - Remote Data Engineer ETL Pipeline | remote-job-pipeline
<a href="https://github.com/ananurkaromah/remote-job-pipeline">Repo</a>

**Tech Stack:** Python, PostgreSQL (Supabase, pgvector), GCS, GitHub Actions
<br>**Highlights:**
- Automated daily ingestion from four job-board APIs with Python and GitHub Actions, using per-source failure isolation, quota-aware degradation and Discord monitoring that reports skipped records.
- Used content-addressed job IDs for upsert semantics, so reruns are deterministic and cross-source duplicates are removed.
- Designed a tri-state eligibility classifier (eligible, restricted, unknown) validated on a hand-labeled set covering geographic and visa restrictions.
- Added hybrid semantic and SQL job search with pgvector, a PostgreSQL RPC function and bge-small-en-v1.5 embeddings.
- Traced a 47-minute CI build hang to Docker Hub rate limiting and fixed it by switching to the AWS ECR Public base image and pinning ML dependencies.


### - Indonesian Regional Speech Intelligence Pipeline | suara-pipeline

<a href="https://github.com/ananurkaromah/suara-pipeline">Repo</a>

**Tech Stack:** Python, BigQuery, GCS, Terraform, Docker, Bruin, Faster-Whisper, Looker Studio
<br>**Highlights:**
- Provisioned a GCS data lake and a BigQuery warehouse using Terraform to process a 10GB+ speech dataset with 5 different Indonesian accents.
- Built a Bruin DAG that loads audio metadata into BigQuery, transcribes speech with faster-whisper and enforces NOT NULL and UNIQUE checks.
- Optimized the BigQuery warehouse with date partitioning and clustering by file name, and made GCS uploads idempotent by skipping files already uploaded.
- Transcribed a 117-record sample, storing transcript, duration and model metadata, and visualized accent distribution and ingestion volume in Looker Studio.

### - AI-Powered Job Hunting Copilot | agentic-job-search |  DataExpert.io Capstone
<a href="https://github.com/ananurkaromah/agentic-job-search">Repo</a>

**Tech Stack:** Python, Databricks, Lakebase, Vector Search, RAG, AI Agents, REST API, MCP, Databricks Apps.
<br>**Highlights:**
- Built a prototype that loads job data with PySpark into Lakebase Postgres and embeds postings in pgvector for RAG-style job-to-skill matching.
- Deployed as Databricks Apps: a Flask dashboard and a tool server for job search and matching.

### - NYC Taxi-pipeline (GitHub Repo) | DataTalksClub Homework Project
<a href="https://github.com/ananurkaromah/nyc-taxi-data-pipeline-with-dlt">Repo</a>

**Tech Stack:** Python, DuckDB, Docker, dlt, Metabase
<br>**Highlights:**
- Built automated ELT workflows for ingesting and analyzing NYC Taxi data.
- Implemented incremental loading patterns and data transformations.
- Created analytics dashboards to support operational insights.
- Managed containerized environments using Docker Compose

*Continuously building more real-world data engineering projects...*

---
## Fun & Personal

- I enjoy **learning new technologies and exploring the data ecosystem**
- Problem solver — I enjoy debugging pipelines and solving technical challenges
- Always curious — constantly learning something new in **data engineering**

Open to Data Engineering Internships & Opportunities

---

## Connect with Me

- <a href="https://linkedin.com/in/ananurkaromah">LinkedIn</a>
- <a href="https://discord.com/users/1462129586459644118">Discord</a>
