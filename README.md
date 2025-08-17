# kans-monitoring-stack — Prometheus + Grafana Monitoring & Alerts

## Description
This project demonstrates a complete monitoring and alerting setup for a demo application using Prometheus and Grafana. It includes:
- Prometheus for metrics collection
- Grafana for visualization with dashboards
- Alerting rules for application downtime

This setup showcases observability skills in DevOps portfolios.

## Features
- Prometheus scraping demo app metrics
- Grafana dashboard visualization
- Alerting rules for app downtime
- Modular folder structure for clarity

## Folder Structure
kans-monitoring-stack/
├── prometheus/       # Prometheus configuration
├── grafana/          # Grafana dashboards
├── alerts/           # Alerting rules
├── README.md         # Project documentation
└── .gitignore        # Optional ignore files

## Prerequisites
- Docker installed (optional for containerized Prometheus/Grafana)
- Prometheus and Grafana installed or containerized
- Demo app running on localhost:3000

## Steps to Run Locally
1. Start Prometheus:
   prometheus --config.file=prometheus/prometheus.yml
2. Start Grafana:
   grafana-server --homepath grafana
3. Import dashboard from grafana/dashboard.json
4. Apply alert rules in Prometheus:
   prometheus --config.file=prometheus/prometheus.yml --rule.file=alerts/alert.rules
5. Access Grafana dashboard at http://localhost:3000 (default port)

##  Author
**Muhammed Kans**  
- GitHub: [kans-devops](https://github.com/kans-devops)  
- Repo: [kans-docker-ansible](https://github.com/kans-devops/kans-docker-ansible)  
- Email: kans.devops.engineer@gmail.com
 
