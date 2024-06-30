# ArgoCD Helm Chart

This Helm chart deploys ArgoCD along with environment-specific configurations for dev, qa, stage, and prod environments.

## Pre-requisites
- Kubernetes 1.16+
- Helm 3.0+
- An Ingress controller (e.g., NGINX Ingress Controller)

# Install the Chart
Use the following commands to install the chart for each environment. Replace your-release-name with the desired release name.

### For Development Environment:
helm install argocd ./argocd-helm-chart -f dev.yaml

### For QA Environment
helm install argocd ./argocd-helm-chart -f qa.yaml

### For Staging Environment
helm install argocd ./argocd-helm-chart -f stage.yaml

### For Production Environment
helm install argocd ./argocd-helm-chart -f prod.yaml

# Upgrading the Chart
To upgrade the chart for a specific environment, use the following commands:

### For Development Environment
helm upgrade argocd ./argocd-helm-chart -f dev.yaml

### For QA Environment
helm upgrade argocd ./argocd-helm-chart -f qa.yaml

### For Staging Environment
helm upgrade argocd ./argocd-helm-chart -f stage.yaml

### For Production Environment
helm upgrade argocd ./argocd-helm-chart -f prod.yaml
