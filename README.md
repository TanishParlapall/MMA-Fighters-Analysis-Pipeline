# 🥋 MMA-Fighters-ETL-Pipeline
An Airflow-orchestrated ETL pipeline that ingests MMA data from an external API, stages raw records, and loads data into a PostgreSQL table for downstream analytics. Transformed data is then connected to Power BI to build interactive visualizations and perform analytical comparisons.
---

## 🤖 Technologies
- `Python`
- `SQL`
- `Airflow`
- `PostgreSQL`
- `Power BI`
- `Docker`

## 🚀 Features
- Fetches MMA data from the Sports Data API
- Transforms and loads data into PostgreSQL
- Schedules weekly execution using Airflow
- Runs using Docker
- Data can be connected to Power BI for analysis

## 🧱 Project Structure
```
MMA-Fighters-ETL-Pipeline/
├── dags/
│   ├── dag.py
│   ├──scripts/
│       ├── create_table.py
│       ├── extract_data.py
│       └── load_data.py
├── docker-compose.yml
├── requirements.txt
├── .env.example
├── README.md
```

## 🔄 DAG Overview
![dag structure](https://github.com/TanishParlapall/MMA-Fighters-ETL-Pipeline/blob/main/images/dag-structure.png)

## 🙋 This project explores the following questions:
- How does average wingspan and height compare between champions and non-champions within each weight class?
- What percent of finishes in MMA come via knockout vs. submission?
- How does finish type vary across weight classes?


## 📈 What the data says...


<table align="center">
  <tr>
    <td><img src="https://github.com/TanishParlapall/MMA-Fighters-Analysis-Pipeline/blob/main/images/finish-pie-chart.png" width="350"></td>
    <td><img src="https://github.com/TanishParlapall/MMA-Fighters-Analysis-Pipeline/blob/main/images/finish-comparison.png" width="500"></td>
  </tr>

  <table align="center">
  <tr>
    <td><img src="https://github.com/TanishParlapall/MMA-Fighters-Analysis-Pipeline/blob/main/images/height-comparison.png" width="700"></td>
  </tr>
  <table align="center">
  <tr>
    <td><img src="https://github.com/TanishParlapall/MMA-Fighters-Analysis-Pipeline/blob/main/images/wingspan-comparison.png" width="700"></td>
  </tr>
