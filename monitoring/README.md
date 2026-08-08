# Monitoring

This project is designed to be monitored with Prometheus and Grafana.

## Suggested Monitoring Stack

- **Prometheus**: For collecting metrics
- **Grafana**: For visualization and dashboards
- **cAdvisor**: For container metrics (optional)

You can deploy a basic monitoring stack using Docker Compose or Helm charts.

### Example metrics to monitor:
- Application health (`/health` endpoint)
- Container CPU and Memory usage
- Request count and response time
