<div align="center">

# Building a Machine Learning System

### Experiment → Model → CI → Monitoring

A final learning project for **Building a Machine Learning System (MSML)** documenting the journey from experimentation to an actively monitored machine learning system.

<div align="center">

[![GitHub Last Commit](https://img.shields.io/github/last-commit/himbarbuana/membangun_sistem_machine_learning?style=flat-square)](https://github.com/himbarbuana/membangun_sistem_machine_learning/commits/main)
[![GitHub Repo Size](https://img.shields.io/github/repo-size/himbarbuana/membangun_sistem_machine_learning?style=flat-square)](https://github.com/himbarbuana/membangun_sistem_machine_learning)

</div>

<div align="center">

[![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![MLflow](https://img.shields.io/badge/MLflow-2.19.0-0194E2?style=flat-square&logo=mlflow&logoColor=white)](https://mlflow.org/)
[![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-CI-2088FF?style=flat-square&logo=githubactions&logoColor=white)](https://github.com/himbarbuana/membangun_sistem_machine_learning/actions)
[![Prometheus](https://img.shields.io/badge/Prometheus-Monitoring-E6522C?style=flat-square&logo=prometheus&logoColor=white)](https://prometheus.io/)
[![Grafana](https://img.shields.io/badge/Grafana-Dashboard-F46800?style=flat-square&logo=grafana&logoColor=white)](https://grafana.com/)

</div>

`Python` · `MLflow` · `DagsHub` · `Docker` · `GitHub Actions` · `Prometheus` · `Grafana`

</div>

---

## About

This project is an implementation of the materials and requirements from the **Building a Machine Learning System** final project.

The focus is not simply training a model, but understanding how a machine learning model becomes part of a larger system — from **data preprocessing, experimentation, training, tracking, automation, serving, monitoring, and alerting**.

```text
Experimentation
      ↓
Model Development
      ↓
CI Workflow
      ↓
Monitoring & Logging
```

## Structure

```text
.
├── eksperimen_sml_muhammad_himbar_buana.txt
├── membangun_model/
│   ├── modelling.py
│   ├── modelling_tuning.py
│   ├── requirements.txt
│   ├── DagsHub.txt
│   ├── telco_customer_churn_preprocessing.csv
│   └── screenshots & artefacts
├── monitoring_dan_logging/
│   ├── 1_bukti_serving/
│   ├── 2_prometheus.yml
│   ├── 3_prometheus_exporter.py
│   ├── 4_bukti_monitoring_prometheus/
│   ├── 5_bukti_monitoring_grafana/
│   ├── 6_bukti_alerting_grafana/
│   ├── 7_Inference.py
│   └── telco_customer_churn_preprocessing.csv
├── workflow_ci.txt
├── README.md
└── README_EN.md
```

## Workflow

### 01 — Experimentation

The first stage focuses on understanding the dataset through data loading, EDA, preprocessing, and initial experimentation before automation.

### 02 — Model Development

The model is trained using the preprocessed dataset. Training experiments use **MLflow** for experiment tracking and artefact storage. In the advanced stage, tuning and tracking are extended with **DagsHub**.

### 03 — CI Workflow

The CI workflow automates model retraining whenever the workflow is triggered. This stage uses **MLflow Project** and **GitHub Actions**, with Docker included as part of the advanced implementation.

### 04 — Monitoring & Logging

The resulting model is served and monitored using **Prometheus** for metrics collection, **Grafana** for visualization, and **Grafana Alerting** for notifications.

## Monitoring

The dashboards cover metrics related to:

- HTTP requests
- Failed HTTP requests
- Request duration
- Request throughput
- Prediction classes
- CPU usage
- RAM usage
- Disk usage
- Network traffic

Alerting is also configured for selected conditions such as CPU usage, request duration, and failed requests.

## Notes

This project was created as part of a learning process. The repository contains the experiments, implementation, documentation, screenshots, and artefacts produced throughout the course.

Not every component should be considered production-ready.

---

<div align="center">

### Built by experimenting, breaking things, and trying again.

</div>
