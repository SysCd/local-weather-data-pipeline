# 🌦️ Local Weather Data Pipeline

A complete end-to-end **ETL data pipeline** built entirely on local infrastructure — no cloud required.  
This project ingests real-time weather data, processes and transforms it, integrates city metadata, validates data quality, and exposes insights via dashboards and SQL.

---

## 🚀 Features

- 🌐 **Data Ingestion** — Pulls real-time weather data from OpenWeatherMap API
- 🗃️ **Data Storage** — Raw JSON stored locally; processed data in PostgreSQL
- ⚙️ **Data Processing** — ETL pipeline managed with Apache Airflow
- 🔄 **Data Integration** — Combines weather data with city metadata (CSV)
- 🧪 **Data Quality** — Validated using Great Expectations
- 📊 **Data Visualization** — Interactive dashboards via Metabase
- 🐳 **Containerized** — Everything runs locally via Docker

---

## 🛠️ Tech Stack

| Layer               | Tool                    |
| ------------------- | ----------------------- |
| Ingestion           | Python + requests       |
| Scheduling          | Apache Airflow          |
| Storage (raw)       | Local File System       |
| Storage (warehouse) | PostgreSQL              |
| Transformation      | dbt                     |
| Data Quality        | Great Expectations      |
| Dashboard           | Metabase                |
| Containerization    | Docker + docker-compose |

---

## 📁 Project Structure

```plaintext
weather_pipeline/
├── airflow/                  # Airflow DAGs and config
├── data/                     # Raw and processed data
│   ├── raw/
│   └── processed/
├── dbt_project/              # dbt models and configs
├── great_expectations/       # Data validation configs
├── metabase/                 # Optional Metabase config
├── scripts/                  # Data fetch scripts
│   └── fetch_weather.py
├── docker-compose.yml
└── README.md
```
