![Ana Nurkaromah](img/github-header-banner.png)


#### Career switcher transitioning from 6+ years in environmental engineering and industrial consulting into data engineering, backed by structured training (DataTalksClub Zoomcamp, DataExpert.io) and three end-to-end portfolio projects covering ELT pipelines, cloud data platforms, and AI-enabled applications. Hands-on with Python, SQL, PostgreSQL, Docker, Airflow, dbt, and Databricks. Brings strong analytical rigor, technical documentation, and problem-solving habits carried over from a prior engineering and research career, now applied to building and shipping production-style data pipelines.
<br>

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

### remote-jobs-pipeline | Remote Job Semantic Pipeline (Open-Source Project) 
🔗 <a href="https://github.com/ananurkaromah/remote-jobs-pipeline">Repo</a>[GiHub Repo]

**Tech Stack:** Python, PostgreSQL (Supabase, pgvector), GCS, GitHub Actions
**Highlights:**
-	Designed and built an end-to-end serverless ETL pipeline to ingest remote job postings from multiple APIs and web scrapers, automating daily execution via GitHub Actions.
-	Implemented data cleaning, automated currency normalization (to USD), and heuristic geographic filtering to isolate roles globally and regionally accessible from Indonesia.
-	Generated vector embeddings using HuggingFace SentenceTransformers (bge-small-en-v1.5) with structured text templating.
-	Upserted normalized metadata and vector arrays into Supabase (pgvector) using an idempotent architecture, enabling advanced hybrid search for LLM-powered job matching.


### uk-estate-pipe |🏡 UK Real Estate ELT Pipeline 
🔗 <a href="https://github.com/ananurkaromah/uk-estate-pipeline">Repo</a>

**Tech Stack:** Apache Airflow, PostgreSQL, dbt, Docker, Metabase.
**Highlights:**
-	Built a containerized ELT pipeline ingesting 2.9M+ raw rows across 3 UK property/geographic sources (2.73M ONS postcode records, 101K HM Land Registry transactions, 88K Postcode.io records) into a medallion-architecture (bronze/silver/gold) warehouse.
-	Designed PostgreSQL schemas and Python ingestion scripts for CSV, REST API, and zip-archived sources.
-	Built a dbt source-reconciliation layer resolving 101.240 of 101.334 property transactions (99.99%) against postcode reference data, matching primarily on the ONS dataset with a Postcode.io fallback path for conflict resolution.
-	Implemented automated data quality tests (uniqueness, not-null, accepted-values) as a pipeline gate.
-	Orchestrated ingest-transform-test workflows with Airflow, fully containerized via Docker Compose.
-	Delivered a gold-layer fact table of 101.334 property transactions across 363 regions, powering a self-hosted Metabase BI layer for pricing and regional trend analysis.


### jobhunt-ai-agent  |  AI-Powered Job Hunting Copilot |  DataExpert.io Capstone
🔗 <a href="https://github.com/ananurkaromah/agentic-job-search">Repo</a>

**Tech Stack:** Python, Databricks, Lakebase, Vector Search, RAG, AI Agents, REST API, MCP, Databricks Apps  

**Highlights:**
-	Built an AI-powered job hunting application combining structured and unstructured data retrieval with agentic workflows.
-	Designed a lakehouse-based architecture using Lakebase for relational application data and vector search for semantic retrieval.
-	Implemented RAG-based job matching to connect job requirements with candidate skills and experience.
-	Developed AI agent tools for job discovery, matching, and application management through REST APIs.
-	Built and deployed the application as a Databricks App, integrating data, retrieval, and AI agent components into a unified workflow.
-	Applied context engineering and tool-based agent design to provide grounded, actionable job-search recommendations.



### uk-estate-pipeline | UK Real Estate ELT Pipeline 
🔗 <a href="https://github.com/ananurkaromah/uk-estate-pipeline">Repo</a>

**Tech Stack:** Apache Airflow, PostgreSQL, dbt, Docker, Metabase.
**Highlights:**
-	Built a containerized ELT pipeline integrating 3 UK property/geographic data sources into a medallion-architecture (bronze/silver/gold) warehouse
-	Designed PostgreSQL schemas and Python ingestion scripts for CSV, REST API, and zip-archived sources
-	Built dbt models with a source-reconciliation layer resolving conflicts between two postcode reference datasets
-	Implemented automated data quality tests (uniqueness, not-null, accepted-values) as a pipeline gate
-	Orchestrated ingest-transform-test workflows with Airflow, fully containerized via Docker Compose
-	Delivered a self-hosted Metabase BI layer for pricing and regional trend analysis


### suara-pipeline | Indonesian Regional Speech Intelligence Pipeline | DataTalksClub Capstone Project
🔗 <a href="https://github.com/ananurkaromah/suara-pipeline">Repo</a>

**Tech Stack:** Python, BigQuery, GCS, Terraform, Docker, Bruin, Looker Studio
**Highlights:**
- Built a cloud-native data platform processing 10GB+ of Indonesian regional speech data.
- Automated ingestion from Kaggle API into Google Cloud Storage and BigQuery.
- Developed incremental ingestion and transformation workflows.
- Integrated AI-powered transcription using Faster-Whisper models.
- Managed infrastructure provisioning using Terraform.
- Delivered analytics-ready datasets and dashboards using BigQuery and Looker Studio.
  

### NYC Taxi-pipeline (GitHub Repo) | DataTalksClub Homework Project
🔗 <a href="https://github.com/ananurkaromah/nyc-taxi-data-pipeline-with-dlt">Repo</a>

**Tech Stack:** Python, DuckDB, Docker, dlt, Metabase
**Highlights:**
- Built automated ELT workflows for ingesting and analyzing NYC Taxi data.
- Implemented incremental loading patterns and data transformations.
- Created analytics dashboards to support operational insights.
- Managed containerized environments using Docker Compose
---

*Continuously building more real-world data engineering projects...*

---
## Fun & Personal

- I enjoy **learning new technologies and exploring the data ecosystem**
- Problem solver — I enjoy debugging pipelines and solving technical challenges
- Always curious — constantly learning something new in **data engineering**

---

Open to Data Engineering Internships & Opportunities

## Connect with Me

- <a href="https://linkedin.com/in/ananurkaromah">LinkedIn</a>
- <a href="https://discord.com/users/1462129586459644118">Discord</a>
