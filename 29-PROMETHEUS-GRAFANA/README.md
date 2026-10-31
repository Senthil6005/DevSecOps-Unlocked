# 29 – Prometheus & Grafana

**Phase:** 📊 Monitoring

## 📘 What is Prometheus & Grafana?
Prometheus collects metrics; Grafana visualizes them in dashboards and sends alerts.

## 🛡️ Why it matters in DevSecOps
You can't secure what you can't see. Unusual spikes in errors or traffic are often the first sign of an attack.

## 🔑 Key Concepts
- Metrics, exporters, scraping, PromQL
- Alertmanager
- Grafana dashboards & alerts
- kube-prometheus-stack Helm chart

## 💻 Important Commands / Example
```bash
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm install monitoring prometheus-community/kube-prometheus-stack -n monitoring --create-namespace
```

## ❓ Interview Questions
1. What is an exporter?
2. Pull vs push monitoring?
3. Which metrics can indicate a security incident?

## 📝 Practice
- Install the tool in your lab and run the commands above.
- Add it as a stage in your Jenkins or GitHub Actions pipeline.
