<div align="center">

# Membangun Sistem Machine Learning

### Eksperimen → Model → CI → Monitoring

Proyek akhir pembelajaran **Membangun Sistem Machine Learning (MSML)** yang mendokumentasikan perjalanan sebuah sistem machine learning dari eksperimen hingga monitoring.

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

## Tentang Proyek

Proyek ini merupakan implementasi dari materi dan kriteria proyek akhir kelas **Membangun Sistem Machine Learning**.

Fokusnya bukan hanya membuat model, tetapi memahami bagaimana model menjadi bagian dari sebuah sistem: mulai dari **data preprocessing, eksperimen, training, tracking, automation, serving, monitoring, hingga alerting**.

```text
Eksperimen
    ↓
Membangun Model
    ↓
Workflow CI
    ↓
Monitoring & Logging
```

## Struktur

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

## Alur

### 01 — Eksperimen

Tahap awal digunakan untuk memahami dataset melalui data loading, EDA, preprocessing, dan eksperimen sebelum proses otomatisasi.

### 02 — Membangun Model

Model dilatih menggunakan dataset yang telah melalui preprocessing. Eksperimen training menggunakan **MLflow** untuk tracking dan penyimpanan artefak. Pada tahap lanjutan, tuning dan tracking dikembangkan menggunakan **DagsHub**.

### 03 — Workflow CI

Workflow CI digunakan untuk mengotomatisasi proses retraining ketika workflow dipicu. Bagian ini menggunakan **MLflow Project** dan **GitHub Actions**, dengan Docker sebagai bagian dari implementasi lanjutan.

### 04 — Monitoring & Logging

Model kemudian disajikan dan dipantau menggunakan **Prometheus** untuk pengumpulan metrik, **Grafana** untuk visualisasi, dan **Grafana Alerting** untuk peringatan.

## Monitoring

Dashboard mencakup metrik seperti:

- HTTP requests
- HTTP request failures
- Request duration
- Request throughput
- Prediction classes
- CPU usage
- RAM usage
- Disk usage
- Network traffic

Alerting juga digunakan untuk beberapa kondisi seperti penggunaan CPU, durasi request, dan request yang gagal.

## Catatan

Proyek ini dibuat sebagai bagian dari proses pembelajaran. Dokumentasi, struktur, dan artefak merepresentasikan proses eksperimen dan implementasi selama pembelajaran.

Tidak semua bagian di sini dimaksudkan sebagai sistem production-ready.

---

<div align="center">

### Built by experimenting, breaking things, and trying again.

</div>
