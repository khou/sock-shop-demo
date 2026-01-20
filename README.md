# Sock Shop Demo
Please deploy this after creating a local k8s via kind or minikube.

## Directories

- `manifests/` - Core Sock Shop services
- `manifests-jaeger/` - Jaeger tracing and tracing-enabled service overrides
- `manifests-monitoring/` - Prometheus and Grafana monitoring stack

## Deployment

Use the deploy script from the project root:

```bash
./bin/deploy
```

## Port Forwarding

To access the UIs locally:

```bash
./bin/port-forward
```

Access points:
- Sock Shop: http://localhost:8080
- Grafana: http://localhost:3001 (admin/admin)
- Jaeger UI: http://localhost:16686

**Note:** Pods need to be 1/1 RUNNING before the catalogue shows up in the Sock Shop UI.
