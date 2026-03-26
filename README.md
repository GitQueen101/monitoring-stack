# monitoring-stack

Prometheus + Grafana observability stack with pre-built dashboards.

![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

## Overview

A complete observability stack using Prometheus for metrics collection and Grafana for visualization. Spun up with Docker Compose, pre-configured with dashboards and alert rules, and pointed at a sample instrumented Flask app.

## What is Included

- Prometheus with custom scrape config
- Grafana with pre-built JSON dashboards (committed to repo)
- Alertmanager with example alert rules
- Sample Flask app exposing /metrics endpoint
- Docker Compose for single-command startup

## Tech Stack

- Prometheus
- Grafana
- Alertmanager
- Docker Compose
- Python + Flask + prometheus_client

## Project Structure

```
monitoring-stack/
prometheus/
  prometheus.yml
  alert.rules.yml
grafana/
  dashboards/
  provisioning/
app/
  main.py
docker-compose.yml
README.md
```

## How to Run

```bash
docker compose up -d
```

Then open:
- Grafana: http://localhost:3000 (admin/admin)
- Prometheus: http://localhost:9090
- Sample app: http://localhost:5000

---

Part of the [GitQueen101 DevOps portfolio](https://github.com/GitQueen101).
