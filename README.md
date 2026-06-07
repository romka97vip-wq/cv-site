# CV Site

Personal CV website. Static HTML page hosted in Kubernetes.

## Stack
- HTML/CSS (no JS framework)
- Nginx (static server)
- Docker
- Kubernetes (K3S)

## Structure
- `src/` — application source (index.html, Dockerfile)
- `k8s/` — Kubernetes manifests (Deployment, Service)

## Deploy

Build Docker image:
\`\`\`bash
docker build -t cv-site:latest src/
\`\`\`

Apply K8S manifests:
\`\`\`bash
kubectl apply -f k8s/
\`\`\`

## Routing
Available at: `https://devopsrk.duckdns.org/` (via Ingress)
