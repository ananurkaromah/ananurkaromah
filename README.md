![Ana Nurkaromah](img/github-header-banner.png)


###### Data engineer with 6+ years in environmental engineering and industrial consulting. Skilled in Python, SQL, dbt, Docker, and Databricks, trained through DataTalksClub Zoomcamp 2026 and DataExpert.io
---

## Skills & Tools
- Databases: PostgreSQL, BigQuery, Lakebase
- Programming: SQL, Python
- Data Engineering & Platforms: dbt, Apache Spark, PySpark, Kestra, Apache Airflow, Kestra, GitHub Actions
- AI & Data Applications: Vector Search (via pgvector), RAG, MCP, AI Agents, Databricks Apps
- Cloud & Infrastructure: Databricks, Google Cloud Platform, Docker, Terraform
- Analytics & Visualization: Metabase, Looker Studio
- Version Control: Git, GitHub

---

## Projects & Portfolio

### UK Property ELT Pipeline | uk-estate-pipeline 
<a href="https://github.com/ananurkaromah/uk-estate-pipeline">Repo</a>

**Tech Stack:** Apache Airflow, PostgreSQL, dbt, Docker, Metabase.
**Highlights:**
- Developed ELT pipeline in Airflow to transfer HM Land Registry Price Paid Data, ONS NSPL and postcodes.io data into a Bronze/Silver/Gold data warehouse, backfilling 5.2 million transactions.
- Diagnosed data loss (row counts decreasing because the source file is not cumulative) and solved by using an idempotent UPSERT in conjunction with an incremental dbt model.
- Increased geographic coverage from 94.8% to 99.9% by fixing an ingestion defect (1/150 NSPL files), and adding ONS-first postcode reconciliation.
- Added failure alerting (Discord webhook), atomic reference-table reloads, dbt data quality tests, and GitHub Actions to build Airflow and dbt images, and test the dbt project, on every push.

### Remote Data Engineer ETL Pipeline | remote-job-pipeline
<a href="https://github.com/ananurkaromah/remote-job-pipeline">Repo</a>

**Tech Stack:** Python, PostgreSQL (Supabase, pgvector), GCS, GitHub Actions
**Highlights:**
- Automated ingestion from four external job board APIs using Python and GitHub Actions with per-source failure isolation and quota-aware degradation.
- Used content-addressed job IDs to achieve upsert semantics to achieve deterministic loading to eliminate duplicates when safe reruns occurred. Also achieved cross-source deduplication.
- Designed and validated a tri-state eligibility classifier using a hand-labeled evaluation set based on geographic and visa restrictions.
- Increased reliability through 67 automated unit tests, 25 architecture decision records, least-privilege database access, and three-tier Discord webhook monitoring; resolved and diagnosed incidents with API and CI/CD registry.
- Added hybrid semantic and SQL job search through the use of pgvector, a postgreSQL RPC function, and bge-small-en-v1.5 embeddings.

### Indonesian Regional Speech Intelligence Pipeline | suara-pipeline

<a href="https://github.com/ananurkaromah/suara-pipeline">Repo</a>

**Tech Stack:** Python, BigQuery, GCS, Terraform, Docker, Bruin, Faster-Whisper, Looker Studio
**Highlights:**
- Provisioned a GCS data lake and a BigQuery warehouse using Terraform to process a 10GB+ speech dataset with 5 different Indonesian accents.
- Designed and implemented a Bruin DAG to extract data from BigQuery, load it to a SQL table and transcript it, and perform NOT NULL and UNIQUE checks.
- Made the BigQuery warehouse more organized by partitioning by date and clustering by file name; made GCS uploads idempotent by skipping over already uploaded files.
- Extracted audio data, transcripted it, encoded transcription duration, and speech model metadata, for 117 records. Moreover, visualized accent distribution and ingestion volume using Looker Studio.


### AI-Powered Job Hunting Copilot | agentic-job-search |  DataExpert.io Capstone
<a href="https://github.com/ananurkaromah/agentic-job-search">Repo</a>

**Tech Stack:** Python, Databricks, Lakebase, Vector Search, RAG, AI Agents, REST API, MCP, Databricks Apps.
**Highlights:**
- Built an AI job search application using lakebase to structure relational data in a lakehouse design, and used Databricks Vector Search for semantic retrieval.
 - Created RAG-based matching of job reqs to candidate skills, and provided agent tools for job discovery, matching, and application through a set of REST APIs.
 - Combined and integrated the data, retrieval, and agent workflow, and deployed it as a Databricks App.


### NYC Taxi-pipeline (GitHub Repo) | DataTalksClub Homework Project
<a href="https://github.com/ananurkaromah/nyc-taxi-data-pipeline-with-dlt">Repo</a>

**Tech Stack:** Python, DuckDB, Docker, dlt, Metabase
**Highlights:**
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
