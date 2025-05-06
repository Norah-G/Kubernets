Kubernetes Hackathon Lab – Widgetario Deployment


This repository showcases our team's successful deployment and hardening of the Widgetario application on Kubernetes as part of a hands-on lab and hackathon. The goal was to simulate real-world deployment challenges and gain practical experience in DevOps, Kubernetes, and production-grade system design.

✅ Achievements
✔️ Deployed multi-service app: products-db, products-api, stock-api, and web UI

✔️ Secured environment variables using ConfigMaps and Secrets

✔️ Integrated persistent storage with StatefulSets and PVCs

✔️ Implemented Ingress routing with DNS simulation and host mapping

✔️ Hardened deployments with probes, resource limits, and non-root containers

✔️ Added observability using Prometheus, Grafana, and centralized logging with the EFK stack

📦 Project Structure
bash
Copy
Edit
hackathon/
├── files/
│   └── grafana-dashboard.json      # Custom dashboard for monitoring
├── solution-part-1/                # Base deployment of all services
├── solution-part-2/                # ConfigMaps and Secrets added
├── solution-part-3/                # StatefulSet, storage, DB replication
├── solution-part-4/                # Ingress configuration
├── solution-part-5/                # Production hardening
└── scripts/
    ├── add-to-hosts.ps1
    └── add-to-hosts.sh             # Local DNS simulation scripts
🌐 Access Points
Web UI: http://widgetario.local

API: http://api.widgetario.local/products

Grafana: http://localhost:3000 (Default creds: admin/admin)

Kibana: http://localhost:5601

Note: Ensure local /etc/hosts entries are configured for DNS resolution.

📊 Monitoring & Logging
Prometheus scrapes metrics from app endpoints

Grafana visualizes system health via custom dashboards

EFK Stack (Elasticsearch, Fluentd, Kibana) aggregates logs from all pods

💬 Team Notes
We tackled real-world issues including:

Misconfigured environment variables

Volume mounting errors

Liveness/readiness probe tuning

Troubleshooting failed rollouts and pending pods

🧠 Lessons Learned
Effective team collaboration is crucial in DevOps

YAML syntax precision matters!

Observability tools are essential for system health

Kubernetes offers flexibility but requires care in configuration

👏 Contributors
Victoria Mwaura
Norah Kimathi 
Joshua Radula 
Maxwell Opondo
