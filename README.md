# LibreChat Helm Chart

## Description
This Helm chart deploys LibreChat, an open-source chat application, on a Kubernetes cluster.

## Prerequisites
- Kubernetes 1.25+
- Helm 3.0+
- PV provisioner support in the underlying infrastructure
- MongoDB (required for LibreChat)

## Installation

### Add the Helm Repository
```bash
helm repo add librechat https://bayzip.github.io/librechat-helm/
helm repo update
helm install librechat librechat/librechat -n librechat --create-namespace

# To install with custom values:
helm install librechat librechat/librechat -f values.yaml  --create-namespace
```
