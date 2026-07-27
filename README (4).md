<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=220&section=header&text=Vihari%20Reddy&fontSize=60&fontColor=C9A9FF&animation=fadeIn&fontAlignY=38&desc=Data%20Engineer%20%7C%20Building%20Scalable%20Data%20Pipelines&descAlignY=58&descSize=18"/>

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&duration=3000&pause=1000&color=A78BFA&center=true&vCenter=true&width=650&lines=Data+Engineer;ETL+%7C+Data+Pipelines+%7C+Cloud+Data+Platforms;Python+%7C+SQL+%7C+PySpark+%7C+Airflow;Snowflake+%7C+Redshift+%7C+BigQuery;Open+to+Data+Engineering+Roles" alt="Typing SVG" />
</a>

<br/>

![MS in IT](https://img.shields.io/badge/M.S.-Information%20Technology-6D28D9?style=for-the-badge&labelColor=0f0c29)
![Recent Grad](https://img.shields.io/badge/Status-Recent%20Graduate-4C1D95?style=for-the-badge&labelColor=0f0c29)

<br/>

<a href="https://www.linkedin.com/in/viharireddy2/"><img src="https://img.shields.io/badge/LinkedIn-7C3AED?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0f0c29" /></a>
<a href="https://github.com/viharireddy2-byte"><img src="https://img.shields.io/badge/GitHub-5B21B6?style=for-the-badge&logo=github&logoColor=white&labelColor=0f0c29" /></a>

<br/><br/>

</div>

---

## 🧠 About Me

I'm a **Data Engineer** and recent Master's graduate in Information Technology, focused on designing and building reliable, scalable **data pipelines** and **cloud data platforms**.

- 🔭 I build **ETL/ELT pipelines** using **Python, SQL, and PySpark** to move and transform data at scale.
- 🌬️ I orchestrate workflows with **Apache Airflow** and stream data using **Kafka**.
- 🧱 I model and transform data using **dbt**, following clean, testable data modeling practices.
- ☁️ I work across **Snowflake, Redshift, and BigQuery**, and deploy on **AWS, Azure, and GCP**.
- 🐳 I containerize and ship data workflows using **Docker**.
- 📊 I care about **data quality, pipeline reliability, and performance** at every stage.

**🎯 Open To:** Data Engineering · Data Platform Engineering · Analytics Engineering · ETL Development

---

## 🛠️ Tech Stack

**Languages**

![Python](https://skillicons.dev/icons?i=python)
![SQL](https://img.shields.io/badge/SQL-4C1D95?style=flat-square&logo=postgresql&logoColor=white)

**Data Processing & Orchestration**

![PySpark](https://img.shields.io/badge/PySpark-7C3AED?style=flat-square&logo=apachespark&logoColor=white)
![Airflow](https://skillicons.dev/icons?i=airflow)
![Kafka](https://skillicons.dev/icons?i=kafka)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-6D28D9?style=flat-square&logo=pandas&logoColor=white)

**Cloud Data Warehouses**

![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)
![Redshift](https://img.shields.io/badge/Redshift-8C4FFF?style=flat-square&logo=amazonaws&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-669DF6?style=flat-square&logo=googlebigquery&logoColor=white)

**Cloud, DevOps & Tooling**

![AWS](https://skillicons.dev/icons?i=aws)
![Azure](https://skillicons.dev/icons?i=azure)
![GCP](https://skillicons.dev/icons?i=gcp)
![Docker](https://skillicons.dev/icons?i=docker)
![Git](https://skillicons.dev/icons?i=git)
![Linux](https://skillicons.dev/icons?i=linux)

---

## 📊 Core Data Engineering Expertise

<div align="center">

| Domain | Proficiency | Details |
|---|:---:|---|
| **ETL / ELT Pipeline Design** | ⭐⭐⭐⭐⭐ | Batch pipelines with Python, SQL, PySpark |
| **Workflow Orchestration** | ⭐⭐⭐⭐ | DAG design and scheduling with Apache Airflow |
| **Stream Processing** | ⭐⭐⭐⭐ | Event-driven pipelines using Kafka |
| **Data Modeling & Transformation** | ⭐⭐⭐⭐ | dbt models, testing, and documentation |
| **Cloud Data Warehousing** | ⭐⭐⭐⭐ | Snowflake, Redshift, BigQuery schema & query design |
| **Cloud Infrastructure** | ⭐⭐⭐⭐ | AWS, Azure, and GCP data services |
| **Containerization** | ⭐⭐⭐ | Dockerized pipeline components |

</div>

---

## 🚀 Featured Projects

<details>
<summary><b>📦 Lakeflow Sync — Postgres CDC to Databricks Lakehouse</b></summary>
<br/>

A dual-mode ingestion pipeline that lands PostgreSQL data into a Databricks Lakehouse Bronze layer — a `full_load` mode for backfill snapshots, and a `cdc` mode that streams insert/update/delete events off the Postgres write-ahead log into an immutable, append-only event log where no row is ever overwritten in place.

| Attribute | Detail |
|---|---|
| **Stack** | Python 3.11, dlt, PySpark, Databricks (Unity Catalog, Delta Lake), PostgreSQL logical replication, Databricks Asset Bundles, GitHub Actions |
| **Scale** | Dual-mode ingestion across dev/QA/prod catalogs via logical isolation |
| **Performance** | Retry with failure classification — transient errors backed off, permanent errors fail fast, invalidated replication slots raised distinctly |
| **Security** | OAuth Service Principals, Unity Catalog access control, secrets-managed credentials |
| **Impact** | Post-load data quality gate blocks bad data before a job is marked successful; real end-to-end CDC integration tests against a live replication slot |
| **Repository** | [View Repo](https://github.com/viharireddy2-byte/lakeflow-sync) |

Deliberately scoped to Extract & Load only — no in-pipeline transformation — so an upstream schema hiccup can be triaged independently of downstream Silver/Gold logic. Ships with structured JSON logging, run-outcome notifications, and CI/CD via Databricks Asset Bundles across dev, QA, and production environments.

</details>

<details>
<summary><b>🛡️ Agentic Aegis — Self-Healing Data Pipeline</b></summary>
<br/>

A data quality system where four autonomous agents sit inside the pipeline itself — one profiles the data, one scores it, one fixes what it can, and one watches for anomalies a fixed rule set would never catch — all landing in a DuckDB-backed Medallion architecture with a 7-page Streamlit dashboard on top.

| Attribute | Detail |
|---|---|
| **Stack** | Python, Polars, DuckDB, Prefect, Pandera, scikit-learn (IsolationForest), Streamlit |
| **Scale** | Bronze → Silver → Gold medallion layers, in-process OLAP with zero server overhead |
| **Performance** | Multi-threaded, Arrow-native processing via Polars and DuckDB |
| **Security** | Pandera schema contracts enforce a guaranteed shape on the Silver layer, not just a hopeful one |
| **Impact** | Explainable 0–100 quality score tracked run-over-run, full audit trail on every remediation, statistical drift and anomaly detection beyond static rules |
| **Repository** | [View Repo](https://github.com/viharireddy2-byte/Agentic-Aegis) |

Separates detection from correction by design — ScoutAgent only finds problems, HealerAgent only fixes them, SentinelAgent scores overall pipeline health, and OracleAgent runs IsolationForest-based anomaly and cross-run drift detection.

</details>

---

## 🎯 Current Focus

```yaml
current_focus:
  learning:
    - Advanced Airflow DAG design and orchestration patterns
    - Cloud-native data platform architecture
  building:
    - Batch and streaming data pipelines
    - dbt-based data modeling layers
  exploring:
    - Data quality and observability tooling
    - Cost optimization in cloud data warehouses
  open_to:
    - Data Engineering roles
    - Data Platform / Analytics Engineering roles
```

---
---

## 📬 Connect

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-7C3AED?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/viharireddy2/)
[![GitHub](https://img.shields.io/badge/GitHub-5B21B6?style=for-the-badge&logo=github&logoColor=white)](https://github.com/viharireddy2-byte)

</div>

---

<div align="center">

*"Turning raw data into reliable pipelines, one job at a time."*

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=120&section=footer"/>

</div>
